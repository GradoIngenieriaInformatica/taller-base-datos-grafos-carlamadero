MATCH (p:Persona)-[:ESTUDIO_EN]->(u:Universidad)
RETURN u.nombre AS Universidad, count(p) AS NumEstudiantes;
