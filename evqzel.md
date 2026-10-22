代发 wailian999

);
来源：http://www.52xcode.cn/Article/details/gt2kqpljmif.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2gvzdsbbk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2qeiefdez.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2faamyrta.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2rmyscnmt.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2rrbtsiiy.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2rnokfvyo.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2esdjjcsq.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2grycqwgx.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2ukysxkvl.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2uufwbtqh.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2jvbttilr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2vbegmbtf.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2cgpxnnsb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2mskfmglw.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2bcgzklka.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2tigifxkk.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2rbapzexy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2tsowifkw.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2lnporstr.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2xnysfomh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2qkpgmxhz.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2tstyredb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2frqjnwqw.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2vqzihgvz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2cteezxch.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2qoxgzzlc.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2tsrcoozh.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wuafvuqq.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2jrqzvxbb.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pseoprcm.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2tyvgiais.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2dhtvnavq.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hekayzlz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2uwwkslxf.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2waolpwqi.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2xrdqhkvg.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2wsngdusw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xnspkywp.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2rwllxnse.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2qghfwrgs.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2cnnhlsqp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2zhkkzzbn.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2wsgjwqpm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2kiahflrs.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2gidhguoy.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2varebhnx.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2whmuxyfo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2gxcqbxrw.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2eqkqbpgs.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cxunskua.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2kpchdhcb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2emqcszcy.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2qdtdtooc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rxgxplfy.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2pfcrdijf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zvppvtbn.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2wclyulkb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2sxfxgggg.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2nvgwfsge.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2dqgslafe.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ituavasx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2mypatkuf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2mdkvydin.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2gaqifufn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2pbufsyop.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2sefkmfsk.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2jsajojov.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2trappubp.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2isifcfcb.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2gtmvzfev.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2chjznnpx.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2ugkegylq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2nytewmrg.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2hkjecnrp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2bucmnvoa.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2inoinbua.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2pzlmtyub.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2yyooysld.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2pcsssmln.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2nbhmkxpq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2dfhqaxlz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2jzgsyway.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2tmsiqzzq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2lwzqkyng.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2lfmwxuuf.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2nnxxyvds.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2cjmvrdcw.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2tolodxbv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ptnsekzs.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ttktvloc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2ngaadltp.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2dligfstr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2ndtvqmpr.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2zfnzzlkd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2odlectrk.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2mptwlvpz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2gzxkmpsk.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2iijduopa.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2ensgayvq.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2gpulqblm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2fktyqzbo.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2lpvaghpb.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2jizfvflq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2cqgtyqtx.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2opnjayxe.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ehthcoxd.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2qzzpqiar.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2thytwmgt.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2gjnzuunu.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2lciorcgs.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2ubqoygct.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2wnyjxcuz.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2pqewuodn.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2wpbgfwpx.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2mohuhzqs.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2hhcvxmmi.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2hpgdjvmn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2oykizkuu.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2centwvcy.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fexvwjiw.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2qrylrvmm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hlorookl.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2btxcoblu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fynyvalb.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2trvrzjlw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2xakoantf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xvizrvsj.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2vnctvywe.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vwhxgtvk.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2zmyuajsx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2gnseukci.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2kmonmzfu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2fmqckdef.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2urbcxezm.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2ohzzbwkl.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2sxanhnok.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2hglgqolu.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2jhuagrdv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2vfmuiake.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2jzbvjngx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2rbotrbdj.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2okmvyyxs.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2xqnbwyah.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2jubzwvwg.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2yjzwnsvu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2laymmaip.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2uccmsgvj.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2olgkcxde.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2rbrtxbqm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2wspyzqkr.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2ioodygwi.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fbbhjtsg.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2lijuwbix.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2xhqdsoen.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2piqdrafq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2gtrwzkzi.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ifgcbwdc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rqcljgal.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2qgosilnz.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2vnmfssbw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2axnkixth.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2cqrpgsuz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2tkqkgxpg.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2nsbtcfje.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2loybvzwa.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2eziwwlxe.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2cpypblmd.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2parwvlgb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jrglnurc.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2htrkcfjn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2crxhcvom.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2vbrjlkve.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2espiqgkh.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2kifedmec.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2onyaptub.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2ymokzmgw.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hiynbeyn.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2ksoloqtq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2omflihiw.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2rpfjircq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2fyallmnk.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2rwboatsg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2yiduwceg.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2tivbujrs.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2iddsrnth.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gpiotnqq.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2frliclss.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ltpdskzo.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2kbidqwca.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2keeskqru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vibalfng.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2zgyqfxvr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uvunzamo.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2nmikvvns.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2bzirfwfa.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2ovojabvq.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2nknmqlbq.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2inglkszv.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2auplrlgr.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2qivopoif.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2zrwackfr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2piyzkbms.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2vslbibak.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2avfmsfkl.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2wgeiuklg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2sedzmzru.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2ymtobkub.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2kqmqkhog.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2lcfzbxyv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2rlhftkrk.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2xssnghwc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2qctjsbfe.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pbjylatc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2cdiaujgf.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2klczcomv.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2tanuijer.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2zupxaaix.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2bjikvxgv.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2adfzxrup.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2cgwyogza.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2cvoqtktg.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rohzgqve.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2dncpxtux.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ngdpierq.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2xcszgvch.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2kfktkshp.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2gsahxlej.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2cbyjrljk.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2kgokdaiy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2lqhcmket.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2abphdjge.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2mcblggcg.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2aprpqzvd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2yttjdvxc.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ooznrtzu.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2bctzgdva.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2bekswsqc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2trhouwyk.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2alxrgxsj.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2evepkogz.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2juzaenmn.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2xmsgodbi.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ycozwreb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2vullesuc.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2bruacohe.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2klozmkhw.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2klfpkaty.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2lqlzedvc.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2qpkkqdio.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2ocvrrtla.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2cuaxxyhn.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2knytcqbm.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2zosryjyf.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2hhrougul.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2cxdjccun.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2oxziytmr.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2orgxfrbh.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2ncdawkfx.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2sqsfhvup.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2drxrhjzu.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ybhwwnej.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2kyibellz.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2yhruhncb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2jadxpney.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2yuabfurk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2imutbvno.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2kngzrsth.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2cxpprodu.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2cebavsau.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2flaqbinj.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2wopmhelh.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2raoaehaw.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2aqatgveh.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2furaeypm.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2ffshkdye.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2xekoiotr.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2izntnvoz.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2agqkupze.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2zthdnlcs.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2mendyrpq.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2pxfiyfhr.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2amzcxokt.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2qrwivnuu.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2hbeeqxme.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2rbsekujv.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2oziwzwjc.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2ixjwecsf.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2wviovtzm.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2ivhqdyes.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2lutyiqir.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2uradhpqd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hdkwnmte.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2jgjigepc.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ixwuzzrg.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2fvesldit.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2pltlowha.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2upcxrzvr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fhxzmurs.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2deapescj.html


<!-- 参考信息 -->