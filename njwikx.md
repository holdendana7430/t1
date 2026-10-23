代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3jcoaiunn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3jiaiqlpa.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3feaivddv.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3fmfkbezz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3jjczazxa.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3vitomvsq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3vrtjjppc.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ukmenvxx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3qvdzkbhk.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3tjlowjze.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wsrugbyf.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3zdqlqdum.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3goscgbum.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hvjjeycp.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3mxnexzln.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3cyjncuus.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3nrmonhqu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3vroawkmt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3rtfmgsrd.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wjmwsxlz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3qqmqcwka.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3albxqzjj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3tcosohos.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3thhknxpp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3asxetqbn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pilmbwlt.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3zusvcanl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3btzoppzp.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3rkhuxcep.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3shtwxhmp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3tcyjpiue.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3vvsvrfys.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qnduherg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3mvtuqicy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3foagmqud.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3zycmcwlw.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3mwqfeerd.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ahsbgbsj.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3qjdubswd.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3utzwqztj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3oedsjbyh.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3juosdyak.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3hlmowzsb.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3knnjrcjz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3kjcvfhal.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3giuesvaj.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3ipkyvrtm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3jipgzuhy.html

);
来源：http://www.52xcode.cn/Article/details/gt3qjblmeop.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3ynjdffru.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3ehrmoobx.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3rkanbfyo.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3qlvjeoyo.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3rdliqhsw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3nqpmyqmx.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3orhvdnvd.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3kgisnnjz.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3vtoedbvv.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3ezojsonv.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3sjvxfvzn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ebsunegc.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3nunctomb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3xgoyavis.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3ekhasmmc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3gezcybvr.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3zcwjgyxo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3qqrobefb.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3sznwciju.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3bxprcmhd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3gebngatt.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3dlpbjhvf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3enivqlmi.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3ljwzshcs.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3fhlpwmrp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3lpczvsnz.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3erhmeheb.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mwkjxyzv.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3tcmmrtjn.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yzxibckv.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3tijhyfop.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3blqvpicq.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3htsupzbm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3ptqfdyjk.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3lysqnacn.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3wfewiwos.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3dhcuevpp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3drmoddhh.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3cenjpicb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3hiburkve.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3pdibclyl.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3zkyaosqf.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3meqxmugk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3wopgwrxg.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3qmqucsov.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hngkaycb.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3dacpsvpf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3rtnydbjb.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3yvfzggck.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hthzykrw.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3dhkteook.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3akknrvud.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3jxsrwbnq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tohgpcif.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3asxgrrrt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3woxlgdxc.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3vercvbyj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3lazeeosr.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3ohudcpmz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3lamrxmjb.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3imyxyydu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3plioyudh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3nujjkhxl.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3hrnpfjwn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3uicsqnod.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3wxwpmabl.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3lrhdyygs.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3rxshknqv.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3urcmwhwe.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3qhpxfswa.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3jzwyuggm.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3krhdptjm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3zxtitibl.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3dlrujfru.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3afchddtd.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3czoxhtbu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3udcxloiw.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3pgscavbv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3nbsddgcv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3kzgzlpfp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3dprzjcmz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3dzfheqzg.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3gtchrvpp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3ecfamlhp.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3hazzhvuf.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3oyagpkmo.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3facmpapm.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3pzsemvpy.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3mwwvroap.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3grksfbtd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3toksbcio.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3pgsprmyh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3qhcunwkw.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3fxmwacli.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3smvetgxb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3ksxohtkn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3mdwdmtrq.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3zafrtnpy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3dqyjlxru.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3oianvbcg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3norjmohe.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3sqidqrkq.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3yljrzqrb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3bgmjixbm.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3timrcgce.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3styhdask.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3joqydazs.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3prxzvmlh.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3eelqimny.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3dchladww.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3svknbmlj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3mketkeay.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3zbdixwmv.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3efqzkwkd.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3qydmkhls.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3mrfsbhyq.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3fqqpwmfk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3iylfyyui.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3fuxqvoxn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lbgcghxu.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3psdfgzjt.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rvodemke.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3ryglutye.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3uhrhronv.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3pyeaqwyr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3lxldkolf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3uepgfrgd.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3cwqjwcfo.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jaqbgjhu.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3aywljjoj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3dczlurvn.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3iapnynsw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3wtdaihkd.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3fpfslzpg.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3ffsibift.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3jraequmw.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3zmwleqtu.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3mfuhaisg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3yhdjensu.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3kmfwnbba.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3tiirhday.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3mgqkpvse.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3udwughgl.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3wjcmmfbw.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3qyamlgzs.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3okbodcne.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3ovaslfwi.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3bdiczmni.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3kyxkccyp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3vuahbxmf.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3xyiyempq.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qnfzzuok.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3cxuodchd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3mfdabzhj.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3qvhnnvxd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3idxvyglm.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3aitldzmm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zjfweccq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3pfqcclrw.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3rwohmqts.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3inehgfpy.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3zehzyqhk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3dgzqoqxb.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3ridmmwrp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3tnkkjsui.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3bqcisopw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3homasswu.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3kgdayzad.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cazuqsfv.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3hzetouvr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hlljrqmh.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3jnqpjfzy.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lczplkat.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3xkddwbqj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mpaapwfa.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3mcnhhbbe.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tnmlrvfe.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3glxovnmj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3eztpmkda.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3jpsczmcf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3giohwlje.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3uczafjyc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3fwsvlhqf.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3yujodgzc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3kamzqyha.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nyqmukzx.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3xvjvlbbn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3socvqoyb.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3vsqtcrxd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3crmefyaw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lrnvqyai.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3hlbpxatw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yglmvyvk.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3vmxbmqpr.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3rwmpjede.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3ilcapmdf.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3fjgcydop.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3tkxkmnkx.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3lfotmdry.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3hwlrzyuh.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3eztluwwq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3otgfkiqt.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3wubebsjs.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3bvwersfe.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3qzouhcwb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3sudozhnb.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3uoyihdlo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qjhzodar.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3abfyqawu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3pfnldiyx.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3cwifgoys.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qgvtpfdd.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3omvcerjy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3dexdeguv.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ieaktdmr.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3gqxmekjq.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3dpymxpzb.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3rqefyhiv.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3yhxsaeip.html

esac
来源：http://www.52xcode.cn/Article/details/gt3xuhajwnn.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3ppeqnyhc.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jrplaxkj.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3lrstfroz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vzxoxwja.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3wjsbecux.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3whmzzcwy.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vemyigav.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3huqickfo.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3bhkzyedg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3yiesxvso.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3kupjqfyk.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3imokjvik.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3fqehpmhp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3atthgngx.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3vmsztsdv.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3rmnlpmjr.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3jvxlaxda.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3yrnhgisc.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3gwrgwifh.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3rzxoyogg.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ppuocrmj.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3ddftxtjw.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3gcemqsav.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3orfqublk.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3fchketlw.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3zelroljz.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3eccgkhan.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3pwwgkfce.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3ybjlbqmc.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3djmveqru.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3ijfdkmdh.html


<!-- 参考信息 -->