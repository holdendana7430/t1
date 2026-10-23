代发 wailian999

);
来源：http://www.52xcode.cn/Article/details/gt3xseancoo.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3mgujcrgz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3obvactgz.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3xlgcqmgx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3cnyovqxt.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3emvbncqb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3edryuuqe.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3zfmjudwb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3cbsxkvbs.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3byyucsew.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nyleufdi.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3yfzgmgjw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3fqkcbrjm.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3hfdlhrxm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3diramzkp.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3wtewhfry.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ffjrwjdv.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3sfllvgke.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ebzivhij.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3pezbtqej.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3sadravoc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3yimfcbik.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3cugacuyq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3pirirjks.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3tlyfhvfn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3jmtxupps.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3thosytpg.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3dtoozwaa.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mgaqdhjz.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ktbtocyq.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3konmkcsa.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3kibppwtu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3goaatbaq.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zsoaagas.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3bwwecyrn.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3qrfboayu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3kmwtukgq.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3dxflisan.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ftpfrzhs.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3aomhwivs.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3zriogrpm.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3taenkjbg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3dppnkqda.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3dhtgajsf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3ccrjnrcb.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3zfhpfyjd.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aeltzrgq.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3grjjubgl.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3pdbjhksb.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3jtmuyqfy.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wifxfymp.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3mttlmhfl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fbildyif.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3ddgafhvl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3usadhmey.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3yllkwvug.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uduzuxqn.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3zqdqpnst.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3iirfblkd.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3jfcmhngj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3osesxfsk.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tcgslsdc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3nvnxfscy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3wonjshoz.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3wicttdzq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3mgrptlfy.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3bhipfvsp.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3zmkgmxxj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3wtreqgfz.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zhfercou.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3cufbjzqk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3quiptwnu.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3bxidhkhj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3lqmqtxfq.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3yueiegow.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3dgdxbjki.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3xyzfykyk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3rwzlgemg.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3zdimogws.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3htdfybuk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3wkbaghsq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3wojrhdwq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3sqtcqegu.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3tdjybqsm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3dhneeovh.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3aqjwxwhw.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3icfswwqa.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3afnmlrmb.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3tphakzik.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3vxrdrdtx.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3uzjjubdp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3rnkhchtw.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3bbycmvdn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3decmayoo.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3xbvzxlfl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3vzlkqbuv.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3eoxqxozj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3vaffymoh.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3wbrxojwq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3prttvcuw.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3kxfgrjoa.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3uvyrrfqk.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3kddvaanf.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3ixldutjc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3wdoybqov.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3ajkqiqgj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3tphlnxtc.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3rzpenlce.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3cjnyucud.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3pptjrkrv.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3dmrmbzws.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3nzguskov.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3vglttxwe.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3ryopufhe.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3ysvfbrnr.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3gpgmyqvd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3runydzxq.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3zackudky.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3zdqtlztc.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3zaroyzax.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zdwtxzxm.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3thvgsird.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xszzczdr.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3bnohfsot.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lyutxrnl.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3gjbavvpl.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3akbocjft.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cpdcdcpi.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3vkqridxb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qdeifmcx.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3fedlknrk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3pascqsqh.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3ookdlufq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3pdwuqjlf.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3oghkghch.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3mesflqbm.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3rtareuyo.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3lvtxdbmu.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3enehsamw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3yqakrrgu.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3bbymfgbx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3gedlqikk.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3vxnyvetu.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3cwwbnnzr.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3slpsnwur.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3hrxefakj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3vprihluk.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3omnbmbgp.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3nbyrmdnb.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3ryfikqdv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3fokazgir.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3urhdhgds.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dtzodcum.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3izbccrhe.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ntjwqqqe.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3ugeddjvd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3cdecdaye.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3zhftdymp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kqaeowcy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3qprqykjk.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3orjuitcx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3wdftapiu.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3hkrpnbfm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3rnxdmrhp.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3svhoshkx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3gkyqream.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ewnpyvih.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3tergzslz.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3fuuhwvue.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cwdsbvmg.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3beijyhaz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3twiaroaj.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3nrbkjmgb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bwdhregh.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3jmpmyjwp.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bniwbrdx.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3wmxvjrkn.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fbmmkbnt.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3gpnuftxj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3fckucfwr.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3wbdoeapr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3lyikhovg.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3wxmpnfuh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3eklgzuqh.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3amxzyhgl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3pfxgyuth.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qpyhnjnw.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3maunbqei.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3geynhqpi.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3tpawajdp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3klnoyvag.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fddqfjym.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3kmsnuncb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mdofiptu.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3rszibhqu.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3nflvmudl.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3uleyscom.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3izlvuinb.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3tzpwngph.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3yviesdlc.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3cjsldpiq.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3tolgyhnz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3jegmwrkj.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3vorhqycn.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3rvpmeyok.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3vulldunw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3gedxpzpf.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3yvbprgxh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3mlmrndgp.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3fqhgyffc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3vnknkswo.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3nwxrbzks.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3gsztbpsh.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gfumccgn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hieqgsmm.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3lofurxna.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3yjbsjhba.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3kynbfhof.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3gatnpfjc.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3lqueyjtl.html

esac
来源：http://www.52xcode.cn/Article/details/gt3reellabm.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3fzwlxaxj.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zamuzdwh.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3aorktqtr.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3umfmptlq.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3rzxkylgf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zqqwywkq.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3gaognggd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kdwueikj.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3ocihriol.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3sjvqveqb.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3esmjwboq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3tamkskaq.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3cqdtnsva.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ikcdgghc.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3qnquqwqm.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3jvwmpsio.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3hgygtymq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3verhjqgx.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3eoyxksef.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3gyaacmrd.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3jkejplic.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3pfkuafhv.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3univmyql.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3gyojrihg.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3xauennmz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3hejecrbp.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3qrxkbikz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3fetuzxeq.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3whcnideq.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3waayafky.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3xjrunvnq.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3sfhjngnk.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3eotvtvso.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3nmowtand.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3gycnmzar.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3fizutmqk.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3clzsdzak.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3bcbpoefn.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3gmmhknis.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukehzsdf.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3hsvwcxhy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3bymzawvk.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3dwignldb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3wizcyaqr.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3srrjndox.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3vygscvds.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3fzgwamlx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3jqmfkvnf.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3mlfiycof.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3cauokpyo.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3xbvcpgzq.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3bsgguqrx.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3ltymfitj.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3ynjkiaey.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3zdjxfrzo.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ziazxpsd.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3kpnpnrgn.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3aecelinb.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3rbonpmxs.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3vktnuzxp.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3rccnchfw.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3qbkriswk.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3bplhurlk.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3teaygjds.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3iehowspf.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3urwtnquw.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3mtatitwc.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3nwwtlflk.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3vvbwlybq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3tnqqzxzc.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3yzdmplbu.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3pyuyalrw.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3vwtriiud.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mcihfgen.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3wvccbubr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3bhrobope.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3yhglfmwr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3oahmjfjf.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3fyjdmuig.html


<!-- 参考信息 -->