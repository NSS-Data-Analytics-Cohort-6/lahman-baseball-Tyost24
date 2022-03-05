/* 1:  SELECT DISTINCT yearid
from teams
UNION ALL
SELECT DISTINCT yearid
FROM collegeplaying
ORDER by yearid;

Answer 1864 to 2016 */

/*2: 

SELECT Distinct p.namefirst, p.namelast, p.height, p.playerid, a.g_all, t.name
FROM people AS p
LEFT JOIN appearances as a
ON p.playerid = a.playerid
LEFT JOIN teams as t
on a.teamid = t.teamid
order by p.height*/


/*Answer Eddie Gaedel was the shortest player at 43CM, he played in one game for the St.Louis Browns*/ 

/* 3:  

SELECT DISTINCT CONCAT(cast(p.namefirst as text), ' ', cast(p.namelast as text)) AS full_name,
	   SUM(s.salary) AS total_salary,
	   LOWER(c.schoolid)
FROM people as p
LEFT JOIN salaries as s
ON p.playerid = s.playerid
LEFT JOIN collegeplaying as c
ON s.playerid = c.playerid
WHERE s.salary IS NOT NULL AND c.schoolid IS NOT NULL AND LOWER(C.schoolid) LIKE 'vand%'
GROUP BY full_name, c.schoolid
ORDER BY total_salary DESC

Answer: David Price earnedd the most. */





