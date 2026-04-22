MATCH (p:Persona)-[:GESTIONA]->(pr:Proyecto)
WHERE NOT (p)-[:PARTICIPA_EN]->(pr)
RETURN p.nombre AS Gestor, pr.nombre AS Proyecto;
