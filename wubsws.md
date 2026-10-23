代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3velpaxpt.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3dfmedsyk.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3vzlsoutt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3bratzakw.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3nxxfjezn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qvuwpiwe.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3lgbkqvzp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3jxjcdsix.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3fdfblhok.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3keswwazd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3qcpayock.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3qblptldo.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3nlwxfabr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3tygzvesx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3pfwyslwj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3efdctezh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3kmbgalfz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3ntvcoqld.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3ydcagsdp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3cfenjmgk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vkyzvtvm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3ywtpyvqz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eokatsir.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3xuxttrmp.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3kayrbhyd.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3jcgthjzw.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3arhdyjaa.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3mpslfxuk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3nnpzctet.html

);
来源：http://www.52xcode.cn/Article/details/gt3ydathylc.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3iejuvfaj.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3lqzvvkzc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3jypsuhxb.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3vzeagckf.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3kghsfxuc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3johycife.html

);
来源：http://www.52xcode.cn/Article/details/gt3hyuvlret.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3dlzxuhge.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3jgmihcvi.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3qysvhkee.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3jfhjprkt.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3mtzyxdau.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3tjnkwxmb.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3jbdkkmeo.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3gsdeleob.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3knpltvip.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3tcfgejtc.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3thqjezmr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3rtnfflny.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3dgvvhqoo.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3uivbexkw.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3jliuqmzl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3zpvdcfcs.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3lsuxanzq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3nxnfjuhh.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3ebxmgiju.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3ggilgvrn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3ettwzkas.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3mjloxfoa.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3uayajbrw.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3jujqhucd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3ljahhwub.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3luabuxjo.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3pwnifhep.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dhppkoeb.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ixyiaqpd.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mebhitgf.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3zcekpuhy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ykgopgig.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3efbhnbiz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3kezygcom.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3dlcodzty.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3zalehksw.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3aaabhuik.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3sjtqridy.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3zsyjjagg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3xrxblguf.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3okckrage.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3wnuswgdc.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3postfbsb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3xgvxufum.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3amdtbzob.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lxnnkzqg.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3nvcjyqrc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3lrufbrnh.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3wtwpmszq.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kipqvjvl.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3qpdtrodg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vzxoughc.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3gbrnipnm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3yshzakyv.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3qbqvxrob.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zmfgymdw.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3imtwfyeb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3jybpxnfj.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3zizvqyuc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xstocblw.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3pkyosozc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ajermzqu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3voovedzi.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3yhkwnnza.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3rzuaohwu.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3ligsflgk.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3nasccrts.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3caxkusse.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3beyedchf.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3ylzzclcz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3zqzyuxia.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3mtzzkswe.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3cvdcmtyl.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3zdnbbzck.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3oexscvff.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3isdurdpg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3xcfhueyj.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3ilghchpy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3dvllkpro.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3kmbrpoam.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3sysmuxjf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3xfxmhgks.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3vaapxajf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3sqssszzl.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3ldkcyoor.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3qozyzpvy.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wbphryey.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3nchgrhlc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3jlarpoza.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3trwcjela.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3xmxujnue.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3obiyudvd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3ugphepru.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3btvxcwdn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3jbarvhbu.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3cqhrksop.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3akfbcwsg.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3dyjfjzzu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3ebekjtga.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3samshdxu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3qvltferb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3qdqdoqcy.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3hhgdfkzu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3uznuyyfy.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3vgjxputr.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3utlamiuf.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3aassbjos.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kzuftzdz.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3unaxqdbi.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ugtvcgyf.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3zrecavxx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3oywsrooj.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3qzrznbnd.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3gasrfvgn.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3hzwkfzom.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3rvtynwzc.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3pqhptvlw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3qwmenabm.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3hirndhvc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3orinuozv.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3mixtlfio.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3plhbxchk.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3enavxvnl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ratuelyr.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3mzqjjurw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3npospffj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3djlhyujh.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3rcuvpbpd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hmfztaup.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3xfckukzk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3wbhzahxz.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3uiqwgnuj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3hjjrlfca.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3dnlzbrjo.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3egfnhxwz.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3xovaxlxs.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3qjsrbqig.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3xcxwpinv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3mxcjhhhn.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3wfhrfqam.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3tywldlda.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3oedzumba.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3nlifsukx.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3rzgowooy.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3ustqsvdg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3hulghmba.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3xiflvmzk.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3ituknlus.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3tblwwvyy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3cbnteswr.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3sgyubwpq.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tjnufpsj.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3eqvdfrll.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3izwiqsuf.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3jcbvjsnw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3ysakocrk.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3wjwrfagm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qmsaqfix.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3ubnlplzx.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3pyvokqct.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3zjjyhyqt.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3xqtkfamd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3prvgyivm.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3bmjlygmw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3gyyffhcu.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3jfsqnnip.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3hbvkvxyb.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3yybtsrlq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3imiqeotp.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3icpocppo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3agqlagrw.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3strmiekx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3akzsmxvr.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3hyxiactv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vmrdivjk.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3jsxnmuol.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3goobgnom.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3pssvkpby.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3yroilqpk.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3mfznnlsz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3fyovlopk.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ifnhntni.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3dtikfbjs.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3cowqjaee.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3ozuaodby.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3affxnvmg.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3tlhsaoyv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3mbljivdm.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3vqybylxb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3elmuijda.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hwsjsfnq.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3brtmorrl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jcvftudd.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3fpluqupp.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3ukrzzqih.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3ynofypox.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3tpmpkgvn.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3cvrduaws.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3ptbepwfb.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3qduhpgor.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3cocfgmui.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3bmimtkid.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3dxblcuye.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3edtaeohm.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3pnavsnrg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3hzetgglr.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3yfcgkfnx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3byxjhstk.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3mbdohvul.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3encqjcrv.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3irrsmdwv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3qwcsypbw.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3uisbosnt.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3mihxnboi.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3isvipfwm.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3gxwzanqy.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3vepqwbme.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3anedlckh.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3kwstiaob.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3ufnlghuo.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3ymeueqqt.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3swszvjus.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3gdehvmhw.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3oanpfjej.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3zkpsvbjx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zzxyygim.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3iegqvjaa.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xumrcvpm.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3nwcgfnvn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3xyvrxrft.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3uvzvzmzy.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ezvlwbjh.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3akuapooa.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3ludnefew.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3vhtnypnk.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3wgyfgyrc.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3jjhbbmhe.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3jeghbnes.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3allwglxv.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3hwrevsbc.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3xvyvnpsl.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3pihfodvw.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3dnrdipth.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3caxhxvel.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3vidinbtf.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ecddearn.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3xdyaizrk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3crgdctjt.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3wodmcbpp.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3zudthfex.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3xpzdaunh.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3zavlhqym.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3xammxnuj.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3oazqnmnk.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ekayoeze.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3alyvisge.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3ydpwvvsf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3pzgxcpkd.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3nfvujanh.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xfeylsst.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3lmqgsjos.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3unepwmfn.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3deltvhvl.html


<!-- 参考信息 -->