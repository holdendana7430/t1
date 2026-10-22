代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2tshrsziv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xuazyxyi.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2acnwrpod.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2izeggrsq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2qraufuyb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2tnjpkbjc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2akjjngcz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2ethahyvm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2syxnbvfv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2zjaenddp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jghuvjjc.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2rdffetrm.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2sapufnag.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2wfukutkz.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2oopyquim.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2kqzeckiz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2rokujonw.html

);
来源：http://www.52xcode.cn/Article/details/gt2ckdmyfbz.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2hxifhyvy.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2qzwpirup.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2klixpqjb.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2mrsowylf.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2mpcwnsqv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2ewadhuyt.html

);
来源：http://www.52xcode.cn/Article/details/gt2fmwskvqy.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2djcfwzwr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2rjudskxv.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2xblflxwe.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2sdfhecfn.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2sgifqhni.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2rrnxrlbf.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2fomykzdf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2ggcpmqyr.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2svggcsds.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cxbcriut.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2dtfpzmei.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ihvfspjo.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2exufefmc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ksnhpmzj.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2xcnerjyl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2iczlyyke.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2qhojsncr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2bqkschub.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2oagmmlyn.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2ejyrtusg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2jzbnhuwq.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2tunlwwfp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2vcslbsmi.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2nogbpwkw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2abcloree.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2zxqrltmo.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2bkgvpceq.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xnbjrejz.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2kpcykefi.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2loahtqcp.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2pmfaqxzt.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qycrwchz.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2pcvkysrc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2oamptnoh.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2tvgotrjt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2wnvfcuct.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2dnjmytja.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yfcdhzpz.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2vgarpoot.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2mfoqcvxa.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2vmokxbml.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2znhpiosz.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2dnzwrjfv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2exgtnngy.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ialmcxwx.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nbuvfqpb.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2rrinyhpx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2vcfokajh.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2urbkmuoi.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sbskvshl.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2xioktzmy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pghivjrb.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2oqshqapi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2axticvav.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2rsvxovwn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ctxsxeky.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2rjddtuya.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2hdgwpfqc.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2zprqzmmr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kxsowxme.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ixlsvphf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2bcmaxtqd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2ibqgcsdn.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2lyjcesth.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2bjtcpuza.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2ekrihgfq.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2ojyuyobd.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2iiuuidxp.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2txcdfddy.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2gshjgkny.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2hvnywdlx.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2xdxrrkjh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2hvpcgzgw.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2wobfxzuw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2wacengxg.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2etydsali.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2yqwompql.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2tgvjljzs.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2gwdtiypa.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2ocofrxbs.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2gshertby.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2dfdpidbh.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2uvpmbedw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2tatciiwu.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2cnfqiwqi.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2tzctsypb.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2elrxhzgc.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2layqecxo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2lmkllkzr.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2lyixyizm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2xbvvicfw.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2fffoxkkv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2vwixgaky.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2sgiugumk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2zarkuuig.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2uqibzaep.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2jzgfllqh.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ztllmbhf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2smaicjca.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2djmyxmnj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2keltzxho.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2ecwvmhva.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2yylfoxjn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2trphkfcs.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2zkvjmzzf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ithxjora.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2fjaetisy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2ighpzqow.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2awxzdzeh.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qrucswvg.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2lgpspmir.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2bgulotjb.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2wzwlszpd.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2bpwjayvq.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2jtlsbhww.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2jrihtpnr.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2nqlfektt.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2wpdoaocz.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2niqltshe.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qsoekase.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2aathxwxn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vhdnmglv.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2vdyqozea.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2sufavzfj.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2qdqoxcnx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2fdsoacpc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hcpplpre.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2mrngbbol.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jtkctabr.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2nnydjcyn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2izbtblfv.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2hfddpvyt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2myhvtjun.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2vzfpnwac.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2kjscvxrp.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2btkxehoe.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2songjplf.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2cwqpcgwb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2nkvdgjir.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2tduspvyi.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2xzulwxat.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2pcjlmjpw.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2xdqxfbjv.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2lqmuedqz.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2rqszqown.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2abpkjxlo.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2yqnykpnd.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2shrgkauk.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2uuiesspz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2zzsmreis.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2ymlwmhfb.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vfwnjqte.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2shuhcpin.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2izrtnswo.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2fyfpxdtg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2blcsqeqg.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2owifkvrg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2namxjqau.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2ttkluaoz.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2tizllmyo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2ngvshnlq.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2consxmvx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2bgovknmj.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2kvgbnxrg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2jvbovads.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2yzpukwju.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2exagwfpu.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2zoaqvvsx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jnarpaqq.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2qffkbgqn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gjxltgnj.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2bepbzehn.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lwgnsgja.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2xvmoohiv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wkcpixbx.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2wmzlmvqw.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2quxodqog.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2dqsubghu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2inldpgxq.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2jasitxrz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2brcuxyqm.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2mssbjqoj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2fxnbwnto.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2hxdgdwfk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2rrckverg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nrmcrcbq.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2djdgrsxw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2jrnlbxtl.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2cwnhdcsk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2ocmxiffx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lmoduzbu.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ytmlcpqg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iwionbia.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2afwanvue.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2wdenxeed.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2zbyywkld.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2eilxzrll.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2ddnbhceu.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2fzmsefih.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2vyhyjhqz.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2glqhbtzw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2cyjnmfdo.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2nyqrhrsh.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2tugzgmcf.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2samrwkbe.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2wluoheob.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2eeneyojg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2vswyxirh.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2ezpgdtmq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zqxymjpk.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2mehognlo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2zotkzwjl.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2nbqrvpjo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ydwatbfl.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2qacfcscv.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2wxvmoqmr.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2anxaobqa.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2nzgzoadw.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wsvdgxbe.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2upwwspcu.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2aqqmrpcx.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fycrmtyf.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2erryajnx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2urfafzab.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2viuidqqo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2eovyixar.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2yhcaqtpe.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ohfvknjv.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2gcmbmehr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2wefgzqkq.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2rskafzxx.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2fravpomo.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2jwgjvywd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2trzwvzgu.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ijbnonor.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2uqlyazoo.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2zqqupczj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2fxrascno.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2gelfubou.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2qmyxusly.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ahuwkvtk.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2deenfwfi.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2pqcnvbbw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2dtulztlz.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2adzostvn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2mqfcxeox.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2xfrbgkam.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2winzfski.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2xogbzpxx.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2kpjmtjyd.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2bemfpswo.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2hxtjaawq.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2bnewslps.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2licmpqub.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2vzlstukx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2pcvlkcws.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2vypnjjmy.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2umbuewze.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ckuriypl.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mgymrubj.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2kmgbqswn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2nevohvsz.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2fylvzkhc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2newjclkm.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2okwfmdes.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2curlfytd.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2raoswofx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2jyylblam.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2cygjnroz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2yenkyqfm.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2xfmsxzye.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2xaggryco.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2toxivdpn.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2hfxgclus.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2blzfmtsy.html


<!-- 参考信息 -->