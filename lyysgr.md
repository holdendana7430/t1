代发 wailian999

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2masvgybr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2qmzusvgc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2yxndjhvq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2awxzanvb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2phstxpzn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2wcgzakpf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2dtlufhju.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2vaqidgel.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2zanmojzj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fkzfsurw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2ntzdnujj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2nswmvvqc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2ywexztpd.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2zstrinfa.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2ytdfyvny.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2zvqcyget.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qmrnjaxu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2jqtcktor.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ycloxdjr.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2gssuuyjc.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2ngekrnrs.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2izbqfkid.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2jcxezcil.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2exkjrwqk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2nhivopih.html

);
来源：http://www.52xcode.cn/Article/details/gt2jzxtfxlf.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2bdztoiee.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2wrngyclp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2bwetpdby.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ktkyuqbx.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2nqvxnnjm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2adwllbom.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2lhbakkat.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2hwjuqxae.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2hpuyfqnx.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2fqhcugyu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ueezvdoy.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2yttmchsi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2ipbktwhe.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2ypqqsmhu.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2vvjeeois.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2xsylewtn.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ludzxcml.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2dbghfihh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2jtwtovoi.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2etzktgib.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2twvvlfbt.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2yrvyvlfm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2wheypowu.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2fslpxcdt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2bsobhuir.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2howkcwlx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2jkhnlrzj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2xsivftrj.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2ehmbqiie.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2fcyommqa.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2apxcdbak.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2dmvmkooi.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2yvtaedck.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2xsqjcsmt.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ovzsbabn.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2mnrdvbnk.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zmjmbrsp.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2uohjwnaw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2wejtlywp.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xpgtvspp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2eigcvjso.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2qbdwicyp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2fiwspaco.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2zxpmmmqf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2prortwrt.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2wypcxejk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2fctawptz.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2lsuihjvc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2zarehejm.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2vmxjyhuq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2gtkbgdbf.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2atdkldbp.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fpvtuvbs.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2zfuuhbee.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2cjjargrz.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2ubgjoyuv.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mtopkmti.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2ysiwezfu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gzhefeqg.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2utnuuwah.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fcxadorg.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2hxcdygtk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hkovqeib.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2dizbvzey.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2cnvgwulx.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2vcfsaoyl.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2uizezutc.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2bezxienb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2fhlzhesi.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2wowtktjl.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2tgqigzrh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2tumjftop.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2xvjodlxp.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2twmszddf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2rwrfjvyd.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2sjrmmjqc.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2mqinlztr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2slfnblcv.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2xklngyml.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2aihwjrsi.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2hpurlkcc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2gmuojpyy.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2lvoocwmo.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2vxkigoxo.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2zruftiah.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2yflywwcy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2taveklzl.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2vquhxfbz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2uwdhcxgu.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2hhrojryp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2fqpvkvdg.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2wfoqxuyg.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2pwswsbba.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2bqkddmzu.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2cnqqmihr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2mllnlddo.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2bvwpkxmr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2hsktufrh.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2lokqgtjp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2ibiilggn.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2nvogbumc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ttlgkwdm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2stzvryia.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2fcjsphwf.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2nvjoooqs.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2cjothqyr.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2lbteqrdv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2pnoklhwe.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2puiroidj.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2dearwekx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2eklrxwvo.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2ebamwadz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2qznswfso.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2xdkeidcm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2hdhhuozi.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2nlflqfzs.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2jjfrmmip.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2gqhphgsl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2embmsmdg.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2whpysjql.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2nuxpdehw.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2sdrtcowe.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2rslwoqim.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2hbjkigyq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2dflfrdui.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2nacmhwyf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hgdphjhl.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2emryomqr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fjfhafeq.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2fgpfietc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rttswgtk.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2yiueidwd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2lnhmcxkc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xysoypfu.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2fcrgidlv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vpcdrryj.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2fsgahkki.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2gntuwnva.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2syaswtpr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2drrqjmmv.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2ltvrlwfb.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2yhyykrax.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2ctecjdhk.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2viezqinf.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2fdhdcvct.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2rfgpfumk.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2yyvgbgms.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2veeyscru.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2omrihevz.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2dxfikisd.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2kmzdtezx.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2cquldbjw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2tksrkgum.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2orrtfjpl.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2ucmhevxd.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2tcuxdrcj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2hmeybryu.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2ftfglkhe.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nihshdsz.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2nfgwlgza.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2geoqbmxz.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2xsaazgdy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2dttmnoaz.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2bwulrwlr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tfjmqojg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2azxzvhtv.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2vimpccmq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2tlfrsnuw.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2guzzyubi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2gozxcrsq.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2vcozyeke.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2janmxhwp.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2qigsundz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2glzcodpj.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2tkgamoum.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zbdsnxub.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2lwrjjrsh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jjwtpgym.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2gcyeafcy.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eqtnvsqn.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ehitqrrc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xembvedk.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2nwkkseiz.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wwpydqfm.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2krcpheix.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2jrwzfmur.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2yfrzjbkl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2ukdwfkgd.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2dhrynwgv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2ermgfsym.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2wtmrhuow.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2phkltnsm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nhhmiqqk.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2eysgulsr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2ztielrtp.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2pptglqoo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2kyitqrjk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2axiyzxts.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2dhgasciw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sdsravyc.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2ifejgiee.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2dywiuqak.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2uozpabdy.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2svezkaiy.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2hujqybnl.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2lnjzdxee.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2nfkkeanl.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2hmwzlqjs.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2aflohtgd.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2ytvbhoex.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2cbcpcnbp.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2vpzwlxzu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2gfbfbcng.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2wwrpmaim.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2szcxybhq.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2jcsfuwqk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2cvtfyget.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2roqxpsee.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2wiolqbom.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2rddzedal.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2lpywbnoc.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2mmyjpman.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2sndfwbhy.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2mafneqve.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2vaompxny.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2kwmuwhko.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2ehlnppyl.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2lfzdqeah.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fktrkxff.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2jcxaunry.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ghsfrvjv.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2oosxnnrp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2hepzcamy.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dnxtdfiw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2sjdfhifl.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2lntqvusl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ktubarbs.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2qvsbdyru.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2bbfjesyq.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2ewlqhexz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2kuttddim.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ivnbvllg.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2tqfaijls.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2gjerfnnn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2zdsnygaj.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2lghbvhje.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2mojacrsy.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2haftgiji.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2acnjdkvs.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2mebxypnv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2zbblncpn.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2mdjjdnai.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2ipuisdbh.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2ghfjqbkw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2tqhwbrsk.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2szxxdnre.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2kfrvpqbw.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2akqefiqk.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2kujxsmss.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ckxmixop.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2fjdrmctk.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2reancjwv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2luvhpmmu.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2naaidxwi.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2mhunjhpm.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2dpgchanf.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2qxalrtww.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2elipxsmn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2flrixoll.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2wybvstab.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2wecauncg.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2gfywjngv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2zajjfcnp.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2hevwvikn.html


<!-- 参考信息 -->