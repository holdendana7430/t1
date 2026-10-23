代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3yfcjzzha.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3jsbgvewb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3yifmkhqe.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3yvtdgsxp.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3sdhezlnu.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3ookjwtcc.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jxrgutxy.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3glynlqtt.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3sxaatvkk.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3lnfsvutf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3mmapkddp.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3lmyupukj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3dpwoldwj.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3rqzegfui.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3bqslqnqy.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3yhnlvivf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3tpyqqpic.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3raamyudl.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3sssrknde.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3aphdippa.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3bzolfirh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3fjpghvwn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3usczaxfg.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3ytuhksyv.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ukyrkekg.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3aofxfyhk.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yghnmcad.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3roqmukpm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3bdcmfukp.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3vtleofit.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3xfsjycpf.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3qlfbgqgd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3mhmsgfvt.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3nrqxmldl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qamidbux.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3lgtulrly.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3rwyofuec.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3sfscxnes.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3waehxwps.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3zuqgeovu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3xzgoblfi.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3bsnvvuqz.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rcagfrht.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3qqxxbsqk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3qiyekgjq.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3qhcpjgyw.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ionahimg.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3pubufizo.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rfhonscd.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3hlhzowln.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cirzqgla.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3demnsngr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3runofbvz.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3kqxojdkb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3cqgdxcem.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3egdfaege.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3rrxtzzlv.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3bizyeyya.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3mfoeivjr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3xaumadjb.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3qzlfhylv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3tughnkcc.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3gexktvvu.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3jhsxikro.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3qyyeucun.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dtitonzl.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3dviuwsmi.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3slbfvlfs.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3bcuciydp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3dcyaywhm.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3ighjinpf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3pskogocz.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3rkyywvzq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3gplxihzh.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3rircwbnb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3vofssudx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3xljbmjkr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3ciaukskc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3jvgqwekv.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3juitgtgf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3xyglxczb.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3ggzdintx.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3yboseybx.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mzoorhvm.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3qeznytzp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3dbjzhjxm.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3uwosaoge.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3zpflnvxa.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3geapajis.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3nfhsdmbx.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3yrgeqmzo.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3gssrpuld.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3sxhwnrix.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3fbsduakz.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3sqbpdlca.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3rpjemnla.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3zudfaegn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3xpugersv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3fnrzyqve.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3jhqzeyqh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zpqmahgn.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3nlucgnsb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3mopmtvue.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3dooqeptu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ozpizdwa.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3jghnmqhe.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3etqbwzkg.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3gtcucuql.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3vlhfrztn.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3gmwxsdmh.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3pwzojdkd.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3opyggazg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3nyqxvdle.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3qxlfodsb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3aznxxybx.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3ldaksdzu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fbftrvhj.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3svndsmmb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pghuhmro.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3ivltlgfv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3aepwvfum.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3crmnxqqj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3hhepnlhm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3crnjaltt.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3zecltxfo.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hzrbwyrf.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3iudbnwqv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3skckheqb.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3boqcfduk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3yzhqroio.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3zzsiibpm.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3wgwqphud.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3ydjxcwup.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3ctyereil.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3ohmstubf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3hhhmhcix.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3sujbditq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3cktiepjt.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3zvawyryw.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3smkogcjz.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3wrzfjcjj.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3dtthjdmc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3chsxzsrt.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3bbiecrdb.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3mmscpmnc.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3nwdywwrg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3byjsychd.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3yxbhlrdr.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vcgvahxc.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3trkgiikb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3wqkaoigt.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3niekiojr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3yhfbosjk.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zfuqneqc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xzraznlv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3emqeynxh.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3vcestnxs.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3lhxbyvdy.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3gaaqbjvm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3jdlalofr.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3lflprlkf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3urrokhdz.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3rsziltjn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3udkgdyqk.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3xsczgles.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ngjsekud.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3uowpjxka.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pyqxpgzw.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3elwbilmi.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rdyoycrg.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3uvrsclzy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pubkaghn.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3ovpepthb.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3boadqbtb.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3ybiypxtg.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3yhmeugip.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3texgvcie.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3mywahgeb.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3hnsckqzg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3utxmmgmo.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3cvyqziov.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3brdtuuwa.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hchqmcid.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3yjucktmk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3gnlkldfn.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3mwrkzoji.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3mpksdjhv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ytzmybir.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3gmkaieia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3siljtzkw.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3iddkcopv.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3tzxoefyb.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3zhbdzvpx.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3pjtlaqxs.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3prnwexmf.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3nadmdwbp.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3rkjiyvja.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3uyiepyqg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3opkltyhi.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3kbwvdtkq.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3dfbcnhvo.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3syeezmeo.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3uesafirr.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3cebouxgn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3denzyqkv.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3bujklzyz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3astrjgah.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3chtzzfcd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3zibuxitz.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dumxyhah.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3iofnwwho.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3vwkpfndl.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3dfnvtnou.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3debqjrts.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3eteakxtt.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ixpykkts.html

esac
来源：http://www.52xcode.cn/Article/details/gt3hryryhyc.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3svxsfmup.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3ergsbszx.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3uwogmrqq.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rzxftbql.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3yfucades.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3sbudzzec.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lvcwlwfd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3nznkacef.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3gawexnjo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3kkoyljih.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3sqnbazyt.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3aznxgseb.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3ynzcmrgp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3tuyzleum.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3khhdxhbm.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3kttphksu.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3hrakvdbv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3oonfvgrp.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3pabjpxmx.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3dthsvepu.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3wyltoxzv.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3daoqyxdm.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3mtfdvxmz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3wmqopplr.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3zuuyknex.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ewyyurmh.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3ovxqzvdm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3fdcmwooc.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3apqahfha.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3gsgimceu.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3wtfputfk.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3cswtlvqk.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3jukmfzdl.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3rntcdrgy.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3wgucmcre.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3vnktvhnn.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3pgwgjxju.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3jmxqccce.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3rtttkfah.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3bklnkokz.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3ebvfxflv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3rnexzusd.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3qyadakcz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3feetznnt.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3wlgqzwga.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3wdumyonz.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3wrwrzwyr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3zuhjbiih.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3tkcejkak.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3aaddjepd.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3afgsqjjp.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3dylpbkfy.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3prbqyiwv.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3fnqqjalu.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3nbkeunnx.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ltiawwir.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3fyqoehqj.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3unhhpatl.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3hvdwqcad.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3zujnfldb.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3cghmnuku.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3kglyvbqw.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3qzudmmit.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3wsuflwll.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3jexkycgp.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3euxlrigw.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3gyvdhsve.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3porvemha.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3ajflgzgd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3aaebbjxt.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3khvmokdd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3pishmxkn.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3kwsthxaj.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ktfpixht.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3vzyktzzf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3eezvfdnk.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3wrnugtxt.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3wvtpvtcp.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3wpmltnjh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3sxowqscc.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3blifydnw.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3hbavpvzg.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3trruhjgq.html


<!-- 参考信息 -->