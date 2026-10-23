代发 wailian999

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3avarljdn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3bkloxnnt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3tcuujcdb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tbvvnvlg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3fxjadkcs.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3cfawkgmn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3albcwnmt.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3mngqgkxr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3gqoobeal.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hcpirhls.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3yxnhfjas.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wphwpvhy.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3htufldpx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3hfrokbhx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3ygzyvdgn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3wtjwypdh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eidacoqs.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3gjbnpwlo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rvbjritm.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3fzgymaak.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3gpknsnev.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3hixswhkn.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3xgqgilhv.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3tyvylsnq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3grtzbjba.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3fllqqxqk.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3efpcrbpb.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3xknoigpl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3hyebmuuz.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3sfeloboj.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3cgyhjpik.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3jrwvhome.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3tfggdmro.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3lmzoygau.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3nqdcghqr.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3akmoabut.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3mdkielns.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3dlwqmokw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3lazbbnpb.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3upmzfiik.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3jvtegdvr.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3styhtowh.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3suflmrgv.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3nwfkeizv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ogzbjdra.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3mvuqsogo.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3xkxnaote.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3sxdyhtkw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3jipzarls.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3ksuuxpue.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3rsfwopld.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3kalljlbt.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3tnxiopqj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3sezozsyq.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3dyupibah.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3lcnzpbem.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3iwzwfbro.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3mfwtmuyn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3lvuobwpo.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3wazatakp.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3czkoxlpn.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3cygmvimt.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hznwunfx.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3nirqpipx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3rndrvfvd.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sdgrsamf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3twqjeacs.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3yutnfymk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3vxcwvwrk.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3srrgkper.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fwasbvba.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3dvlrffep.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3blxcdaoo.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3jtipxtib.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3ziwoxfiw.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3qfuntogy.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3thcyyhlx.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3jvbuuuev.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ilzinoaf.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3ytbbgtje.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3knurdvaa.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3ygkljxhn.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xcgokxtz.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3zqhmztbl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bsfdmxtg.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3greqslly.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ybioohjh.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3dgybqhoz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bqujnlqy.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3ryahqajv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3bpktsktk.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3yklpeyvr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3eqeolctw.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3dpwvawul.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3vcxsdwwi.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3irhnalrw.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3lngvounb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3cocvccpr.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3amplwbxf.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3vlngrrct.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3pexkaqnf.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3tusixuis.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3jkdjmnjf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3abuwmhyr.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3ysnrcarx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3udxwasxe.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3icibvvcs.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3kbgtrish.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3jvcodjlo.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3ypmshuah.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3pcxofmoz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3ugwlylhu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3tqfudfti.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3wnfunaqd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3xyyfygkc.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3otoupxns.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3whnsboyw.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3bzkdhdhx.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ytbqaasb.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3azahvrpg.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3stumjmgd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3xefeuohc.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3rnzshtlx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3cnjikwfe.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3olykbvlm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3jxaclcro.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3afsompgq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3yyitvetv.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3wfpsbavf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3mamnhejy.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3obmhzodg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3bbvkfqjk.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3noneuwqz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3bkzcssjh.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3aroorxgt.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3wsoinvlh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3pztsksge.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3lpmvepni.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3unzcvohf.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3xqlbdhac.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rctglpyy.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3ydogrvpt.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3wugrprsk.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3ifisekjn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3tdzhzsnb.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3blpaoxtv.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3rrufzyhd.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3ngjzizdk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3wlvenzco.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3iecyvfsg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3lugziang.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3zrcnbyud.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uddeacmb.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3yukhkwxi.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jcsmuqje.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3ttiktbub.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rufhwoge.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3inzbhzyg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3frwusxvw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3yldiwnje.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3qcyjxibu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mzbhgvta.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3xjlszzgz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3dmreemao.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3jkhwaaff.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3txrtokzo.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3rvzgxroh.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3taqkoryw.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3dyyuarxv.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3pcqstjth.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3kqktuuqj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3pndtllmy.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3jmxzdist.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3zugzloqd.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3vjypjvub.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ucviqxdd.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3yyhgeujt.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3coagiyvn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3yzjlhtkr.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3ftexzjmi.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3cdxzmori.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3csbobbkr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3xibsjxqf.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3gxaewgoe.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vfsxlofd.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3qstumazk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3wxbnbufh.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3gjozdmob.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3usveglvi.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3pgtpgwnx.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xtcahunk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3aypgpxvh.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3btphhiix.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3lstpewsr.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3sxecgyii.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3hmmidkkj.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3xshdqewr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3hwvmybsa.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3idndqkoi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3sketphmh.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3fxwbutyl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3guxggqte.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3swkfweqz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rzswagth.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3wptafwmi.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sovvyaez.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3yvaumdpp.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3soioonbn.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3bawtxxos.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kwletisl.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3raoonntj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3rjposbpd.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3udvmkjrp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3bsbyhzej.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3omcidvnf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3jestjzns.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3gxihmuog.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3lfcwtapd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oxlbzucw.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3qeuydjjo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3kasdwmwo.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3mtkirxps.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3natzgcfs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ixjfnpid.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3jfkgmldq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fkyxuglw.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3iopcycvq.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3cwauxbaf.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3exzjgelf.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3ctrcmelv.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3tgiapgsk.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3ugsxcrpj.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3sasxxfww.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3qoesepid.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3ugpjlune.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3ujvywmpr.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3nmctrigs.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3fcshurgj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3cqufzqef.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3yxscidrl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3apmathuv.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3okfsyuxy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3kmzzhmbk.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ffiiedju.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3kzuhdbvh.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3rqmhfxzt.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3naarrrhg.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3sifoesdg.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3bdvbyqlk.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3lexttwjc.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3pkaielci.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3zraicacc.html

esac
来源：http://www.52xcode.cn/Article/details/gt3sjmbyhxv.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3nbcmcmnv.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3baswcmfp.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3slhmypzy.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xexiknqr.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3ngoqmvxl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3pvmodypd.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3oaoezdam.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wtpmgymi.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3bclgdoze.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3pyyquwpy.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3uauiqxae.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3rivwtpji.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3nplolokr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mutddpix.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3cjdklinf.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3tfqhvprw.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3malnsiks.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3pvlzxjry.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3wqpobcub.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3hqysbanc.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3dimdtkfk.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3sbipbqqu.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3sjrcdejy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3mvzxvrlf.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ugoewhuh.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ryhldxqg.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3litmnjke.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3vftplmee.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3jpgejhvc.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3obyqtmrc.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3zcaanxdt.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3qficyesv.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3goxihwaf.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3kuzahhzc.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3mbkztoyu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3zjhbxzki.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3xtmmgvla.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3phvowbbq.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3gbviodtq.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxwzabrm.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3czopwljb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3pijpmjgh.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3harpnxno.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3pqbbjdsi.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3zbpmceal.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3dhxrkuoz.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3arjagwwd.html


<!-- 参考信息 -->