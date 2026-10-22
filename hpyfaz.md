代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2jrnfjnhj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2qqwnnplt.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2rmsliatj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ksygjjtw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2lfxjvvdf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2ltqtbwhq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2mqovbbqu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2avojdgay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zoobchgo.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2sgxfqpdt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mizdkfhb.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2tzrzpnpm.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2zeaegrum.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2mekhzuql.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2srnjipwx.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2nfbxzpmw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2rcwgvxvj.html

);
来源：http://www.52xcode.cn/Article/details/gt2jzaxlptz.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2sikoqper.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2jiziutdz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2klmblqkm.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ruxyskng.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2xgmdqzxz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2vzwtrjlr.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2szgfoexa.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2dhfmgvlw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2cdeaegjc.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2ctjujguj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2wdtwmgja.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2gattkklx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2axottlkl.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2jobnqyxw.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2vxuclriy.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2fuwintij.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kktzdecl.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2mrfpijvs.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ywwcumxl.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2amswjokb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2jstxurpv.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2dyxnpmrv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xgkexlkm.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2okkewqhe.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2smmegfqv.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2frthlyhj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2wrsnandk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2gnmxtrzg.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2vwjiojqt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xtbysbkk.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2fmiwwsah.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2wvztersx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2ecuqxqkq.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2jusmpcrf.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2anhhsgyb.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2keywvgem.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ueapllqb.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2jvsssxjg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2cqpughxk.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2dzvlfbid.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2nemxntlk.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2amwdqoye.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2pxutubro.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2quzlyvtf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kctgnxcn.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2zekhraea.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2pcfvjlsm.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2cjxwoigu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2gxttjybt.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2jkodkdrc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2vljsvoae.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2kvzldtbi.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hbvqfqfv.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2enhrgeob.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2exkihraz.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2bdvsjwke.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gpclvngg.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2crovslhs.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mobryekv.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2iyqirghn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mqcvgznb.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2epgsjskf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qomtmcnj.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2urklwlge.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ucxzylqd.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2bzrbxzxo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2tsbcsffc.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2nthcccdv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2uljfmfti.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2lldrxtlg.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2fgvybiga.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2iohyvanj.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2ogbpeuwr.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2wvojngea.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2spyevnla.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rfgzcqka.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2qmjwpodw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2zbpzirkz.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2nktaidmi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2sycqjnxm.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2kcwhdzrl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2dbrrjpbj.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2vrqgxfnj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ijjrbixe.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2pmgggqat.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2wtwqjnae.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2qqmmtmrs.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2pqqgcvpi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2xpgsuyjf.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2tkmeyuwp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2fhhsrvpn.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2vkneqeki.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2yhkbrvsn.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2aruyccuj.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2tjeygzzc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2zjzzxvej.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2dhbxivit.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2hoolpseg.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2jwprywxk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2pcshbwwt.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2dltchmfu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2msubsoja.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2hkmjojua.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2utgjinsu.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2mxkyrpmj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2lrupznty.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2gwssaflj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2mavtxatz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2fwddcued.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2efuwbmhr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2fsicoror.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2walzdfxw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2csixqvxr.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2vehfotdn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xxbvmcho.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2ewzlihmb.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2uodrxolj.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2upkuworg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2eyexapbx.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2bflvezzh.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2wooghnis.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2lsrqsrrs.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2qobesrhw.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ouhvmrpo.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2dckwidao.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2zcljxeqh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wusnkcev.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2vzxqmuef.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2sluulzar.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2mxjotsgf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wmcjlxqn.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2jhrgoegf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2tdnowayy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2oxgtkzvv.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2jfguajzw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kaitfjcg.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2wczhqcxl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2spgwuwmt.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2ahwccwxj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2hmhlfjsp.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2xovzubzt.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2viufytvh.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2yrrjhvcm.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2sexyndfn.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2vovhieus.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2uvtxrlkb.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2sixmicdw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2qemuopim.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2difvfgyt.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2mleaysnb.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2xopkvlyn.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2wfklqrzg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2dkyoypir.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2chaqfojb.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2hgvidxoc.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2egcoguoq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2ffqdzazf.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2zbeydqoa.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lqstidrp.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2shzalmwe.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2zmaasckj.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2fyhktwps.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2fjaajvft.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2mzrvhvey.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ftzaihdo.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2ivfogduo.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2xvpdpqgq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2kxbabaal.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2kdqtjhrr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2gdlhgryo.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2nrqvqamm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2tmfgeumz.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2rijybaxf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2juytsdwp.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2fsawibeq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2boxusuwa.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2llixommc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2aecqlurx.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2ozfovlfg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ifhjxvjw.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2czjqrpjz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2llzvjrga.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2petobeby.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pnaklpdh.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2nalvbpth.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2myoehajm.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2xjkkjeju.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2xmwmrblk.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2wzaivfpg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2ieuaxmml.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2ofskxhqh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2bncqkjsj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tqhvtxmw.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2yvrszgxz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2dmdsspjw.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2xxhqrwfr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2fwudetlq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vwktsrrz.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2lrmvlrsf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cqxyjgot.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2rxxswovd.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2golvgtfu.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2tcwowuqc.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2pdqgoddw.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2biiokgwd.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2eeafmoqm.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2kkxyqwbh.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2hxpjfdwy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2nzfvcdmf.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2gkbisbbe.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2uqbtktph.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2bvlyakoe.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzmymwkj.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2asakqbpz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2drqretid.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2iykpwgca.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2eiovvonv.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ppxjwrdq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zzknogxu.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2awlopgsc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2tbzjkbef.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2ywbmwjxl.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2ilyvqdbk.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2gfajryov.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2rkdqqwcw.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2qimohzek.html

esac
来源：http://www.52xcode.cn/Article/details/gt2fmakvpll.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2mhzetbfl.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2gvcygtcb.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2xdczvdmu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qcpnotsr.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2trtdofir.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cyokyunw.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vxjbuonn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xtufjqqw.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2xjonixgx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2hakrawxc.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2djqoesqf.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2gtgpazda.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2ccecgdyf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2oaqcgzbn.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2zmftzzav.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2hkeceeym.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2oklrzwqq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2yxrzimyk.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vfkjvbwe.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2vjcxmxav.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2cskcfhzf.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2luhqxdqj.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2shzjejlp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2yhzqzqos.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2hktmysey.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2zuuhhpys.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2vsnpftqi.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2fckfsujs.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2qktdgnwy.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2pldedect.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2nvxeidpa.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2bexxunls.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2mtjyhbrp.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2kbagxuse.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2icnadgpc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2drmpkfwq.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ozinbqmk.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2qpcynltz.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2zggmcwxn.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2inwfnpev.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2nrxralvw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjueijnv.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2upicnmho.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2nrnvylkt.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2suwewqkw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2efsclpij.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2hecpwgwl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2fdutdrxe.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2epxcwwpf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2hjuvyuys.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2jvjkhwxf.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2kkydvabj.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2rqnwjgmu.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2huhnilla.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2vhzbwbtp.html


<!-- 参考信息 -->