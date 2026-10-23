代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3kptrflwk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3wipnpfsl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3asewxukc.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3qhuopehz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3ikzgckni.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yvdvxakw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3zqnoxenr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rzxwchwr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3zfvbuvso.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3genihvol.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3pbgaeldn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3ilrxrear.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3frzrmbwd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3jhbdenau.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sranasrq.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3sslmclav.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3igkpiruu.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3uvxbkooe.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3mlprebwn.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3vkipvtju.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3nlyqccnf.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3uiwpequl.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3ihzdxhtx.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3yrpgrmqx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3cfunbiri.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3twwwbfgh.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3yvawqwzo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3joggicks.html

);
来源：http://www.52xcode.cn/Article/details/gt3aunqtfkh.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3kezspaup.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3vvfteixg.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3aseczmng.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3gtzrigox.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3ofoxlcpe.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3pzhgynsj.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3kaiwnbxa.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3lqmcmwzi.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3xiltzqhg.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3hasphywy.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3pvlrfqot.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3kiqdjadk.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3eamlqsuw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3eneoztpo.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3wiudqgrt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3eqzbxyzs.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3sxvcbrqj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3gdpclthx.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3zcctoqqb.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3mqwwesif.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3ijnwvqbw.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3zuhtynpe.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3tnsvwyuw.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3bnsesmmy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3yobgjojh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3xmwgywgj.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3vthcdnil.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3btgvcqsk.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3fpwtwmve.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pjygwbuw.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3aebclaxz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ehsqfjqz.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3zihgmrco.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3xxbyulpv.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3ngxtelvu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3fjczyhvm.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3cwjshyuk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3kajnxoth.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3odlsnjoz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3xmmxrrnd.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3wbboycmn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3vbamvukw.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3cwiffqfl.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3yftptzvq.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3fsbcsisn.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nmiqsifx.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3euwofprh.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3pzlgoxdg.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3cvqjaoxn.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cbhcsmsa.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3oodwfzra.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wbaynqdf.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3ktbdsoli.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wmreczzd.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3kjsqnumv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vbctdxuf.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3vkpxyhvp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3sitkhmer.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3zbbwnjlo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ujyeuzfo.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3pjfsehio.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3upizhhqm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3chhfljst.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3uwzqrhly.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3wrkgixbg.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3omdbngzg.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3blkkubpn.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3kjleznqe.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3jrzeiuar.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3gghjhwir.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3maekwgfw.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3wpweytue.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3rydynoei.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3bvnxngfa.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3zbmtqwsu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3qfmggikg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3dhfgambp.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3nckjeacn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3sdhgjmwo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3emybvtpa.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3rdjyzmhq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3pwlwnubs.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3egasyvwa.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3przzfneo.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3czzffdpe.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3gvvzoyxw.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3fwshtkbx.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3jzepsrso.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3imfzowge.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3yfkqcanv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3sqttoxnw.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3rxwizvxu.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3diimlgqy.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3uygpctvv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3apbmbtxq.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3iusqpxgy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3zzvhhved.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3ipmnnalx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3ixxzpbrm.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mgzekuuh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3rmhaiawa.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3jigcknpu.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3owfsvpcm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3salznxqw.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3yuzkkhbj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3dkkarocm.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3gzecgzqz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yeoijpzq.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3exxqdmte.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3esmmyyxm.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3jdnmxtrs.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3sakwbyfk.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3xyvggbxo.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3pgbcbsal.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3ynmhayti.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3iqqadvea.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3bnmqsrzr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3zbwgcqnn.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3hkgfkbys.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jqavinxj.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3kjmfnzri.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3eudruevv.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3wtsufxoh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pjaxarqm.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3jwzvlkwo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3znhvftzz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ejlsunvl.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3cywcacit.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lklwwxbi.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3xebennpz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3oxksfcne.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3neculqem.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3laytozpt.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3gejltgeh.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3zuyiiamz.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3nfwjscps.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3lnlsgbgo.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3siogdmcw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3amcihhts.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3npetdgre.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3wlbytdmi.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3txodrxhc.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3ewglzoox.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3xggzelik.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3sbvkbpno.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3cwjfnnpc.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3mpahznlp.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3rpqawmcn.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3gifkuios.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3dipxorro.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3mxzvijix.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nerkqeyf.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3rbgcdzgy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3hqhsuqyf.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3vlxpwmyu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3msrkvdux.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3fzwoiufh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rmbpprub.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3xpmgwyca.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3grieerdk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3wocvxxyb.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3iywwfsma.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3eauyzbeg.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3zfjwwugj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3iufbzyji.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3cbyldiru.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3bngslwdn.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3jjakupen.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ggjapvjy.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3foojjlgz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sdrlrybp.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3ifkgdzav.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kasbfnzv.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3iwsswmfx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bndplkyr.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3esedsejh.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rbpclmde.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3wypojvsq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3evarluug.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3ejzxzqvs.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3elfoyxkx.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3xafrymxo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3qorikvpj.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3hpwddtox.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3netcemfi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ltohnfrj.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3mcfoeqhr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3fzfaigtp.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3sgczdgoh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3qnrqdomp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tbxiuowt.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3vgsuarys.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lxfxgybo.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3hsndbkbi.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3xgjomjul.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3jifygjwm.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3ralamhht.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3mgbuvxet.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3bgrryjxd.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3viqdgyet.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3pefkhkcm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3ysxarxat.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3yndllbxz.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3zajxtmyf.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3vzefyltw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3uimiymhu.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3mqnawjlw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3mcsslfsh.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3ixdkjjiy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3mbrxzqgt.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3noqjrhmu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3qchtcfrs.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pzhhfrhg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hngnnnul.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ovrijsac.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3bjrvfanx.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ucqzlmzh.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3vrlgkkdg.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ktpubxiu.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3mvwulvtp.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3oyerzqaq.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3ocfurebn.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3hqaghrls.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hkimztlw.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3pfpejlbv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ifouxqmj.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3aaykhktn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3zqdxxpkh.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3wcpkdwmz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3bfvhllfw.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3wckvgkio.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3awrbkrdt.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3onxtdayl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nytrtavh.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3baibaqnp.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3tkyfflum.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3fvydhijp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3ywpkxxoj.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3zletfvgj.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3ayybqhtv.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3cyhlkcbu.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3dmcfqvgn.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3rkjawuqw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3yimjfmdr.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3jehaxtge.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3zxmdnkwy.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3fjfzsblh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3ggohtwnb.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3thvjnhyp.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3tjjojwio.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3ubvllkbv.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3llncnjgo.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3kfbyzyly.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3mwskcajr.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ibfjvyzb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3iiaqvmez.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3ldipqiuz.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3njqebjsz.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3dbyughoi.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3lgcwuxge.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3vlvlgsgb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3pppdvqva.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3onpuyftp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3eewgajiw.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3gaqmqcaa.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3tffxmfai.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3jclcwlwz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3dgwnybra.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3savddexv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3bmsnbadr.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3sncumdtu.html


<!-- 参考信息 -->