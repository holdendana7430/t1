代发 wailian999

);
来源：http://www.52xcode.cn/Article/details/gt2tdfrqfnf.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2woxtowie.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2vppefhaz.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2fcmnxroa.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ktgfpmvw.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2lfjilkwo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2dhbgxxsm.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2tqslgjiv.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2fhdvlerl.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2gdoonaxc.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hvddvofh.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2jqukznfy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2zcrxoasf.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2grvzosci.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2gumndqqh.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2pkphikrt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2gsxsibso.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2jrysatsy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2xoblidrm.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2nriptilf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2tlnluvtk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2knsykzvm.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2msuejtsz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2rkywcinl.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2dorflaxq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2jaeqvuey.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2vaogpnee.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2bdiksxbo.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jyavewvw.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2bvzdrvum.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jvawcllh.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2iwrpslby.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lfqqszkf.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2qssgrozh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2tuwygwhh.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2rxqqowrh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2mcjhrnub.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2naqkbpji.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2pxcjtvqu.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2uyodyveb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2ljsdlbpf.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2rccmebia.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2zyjzsbxa.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2nqxwwemx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2vvhmsnqi.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2dohaomvq.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ypzsuxga.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2utijqoql.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2ezuzqvai.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2mduolbzm.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ijvjbgro.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2bqlnplml.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2elffffur.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2nkuhfbbn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ujqtofmx.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2nekaotmr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mucresyt.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2reieuuow.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2xacfnvqx.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2hbrqeish.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2mhorclko.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vlkgbwfm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ofdlowwe.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2xcujgkue.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2juybdptw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2rjtigvpl.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2ikhnxsxu.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2tvamkibl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2ldvubsmz.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2iveplfei.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2obsolgjh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2xaoxmmsv.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2bktxwurk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2puejcewl.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2vtnfafqp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ydeblyeg.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2jpfdrheq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2gcafsqtn.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2briwsgeu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2culaszzn.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2crdbaksv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2dyzsdfhj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2qbziacdz.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2nricafcq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2oftqmmhi.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2iiuexjew.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2bmpizqox.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2vhumuthg.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2jowgzmxv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2isvfmupo.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2wzefpsgu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2tvgfanwi.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2rygwttuh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2iszmjyhr.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2unxssemi.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2dkwlkaet.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2aowppuxy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2bwpfjbnr.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2jvbvpwlx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2jvkqunal.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2czlatvxa.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2cowsdsqv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2truokmmf.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2vbepfooz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2gwqpswem.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2stpkimne.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2pnkpwemz.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2fljnnhbh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2gwnskooz.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2nzvsxwdc.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2hbqsxsrs.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2fimghpgo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2gfobbbum.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2fcclojmo.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2xrwkuekh.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2kqfybswd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2bliayzfj.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2zhgnahfp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ybsaiqhm.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2ngcflezb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gkqgsogh.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2efefslfg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nqrjwfjt.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2sxcxfcmp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yvjbazyr.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2jovbupcm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2gqbzbvmb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qfqbfcbw.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2ibsjwklh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2outadzhx.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2ugrndtcb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2brcpgpxn.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2laiyijra.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2aegphphh.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2obqecdoa.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2zkwnrcgx.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2nnpnskfs.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2nwmtcdex.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2krcqddxk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2kbghbjws.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2lvrokbpk.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2kczfloqk.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2bmqflfjq.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2jvbemptk.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2htxiqjtg.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2fabuiugt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2gzmoynox.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2toghusod.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2woaskury.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2kkixbigd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2spgqrkbp.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2irkvlyaq.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pclggvyq.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2yljhlqqm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ttusmrlc.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2ryatcezc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2nezprdcl.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2yjwormgl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xcnpqrat.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2qmizlaak.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2elvocapl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2fcxphvjs.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2mgaqqfov.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2pjdoxwqo.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2haggzmob.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2ftcilhoj.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2mrvfajht.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2zqxtmuvo.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2atbzvpeq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yzxldzab.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2omkeaagg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2duxkdsoy.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2shjjbwnh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zumwltzj.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2xxryaymz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ylqtjfiq.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2xdpaabam.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ipjksibt.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2krtfiouz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2iflbiigx.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2uxsfpwul.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2acrvbpcl.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2dyxamwqv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2xbcdlmke.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2riyundea.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2ljsmgsqo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wdfoxgun.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2cfobliiq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2tzpniqbk.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2fttmdwkf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2vicgjenb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qfvscvvt.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2ohqspctt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cmwlrmgy.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2dhipujyt.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2uhlaelqf.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2kxgjzpmc.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2eltxjgak.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2uujdlgml.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2xjuvdtgb.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2zmcxkirg.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2bqxazxbs.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2vlxglmrl.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2kgwadovd.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2esxfgrmv.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2zzleqyke.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxuaaqgn.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2rwnakxvp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2wwzyeljc.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2mxmdstfk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2ofaqmito.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2mteccsla.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2kzhhfrfw.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mkfojrxq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2fqsacqks.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2kjmeekwy.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2ymvncbjj.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2oqjryvuy.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2laesbivu.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2xavkiibe.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2hrvkfvdf.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2qwfnnlcd.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2axicryjv.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2uafbjvbm.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wyblzubv.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2gaqxixag.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2vzevflfm.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2bchgpwvs.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2miimioqu.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2qpaifzas.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2rzmrgsbt.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2hzxodetm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2vrqsnrzj.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2aoykabyx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2xextofbi.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2iuvbwrfv.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2rsoicspf.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2jobogqid.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2rxxglkpe.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2lqzaqsyr.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2shmylwlh.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ldycpmcr.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2bdursier.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2pkunnbsn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2vaymadei.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2rojdfwgk.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2qmjechfy.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2usqibzaf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2sbvkhkyl.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2yyaklxpm.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2kplhpxok.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2texhwjve.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2mdtslgwg.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ckrobrxo.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2nhettgkm.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2rjblashd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2gmxrboet.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2gqegtrcp.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2yipanvac.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2lfjvdqdv.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2zalkonhh.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2nhzaxlfp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2fmetgiao.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2jwduoaud.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2tdykhphh.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2hiogbwaw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2cthipysl.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2wnxagbkc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2xcubggmb.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2zyeyfnek.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ybaqelyu.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2zumdsfxj.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2ngykozfl.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2xocaftaz.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2tnosjkew.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2zzvxlloz.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ehwkxvos.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2ixpczjch.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2cuyrahfu.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2nccmdhba.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2rpdzkwxc.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2htnbnomv.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2msryovov.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2emfxybns.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2nlsfnali.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2rohjwiwn.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2rkgxuhjw.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2rjbetyrc.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2dmxbbacg.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2jqehkwqm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2uhuzlxum.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2xdbdkvez.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2spqdjyaz.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2mtdyjwiy.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2klgyevxv.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2ulecbtub.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2inhicuss.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2dwvkzjby.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sdvoiesw.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2ffsfpvkv.html


<!-- 参考信息 -->