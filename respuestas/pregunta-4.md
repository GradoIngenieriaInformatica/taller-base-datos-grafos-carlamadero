MATCH (p:Persona)-[:PARTICIPA_EN]->(pr:Proyecto)
RETURN pr.nombre AS Proyecto, count(p) AS NumParticipantes
ORDER BY NumParticipantes DESC
LIMIT 2;
