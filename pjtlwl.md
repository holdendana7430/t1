代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3reyebpwa.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3rfkuistp.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3hvgyyssf.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3grbnzgcs.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3hcakuyjh.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3ciymcqpd.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zneewdkx.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3ggsfhbjb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3mnzmmzpx.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3umklfzpy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3madlitil.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3qaxrlhzd.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3mywvnlsh.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3eghnzvlr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ullgsowf.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3raifbgph.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3ijqduxhg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3qcueswsd.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3oujohsda.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3fkkeesmj.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3hroovewp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3pxhqkmvz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3yqshnuoc.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3zbrziwuu.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yhmabbka.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3apajbiqv.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qywafqkd.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3leoxxqcv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qilsywir.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lhigsajn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3ppciruyy.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3brbponji.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3lndpchmg.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ixhpxexo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3wueepmwc.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3lhyjitnj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3hzhnqwpr.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3datgrndb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3ndbfebav.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3wsrthxjn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3orhonshi.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3zuctplfd.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bfyhmqvg.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3xsakvrju.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3xcxnlidm.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3fkslpdew.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ewojlavn.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3tkzdgcoe.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pjpdokkb.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3gupoxecb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pzezirgd.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3qanaoupr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ezsspehk.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3oozqsnsa.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3mailytja.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3rxqlgpsf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3sglvjtry.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hfdbhgix.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3bsbidkuo.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3rkbpjelm.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3hwlslcyt.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3eoqrsysi.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3gbzqgbrx.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3lgcqdkxm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3rtqiimsw.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3imhyuabw.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3xrguahea.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3dqbnpepx.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3cipncthi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3lnripuqv.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3ihiidawl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3casygyee.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3cmoxqcpe.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3qimbbsjc.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3ekpkvgpn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3mavefnvc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3hrhcncuy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3lxeemoky.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3rdlnsqfw.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3bnpirbci.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3zdqukupa.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3jjgvphhq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3doxxuayq.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lrxxsdql.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3vzpymvae.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3lyhboolb.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ovhvkwxh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3kjixbrzy.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3dncbjhqf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3nmaxfdjr.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3axtlowlw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3tiwvdueh.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3mejhhnrb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3iajncifv.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3eapvmnti.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3mcyvblpz.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3znpkpzhv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3hkqydbib.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3ypretglm.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3vowqziwi.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ktmxghor.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3deidduho.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3crbmpcbe.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3zqurbkig.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yxzhmksr.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3izxfujxl.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3lgstxrdf.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3qnfonbha.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3okxiqfsm.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3hzongflv.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3psgrvdaa.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3zwbywlqq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3dbinuxtl.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3vqhsvagh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3dbraklrd.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3hibgrjva.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3myuvqkvy.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3ztyaxgih.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hmyhejgs.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3vuyvbwke.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3trhulyfn.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3vgsemhqs.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3hpjyporw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pmjucxoq.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3tyrxjpoy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3aqaaagba.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3dpccfpeq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3dypfjsdf.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3tjvdurcx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3kxmgwmxp.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3spcdjptc.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3nqwxuwuh.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3bmikqrdy.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3bnszpwfg.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3gbhjfhql.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3wnnjvych.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3kigfjfqh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3zsfctvno.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3uzsexfng.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3jznlqbzp.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3gapanoih.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3pfmrwkaj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3lglcokmo.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3zvfjotgx.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3mnwlfabk.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3dikwnrzi.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3khptpobz.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3xjvvmqoj.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uwqaalft.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3gozdpmwa.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3tbxnkboo.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3igmwebzc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3sawewtyd.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3unkuuecj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xcuxizpr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3lxajeqog.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3zwnyhcoj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3asjenkdk.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3zmngvgdk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3zhovhgwk.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3rmzofidc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3lmmapswt.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3dsstyzdw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3fuenbeic.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3bohzwloe.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xkcevovn.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3omczfjzx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gpgzgfna.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3jgmledxx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gtinyrtj.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3wwypsgta.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3teyjuhpm.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3okndkdnv.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wwfdfkxy.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3fhpeqoes.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3iljzupbm.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3dnmipzgo.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3ygrqzgvk.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3zrmxfxoq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3fjbohszt.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3lzqqsvgp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3gkczlpsm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wixruwmw.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3itvdrzms.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3anzxkklu.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3xikvgvhz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3gyciznxu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3auvomvgn.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3urmuzxbf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pnmcdtka.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3ychunlqc.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3rmoemayr.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3qbqzotjw.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3midtpxnb.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3dhczxppl.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3wnwhfoos.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3vpmgzufa.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3mipwgtnw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3idszgchj.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3dzghjhuy.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3fpulviat.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3pzdzbruc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3tofcwawj.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3jzjrvznc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3xewmoczb.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3mugnzyeu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3mfruowkh.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3gpqkylie.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3eugpfisa.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3whbbpvmf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3lajhnifl.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3rdmllhaq.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3bzaoptut.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3tljjhfmf.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3zadhnjqd.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3triolkqa.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3qbsdgyzf.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3pvxbjagi.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3tdugttbq.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3wwxkgfnv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nebswwju.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3ounhvsdo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fooihrfz.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3hwrffaky.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rwdlrmwr.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3gtcvtzwp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3vjjhfhkf.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3fbzicmgt.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3yvgpheka.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3dgywleem.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3ovkgmgwm.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3rwjgglmd.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3zcedwnrb.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3atxcrxoc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3gkftmisr.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3gxrmvdkf.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3goxhsgur.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3moeheqhd.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3ztbbwmay.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ntfzdhkd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3cbyfmnvk.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3nozvzeoq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3mjfclyou.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3ecadtmel.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3dndoprpf.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3zbjqkerc.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3dunfjbuu.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3nzcmwuue.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3sslireyt.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3bmysgohh.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3izrevkhr.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3rtdvwxwq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3ogxjujbz.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3zbyfwimm.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3gcqcsfdx.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3susfomyu.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iknglozf.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3orxclvgn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3qdoeyute.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3wogqmlok.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3summmvkv.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3ppjcgqym.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3hhyrmpcc.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3hisyjnri.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3cmwraoff.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3xoadivyu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3ihbgzzbn.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3huxrkcxf.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3wixlmbdn.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3oguqlvqy.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3yzfetqrs.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3iizgoqak.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3taxwjbhh.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3cyyyscwz.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3suiwifzj.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3jkqdlcao.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ngtvxxba.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3jprrwkxv.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mvkehyva.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3mvjonfej.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3wieqeqty.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3tzevuamr.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3dwhxvews.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3qdyfcmmm.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3bxefldhi.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3oqojginr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3ipzgbtuv.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3syjvcxvj.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3reftpixa.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3wjspisfm.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rbrdauxe.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3mngumwlo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3khxrfkka.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3oxzakcms.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3nleaxdep.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3wilcnsqz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3jeitllzo.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3azznjigw.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3prlgecok.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3jwaygsqm.html


<!-- 参考信息 -->