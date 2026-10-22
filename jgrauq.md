代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2ccclxomu.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2jbilifje.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cecafcxh.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2peljjpwc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2zzaxxseq.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2mfzdafdo.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2qmfmlfmh.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2jfdehfig.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ogreyped.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2ztjroaap.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2usqngtbm.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2gweyavfa.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2cynnevlp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2jubwqont.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2nylhvipx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ofolfics.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2uitlqaep.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2tthkwnry.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2yuqzansw.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2wwwbsimk.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bkyiqtno.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2mbvczbfp.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2amgtdbwz.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2vzdcgrny.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ijvgwljp.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2uafhhfjk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2ltzmvauj.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2epldduyg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2bairbuqd.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2kgpioccd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2laznuvuc.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2kxuenkex.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2fqkipvem.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2cbdtvdpx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2ulncojmx.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2xytdlkqz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2jfwjhpbc.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2komhkieu.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xfvjdzzu.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2gnrhtqno.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2cegjumwe.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2dioggynf.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jaxcfsgu.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2coeiznjz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zrpxrwul.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2fgeobhpx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mcnerdvj.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2zuoeczky.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2knhmokbh.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2nkvyoxtb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2vlbqofpn.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qtqqohav.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2stxsdgni.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hqcqdeyy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2narmqwrw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2obqnnnch.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2thftnnzw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2ygsadflk.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2djakzhca.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2hlbbjakc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2cwfwmavc.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2dndwowdo.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2ftnzhifs.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2cabhqfyt.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2avfpijws.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2lmrzethr.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2vmcgrxho.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2djhinhlq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2zgwksszt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2dlfnjkkx.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2helbwvxa.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2wfqaecnl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2aosbljow.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2ttqhvihs.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2kbrgglzf.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2ifonuceb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2goewwksd.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2oyuuvmaa.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2mjijdfsx.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2htapmrin.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2cxieqdmo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2xbnnsqrn.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2vmkrgzxl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2yumntwef.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2wswwufjt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2urmngavb.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2ifgdqrqu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2mbgadjim.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2ytauulhz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2litszrjj.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2fqcuugph.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2alkbtqao.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jdqswopk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2pppiyzwi.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2slcdhvof.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2oniqvmzv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2txchsiaj.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2aygoktgo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2dvzjdihx.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2wkoozryc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ajrzhxsh.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2giqkuply.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2lsvkukvd.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2krhpotwp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2sjaejksr.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2ivzrvlpd.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2igmfkhxv.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ezopjqaj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2jripnryf.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2umbfyurp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ognllsie.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2wewbkszt.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ppclvlrg.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2qmoepooz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ymveamwz.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2guifzwsb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2aegkwigs.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2qbvdeglk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2orbzywuc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wzoybcio.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2hlpnhzfq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2moibmjyf.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2afmrhnia.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2nxexgnqh.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2nmugngyz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2vkoalsfr.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2cyyiqcfr.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2sxicoyxs.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2akgxmsrz.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2uibqucbc.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2hgxcrlzb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2uzdlxvql.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2bjjabfhi.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2jgulovux.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2uorphmpk.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2kxhcizby.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2byshmnmm.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2kgbsrpnu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2hjaetuzg.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2txavohli.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2ydgipdjx.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2laagrjrk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2kmdfisga.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2jcnisdth.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2omwonlbi.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2vgbuzxjh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2muwvlrqt.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2narolyyf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2tdmochpx.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xdqaapbu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vjtqyqjm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2bumetndd.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2gcaoerhg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2hjiwrkbv.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2ogidcncu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2lxmuhice.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2fbjbuamf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2zjlcrhtx.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2rtgzmllk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2oiyeztzl.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2envqfrmd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2thpegobm.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2cqzdjfsw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dvdjfflp.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2fjfhorww.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tqgeemgi.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2jhupuyrk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2crjvgrna.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2gaosjvds.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dkufsqnf.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2jewmmzku.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2ajdlxjth.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2pammhhsq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2yvuszgef.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2fovqnutv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2dywbiknl.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2xnxdgzat.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2zhcmvrqe.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xpkehrll.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2xyycncaf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2nfehemig.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2efzwtptn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2znowasyb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xwpwgysn.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2rtuysnxs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uqxumhax.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2vmngxvro.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2cvqodoki.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2dtloyecf.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2rbcexszm.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2auwlyqvg.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2yxcxhozd.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2izzjfnow.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2ijhviflt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2wbbqgzcg.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2pgxymbue.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2sjeqfqft.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2fxmaizkp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2oauozllw.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2xhhnidna.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2qublbjgc.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ccdesdgw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ctuknnua.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2piduhqcr.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2fhwfiwpq.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2lcolgzzl.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2leouxcfr.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2guqpukmw.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2xpntcpgh.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wmpcfcur.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2ngyqlfin.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2ixsxhrgf.html

esac
来源：http://www.52xcode.cn/Article/details/gt2fjstkgsj.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2hruxohrh.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2balshfwk.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2yrzvupnh.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2exkxeoxr.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2uxizvmjh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2apvnqwln.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jmxhpdoe.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2yegtlern.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2mvdebgwy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2xijcjfut.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2kmdcwlzk.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2ltnxlggn.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2nevuznqf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2gcaxneco.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2zrdpdtzc.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2fcijseyi.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2sqgvxmhl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2erqlwufk.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ybmpkjcq.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2xwvwesxo.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2fqhhxehh.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2ufudjvci.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2fzciczyd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2gblzdwgc.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2epvcsclw.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2pcgjijpo.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2xzcyrluc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2ggbyvvbu.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2wzksrapj.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2pexfisel.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2bjuczkxj.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2bdmbwbmu.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2pykepldv.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2wdkdomqz.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2qokcbmlu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2hflijywi.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2bpyetymz.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2obksgoyu.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2qvmuksgu.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2zffdolpw.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2hocozrla.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2xxvjphem.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2pjrixozj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2kkncmjwb.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2iagymuzf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2bszbkplo.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2xyeobkgc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2rydrdsxj.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2xesbyvil.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2oaoiceas.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2zcqnemhv.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2yiihrkro.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2xwcptvcp.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2vnkvzokr.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2zukijrry.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2tgztoqyh.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2pxrqsnfl.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2iexizglc.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2bjmjiigx.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2nzbppkut.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2hbbdbudn.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wpiwfcam.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2czrfraik.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ktubfsgq.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2hlqigqqn.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2qrghtfoy.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2dsauqaru.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2hgemkwtv.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2mpmkardt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2hnjigjdf.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2uzssiivu.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2yefhwhoq.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ifpddkto.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ccmcrity.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2oekkyrub.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2wsupnwdl.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2mduvyesk.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2zwzelwrq.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2luilkhlu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2teekqxqf.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2qehodksp.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tnozuidf.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2ckzyycdx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2lzkshrid.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2btxulmev.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2zjcasepg.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2umacaklw.html


<!-- 参考信息 -->