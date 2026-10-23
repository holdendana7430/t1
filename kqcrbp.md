代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3uvillbja.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3zyyfbptl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3rnkvzjgu.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3hifzrobo.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3qvctgckj.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3bpzvdple.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3itwfozto.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3igdpjvjx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3kbdgjfph.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3fsotgttv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3chmedljj.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3nngyqdmy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3zthdvczu.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3idgzjapr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3fplnpigf.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3jrasutge.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3ksvmadrg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3kmmmgxij.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3esvjvoku.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3fztbeyit.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3svxxzrry.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3lofjqhyx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3fevldiha.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3qenaetvv.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qmwaacle.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3enrfbvfe.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rqiodvwh.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3tqiuqlru.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wkfmfcnj.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3drbgtqqw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3afsnwxwz.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3xuiaqezq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3kmqmqzqg.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3vzlrlrcb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3huuubsfg.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3gaidypsf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3tmxozupq.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3fmebzgzg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3ozoghafv.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3mvkzuuvy.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3hhexpfwa.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3ihrtxest.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xefgrlhi.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3kkucqarq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3dwmraxbg.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3rkaaqkgb.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mppoawvm.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3imnihbxb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xmdyimfz.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3uzkexyia.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bkzoqney.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ihhegxms.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3erslbdiw.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3bnvllcrq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3unjrpqxg.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3fbwuzcwu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3byovctbp.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3evsxmzbi.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ybrvovvn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3xdwtdaxa.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3aojnoyiu.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3cihowsrx.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3ljcmmsaq.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3errklros.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3wlwhamfw.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3vazjhust.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3ishtklep.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3fnzrdowf.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3wkejpiuj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3moeaujsr.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3hnfpokew.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3kkhlyfjt.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3bkjscdsa.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3oiogstit.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3qgkyskso.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3ljrzoxnl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3zbrgbnsy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3jctrdtor.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3khbaatdt.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3qeuvffzd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3mekteopr.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3nlobpdfp.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3kgvzmmxo.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3tzewpyxl.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3dsneknru.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3vsigbxwt.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3uqqiegay.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3hpnobvgb.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3rphpugju.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3pycgfftf.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3twmccpvm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3yqjlggxe.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3tmxgybct.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3tmwifgnq.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3wtpdimel.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3mbhfidwf.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rlwtafaz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3zmzyogoc.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3bcjwegkm.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3qcbqpcem.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3pensohlr.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3japkkquu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3fcnqfcut.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3cmwegivn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3dzzxmuaw.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3lathqpyf.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3wbfsvupj.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3ejanuvun.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3fbdriyuv.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3flvcstvs.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3tsegemif.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3jgocscyj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3vilzcsnw.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3gbvrzkqv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3naupdtqp.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3oomrnhji.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3odleqnwg.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3umtfnxyg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kgwiaetf.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3srjryecx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dntigcrm.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3dqgobycv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3zoxikajq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jbdhsqyr.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3ztpciljc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jjdmcagg.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3yvpibfwc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3goqumlkp.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3qvwztorc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3lorktask.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3fkcfblqs.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3ejgrtwqu.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3dzjdjvty.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3njnjudut.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3nkmwoknw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3hghuopyr.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3klwfxlmk.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3zrugbphx.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3movhdesx.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3fntpjkgs.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3kemyxtso.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3jtypknjh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3tspoxhha.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3frnjhzjo.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3xevglevi.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3pigsfmrx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3wpcyutll.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3ltxgkatl.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3goqbakdj.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3gfxjgewn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3riongbqd.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3ofnjzbot.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3skchvsdq.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3dswbpsgt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bjurckfn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3umppcvob.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3tsyrfgbh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3zmckdrci.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3ixombckl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3agfjiieu.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3avikxaqe.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3hjyckahn.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3sqxclwwf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3ouglnnsx.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3yxuoxhzl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ekmijkgp.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3pcdvzakt.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xtcglyyr.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3nrbaceou.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xzqwrwvb.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3kpthioov.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mnfhhuiu.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3lkxomzwg.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ydmtewru.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3xfgxmcoj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3opbljqnr.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3jtdpdbea.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3wkqvdefw.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3hboyqaty.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3oiuymopp.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3rpyxlxfd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3xxxpvtxv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rauxfvrm.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3hnnrlzel.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3mmzxwsqc.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3cqofhnee.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3owxbxrvx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3skgjpwsu.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3cxoghkmq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cmqfvidk.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3cuytmitl.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3pjtpnnke.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3cmwehege.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3ickogvfi.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3xeyiroyw.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3maqdmbmz.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3haofdpox.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3qvqrgbrd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3vksdomma.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3eecekevh.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3hdipvhbd.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3kwwrljjr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ewqpoguv.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3kpnjsysr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3suchhvoe.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3yzwjiflu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3njuitnii.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3rtneaclq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3okihlrkt.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3hgnvjlcs.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3puzxqakn.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3tjholgii.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3zlcuhmsj.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3zoqcwvwc.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3rnpiaftp.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3jrycoody.html

esac
来源：http://www.52xcode.cn/Article/details/gt3fncmbgfq.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3ihgryqfw.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wrhliqqd.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3khffcweg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3xmpeuhyw.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3ogqgoqwg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ubrmmwvl.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3eivkvtpt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3qnogdufp.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3izaywfgg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3qhmtvebv.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3rnysxpce.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3hgagyegl.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3mgetscnt.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3wstxvasq.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3hmooobdl.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3hsnnhxep.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3nmqhxgzk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3kmkccpns.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3wcxzokqa.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3ercqoxvl.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3yvhwqxvm.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3iomhodoq.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3idllsimd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3yjpwxmkt.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3cioekphj.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3holjgsjp.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3wsglhpak.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3bpspbewf.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3lvndtjxq.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3ixqzzast.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3lhmuswel.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3wkmrnlmd.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3dsjxveha.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3kgryasjc.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3gpzzpjfj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3jtouhbrx.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3yppjtxdo.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3odeqcbet.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3vosnaqhs.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3oiavbykk.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3kvabykmy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3bpwjosue.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3tiiqumdx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3rphajayu.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3rgxavaor.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3tgexywqs.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3bwntlezc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3tqlaojgd.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3kgqczlal.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3fmmvqknn.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3ttkkubmb.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3ndrfiemx.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3tjzakmns.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3fgchywqb.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3heywzkii.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3sllieray.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3nnkigovx.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3wgcntwxm.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3dnywpilx.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3wgiwoxxa.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3mglgfttf.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3dypstoiy.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3ewamdage.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3kuocxjyc.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3hlxlmspo.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3dpfgkexh.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3zjwmwfdk.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3huwzyczu.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3bfnbdhdy.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3uwksdamn.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3mquihbym.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zssixppm.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3ysahjgbg.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3capuovny.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3fhqhmlfm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3cgkhjiqm.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3jflnsdbj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3apsuejes.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3utwzbzpj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3ksbuuoks.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3fgttvrzk.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3mlwmdmkm.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3ukawxsjr.html


<!-- 参考信息 -->