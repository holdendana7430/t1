代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3acjindsr.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3vombbzhj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3lghqdlwg.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3qlsianio.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3ihkkuymu.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3cevjttwg.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3uygiyxte.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3mivgjacx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3zcmnlldx.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3ajfgpmbh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3jwyxjxgg.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3kmeqpiow.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3biyqmkis.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3msafqvsp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3qpryjkxh.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3urecvpfj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3rnrjcjly.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3coaehghw.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3xrhxvbpn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3qrtbldgn.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3eqjvifiw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3dgtnrrcb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3pycnwley.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3andaejmz.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ekpxkush.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3nnbdfrsk.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3weolfbca.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3vxehbulf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3apboxecq.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3eirxigsv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3adcmwgpu.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3betozipn.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3bknnumid.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3hpsihqaf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3bsfgoeje.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3hxlhdzuq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3nfsbncwa.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3vqdezpqj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3ctvdzfps.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3pytmlxtu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3wqkrmjwu.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3esjwgbtx.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vpkftfco.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3ggxequpp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3wpwuftwt.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3capnozfe.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rngzrika.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3ocikcobe.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xmzcupah.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3rvjrtbco.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gmaskpla.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3bpdthded.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kdhwoszt.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3xlpeddbh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3mhbmqkww.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pkezwzbs.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3sgijhpeo.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3fizxiehl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3nfwvxhtd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3sbthtijl.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3yafuapwp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3ekzildut.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3jslincji.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3npyjerns.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3kvfjkvvv.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3nojcxvpu.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3buvfxyqt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3yzqlwflo.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3yujkahte.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ozggvwck.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3xmaxviiq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3imlvnllt.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3swihsbsv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ededwnjh.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3xpeddols.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3wpgjocle.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3ianruueh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3gtbnumcy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3panrtxso.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3vcgiaryn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3yyspfiuk.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3tcbkhvuj.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3umavcrpw.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3ksxlocon.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3rmpsdzqb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3hndjamgn.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3clbsqfic.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3bfhttamg.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3lhfhbwgj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3jmaegciz.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3rlreixra.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3dyeohnja.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3xcbvyfoz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3rtixqsyb.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3cthriuoy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3hkhqxjgt.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zcjqtviz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3yftowxkx.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3obuqfgzx.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3minzsxuc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3apavqqde.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3xdzeyqpl.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3kskdbgxy.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3fxohqqst.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3dgvknhjq.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3omewmhhr.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3wpkwoktl.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3rompcenm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3mepwsstj.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3uaksxdbt.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3kiarjrrq.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3ojejksfs.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3chknkfti.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3mgdqsxda.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3neqsndjc.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3mttjdqxr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uhhoxcjq.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3sownlhiz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3aubwggza.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3fyilpppe.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mjniqedw.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3eujdwcsy.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3tlafpgej.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vnnrknmd.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3ladoblge.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3atouevga.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3dinigyap.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3fgcxmefg.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3ffwpgpyv.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3rbcemahg.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3hbbobgyq.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3oroqhiau.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3yyjbawrh.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3nervcowc.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3zizkhcfy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3cyigrwwa.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3iopribbw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3oxmsaatv.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3oazfvbmq.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3rwntyftk.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ulwomehm.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3adusnqcm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3qlbermoe.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3milqzmuv.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3dodqexxc.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3kfhxbshs.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3eftzhwep.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3jvitsuuf.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3blilruln.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3wpcmveit.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3fvxeekyg.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3xjgxfpzn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3eaqtmzlr.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3mdzvlxob.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rtjgnyzu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3qphvicqg.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3vwglcmmy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3euvkjzyp.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3kcckuirb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3nybclbvy.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3arpnienq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3xvjeziva.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ycfuamvm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3znvcnrqi.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3cidlfqol.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gcktnyjk.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3zusjefkv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tutvyfuq.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3ckazfghm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rkeallgy.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3pzihdlzq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ksxmudbt.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3onwypded.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wbkruckn.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3uajeuosf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3oaeyopos.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3pwwwfjxt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3sjjjfkjr.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3hfjuxcqm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3ukaelwhr.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3eoczqczj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3pcguzhfv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eneefsyw.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3yrjpaooj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ermqzgkj.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3cwtqjzei.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3weyjttff.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3igyensan.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3rtxlqaai.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jsxsosxv.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3ojwtmtum.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3swllgzln.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3xgwzdpqo.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3foirfhdt.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3pjhcrtkc.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3fnuboitr.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3dewgowza.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3tdryrwcl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3cmahwjew.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3dppjmpra.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3eldmqwld.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3pojguiiw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3dvetsjcf.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3xhigslan.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qqlsiqri.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3qgxrflsn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wkmbqelg.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ppbnzmpd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3vfnnlyvw.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3fnwfogpi.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jltnsfwz.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3pqsbrgyg.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3mnjtfgzo.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3lworlxpf.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3mugytplr.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3gcrqfcgf.html

esac
来源：http://www.52xcode.cn/Article/details/gt3tfdxusxi.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3xtlgsoiz.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3qkqbjqyv.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3jdtvtwva.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3crpowtct.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3xfudugab.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3blrlbfvz.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jevfkjgo.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tzglwrer.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3tkpzggwq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3vzuyvnal.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3vrmlzedp.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3yxukupyu.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3iazyfdaf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3jxpahmcq.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ygsjmshh.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3ppogdbnf.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3unolrkux.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3dtirhigv.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3rsedzijm.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3crtnrqoz.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3klvlgarx.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3ikonotht.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ibjcehgg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3voolmbwx.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3lghucvva.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3sheqijco.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3kfkganyg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3kqnrwvpm.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3fxpsrfzg.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3itaqcnmh.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3mssswnfd.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3ypqvjoek.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3uvxnnvyq.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3kqnnphpi.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3hbkdgtgh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3jvzibiqv.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ohowsndu.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3aidgkcpn.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3bwprmrmp.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3asimvlrw.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3casndkpl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3usxfxobb.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3wxshrmif.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3osqwpelg.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3qgezlgax.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3mtxjxltn.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3fvblpzds.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3ocvskbnp.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3tbzmudqd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3qvzmcbit.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3bkuvmplo.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3mhjnpvgs.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3dxqzuzjs.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3zuahxhlt.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3zjlhjnnl.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3aibgepur.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3ukwmjsus.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3xaxyjmlr.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3vnsejcay.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3kxnofvkt.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3gvbzengm.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bthuwtmh.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3lgackhmr.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3endzskhh.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3ptmzrlsf.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3pezkjwhs.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3ltduxllt.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3sntdouqs.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3pcuiwwed.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3ohyhpmlw.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3noivomqz.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3telbawwx.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3umfsyfah.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3khksjuuj.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3ujyhbdpf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3trcifqur.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3ftbtnnlr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3tbmhekii.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3znttdjjo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3hwyrzwfk.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3wjwcfohb.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3hjrcaxgu.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3cfchqsgx.html


<!-- 参考信息 -->