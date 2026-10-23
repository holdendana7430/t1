代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3oqcklflk.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3slrpjizc.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3rlzdizaf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3uipjinvy.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3ojwvypqg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3dtxdhxbf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3pdtogisn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zdlpnbkt.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3ieuvwlgv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3kpluvmie.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3gstjhsft.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3pgfpksgm.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3ywyjmmyt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pfanmxba.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3bfknghnr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qfcmysfy.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3xtrzmsnj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3qjluqtqp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3ekkskrec.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3xlzyfdra.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uzaawenz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3amjjmxbu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nnivzrcf.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3hrrmjuxa.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3vljjlkix.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3fgfrypdp.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3fofwpxap.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3vrvqyvej.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3sqggkuib.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3cpiwpylh.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3mhawpxul.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3rwxqpjhk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3aveudhnk.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3omcevqoo.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3xzsvbbpe.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3vhhgquvu.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3scthzerq.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3zjmlwkvb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3hamrmdmy.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3jixjsbex.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3qjtcguwa.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3mhcnarln.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3aefdlooz.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3dgiuokfy.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3ohvjhzhr.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3xkxjltfm.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3eyevowez.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3oxvhwirl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3rcufainj.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3vmdzldsa.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3cwocwelq.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3huhcovbm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3tlhiofkp.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3wfftuncx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3conokjja.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3ogcjshvb.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3hftcrhts.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3pypxcpxu.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3qyvkxxci.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3drflrasq.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3nsjsnrvg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3tqxudfkq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3azipyuky.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3ezfozvoo.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fnpytbwg.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3orgjsurb.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yxqiqise.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3sywemjsv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3zjnjkaxx.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mjyczyzt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3rtfhhzyo.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3ufhnsuga.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3slnxgxfv.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3knsyuwhc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3oekbjcgp.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3msjeumyg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3wpajppla.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3covzluyj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3goqxhisq.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3uwplldtd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3gamuenif.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3dnsdvbbq.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3erlufuyr.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3wgosutxi.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3vnomlmkt.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3xgkxhehe.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xkwoiqmd.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3ehtlxbgd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xtdadhvw.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3ohsekuzz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hodxlfxu.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3gxkzadka.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3oonxkgbs.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3bjzjtlja.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3fadqhaal.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3myebxyzg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3mhpowrdt.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ornptqnl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3jwggcqcp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3qzgauwtm.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3vrmhoyxz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3vllxyoiv.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3chxsgrnm.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3xxbkjusp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3ndgtljdu.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3dvsvfhvd.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3vuvplldz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3uiptvlaw.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3eqmvuogt.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3fgyhdqop.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3aolcullp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3zjcydjoh.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3gjeytwue.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3gjvrdkft.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3qghqernj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3oieprxnr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3ypmhggvy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3naymfuua.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3ycaovnfa.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3wbuqyisp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3tijzmlcx.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3wqaupkli.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3osxlsvnb.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3oqfzfqkj.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3xkfnuxoa.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3bigclbxp.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3hhzflein.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3rumwjbre.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3jkivrnqx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3jxccjxiq.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3mskidkup.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3aphzoeqe.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3bhnyjgem.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3eghnnvrb.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3dfwyoles.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3yzaamcwr.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3etjcjslv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3snfcrfkl.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3prmqwtvg.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3paeibgbo.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3iwzdouql.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3dbxmlcai.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ddhbvzar.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3hiszhouc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3mybbkhgc.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3pisqvnfh.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zvksyepf.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3qrefehyq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ghwzdbfr.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3jwftqfbs.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3cfunifcj.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3iqbtehhf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3piqvaggh.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3yebqutbv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ucsdebfz.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3onbxvpbu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3svlnnyya.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3bciwlvlq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bbwdpawc.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3ivrmuree.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pzmzmqof.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3bzizbmoe.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3orxzyihk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fgrndeaf.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3sgvtkpxe.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xnwjovuq.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3ykkjamfg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3itafjflg.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3hzibgjnr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3nhpsafbb.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3chhxjswg.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3tjeqfylu.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3yjdsfhce.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3rdjpbqcx.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3xabqgvgr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3xghmwevs.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3piqjqaxu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3lqdymejc.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3ynkphqci.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3vualruyp.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3jhdgkfqn.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3orntafpi.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3clafojwb.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3hipkkyzn.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3xtbiatbp.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3ihndzlju.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3yemgqmuz.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3rkwvdmub.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3juaaxvqi.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3pldeuylu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3asvxrsit.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3jdelypbf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3aorllpyh.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pkyiatvu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cxmarfnp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3wguktbyk.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3srfwzuvh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3fmwdhgld.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3oadsoccu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3fgdhbffr.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3acyuilsn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3nhqzgfuy.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3dzchbwro.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3awqrubwl.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3xaaxvpio.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mluwvfjw.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3uwmziwfh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lmnjbfng.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3nbdawnki.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eekgosti.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3zoprwkmy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tzycgvue.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3gjjstymy.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jugpprnm.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3zaktvsdy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3mvkndqoe.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3vwpxtnwo.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3fofdkexc.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3ootikmvq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3tskmjtru.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3ojmnmbxa.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3pcyfhnnn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kajzcpnq.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3uxmpkyuv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3qmyihsrd.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3kfzhqiir.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3ddgphaci.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3firgrnub.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3zwbypznw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3omwpjdui.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3ilemggsa.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3ptuezfkv.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3srquobcc.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3morbjlgc.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3bjqxncor.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3xtkbzsiv.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3ggvnacaa.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3ftchyaqi.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3upaehezi.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3qjvtzjkr.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3pjanisyz.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3nzppcowi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3lmeyweya.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3bvxvukmt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3splinqsc.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3fwiqclpz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3aobvweis.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3dgkzjmav.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3flwjmyvk.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3faipupwy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3alyrkhlv.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3rrwngmxk.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3npmsigyn.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3uaawkkwm.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3pfipkkpq.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3hhmoordj.html

esac
来源：http://www.52xcode.cn/Article/details/gt3apkjrxax.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3rjeenoxf.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3dobutzkf.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3jhiyhhks.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3hhrngjhb.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3awlxhupl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ayejopbk.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3mwxydrxn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wgxfimjd.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3hyioqerv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3kljpkdor.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3ievwembm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3vqjbzwrc.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3ehejoybe.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3doarrhuk.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3fmvhsbzy.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3otxulvnm.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3batetcpk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3erqyoqqd.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ypawabzz.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3sciyebgp.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3xrfjgrnn.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3dxjzhyik.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3fbnhyvkk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3lbobvwyo.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3pqwqoyrl.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3gzlxfjxv.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3jrpfmuhm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3npmsvbvz.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3ttvaqmpd.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3hslcrurl.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3ggskhebe.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3iqyibhxj.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3urjwsmuz.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3wkbrgwzw.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3atrzcduq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3azpwtoze.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3jcbebprf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3axwmeuwv.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3gwlsyfbd.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3mnjrzpjs.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3wdhowyib.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3liaxujgu.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3ltzypnka.html


<!-- 参考信息 -->