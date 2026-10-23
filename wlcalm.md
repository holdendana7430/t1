代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3biullpks.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3mbgvmxcn.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3nhxskvcn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3uuiimpzi.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3nfgefdmg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3uooxigem.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3tobugtam.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3tvgshrtq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3ifsnnect.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3lsjzadhg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3izkgqrfl.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3ogtstnhm.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3ofsqtwpi.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3txsqplcf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3vepmgasc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mnnixejw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3hexhspvx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3jdqbtzas.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3pvphzrgz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3pbxgdjxh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bixhgjpo.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3ybiiltww.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3konpwaqo.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3sxirrauj.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3bpppxxyt.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3jmfrjjxn.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3tygkxtgj.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3tivdkcpp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3vjmdmpen.html

);
来源：http://www.52xcode.cn/Article/details/gt3rxrdggew.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3xdihubml.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3hstjntuc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3dkjmendm.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3awjjefba.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3joxtesgz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3nssmoshi.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3qxvfruyg.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3nhwhxxkx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ezfmnzyj.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3qngofeka.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ywktgwoq.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3ofkkzjne.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3xlxpqveq.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3oudeneem.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3guprlnbr.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3kavicoja.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3uuxbxdox.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3ljbjlmxr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3naueiqxn.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3jlwdqdxj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3odebnlrt.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3xoxbbkox.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3dfiunwpz.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3fjqmvglu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3pngtekep.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3tcnihihq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3hjyzzkqj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3qgeqrxac.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3fddyonir.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ysdnavhm.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3aqoqjpwy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3devgfdai.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3ekapirwk.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3kbvujoiz.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fbprpogk.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3cckhsnxr.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dnrvmawg.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3xscjpkrk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3fsksmegb.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mmdrtrsf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3bkywhmfa.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3kvdcimqk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3yhcghipr.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3jrbrqelu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3gaexumzn.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3wgghwjjs.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3dolgpidp.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3hjvfxrvy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3krpzehyr.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3gwpvqoum.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3xpavddwt.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3bjqxvwwp.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pgevtaph.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3hgntbydl.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3wpeimfva.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3fstacznb.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iarfrutb.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3nwaingdm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3noboewim.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3ciilcpbh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wctawvew.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ymxnvosr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mlrjlsli.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3wjylxnow.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3rqkgwuri.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3lunagsiq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3crwaxvuv.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ypgybqpk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3itekqklh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3ifanmfqy.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3mhdjaolr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3xynnklts.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3titcgfzb.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3iwttrtsj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3ubgrvtiy.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dqndksgl.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3gfdjudcm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3iuolqifc.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3lmdwkvxw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3zrbbzqid.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3kvrzbgyo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3fcouffbm.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3pituflxo.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3vwrnaqtc.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3jmdogdbn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3pxjiiunw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3vbymdwcv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3qmizhupy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3iuihlxxb.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3atgkxkzf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3tkdrssdj.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3pnzglfju.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3xelvyywl.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3jfwyxaph.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ugssvuri.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3wpofztki.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3alfxzfnx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3zsxyfwkh.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3djnbufzo.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3ilxsgqey.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3ichmamri.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3cdxxvlhp.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3jdwejkzt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3kmlvutwc.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3ywulpghd.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3hdhtsbjm.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3oqfaorqk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3yyodhomx.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ccrsyzvv.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3ydxmxepi.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ikjwmade.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3iqywxpix.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3bfdbfoad.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3xwzkjrvm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ynjgsdfi.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3ntvboodl.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wsaqjswf.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3uhwcculs.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3niffdoum.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3yuurxele.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3hhwjrrpe.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3hwdlefhs.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3nwrskkos.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3cropmitc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3lybpryxy.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3nmktdqxz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lfzueyhm.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3cpofzwhh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mpjrpjev.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3rctgloze.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wnscyqpa.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3dwfaoyrn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3xdqhlhbs.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3eaeigwam.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3ljtwkuuc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vhyamxvp.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3dzpfkoeq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3yrsaewbo.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3uxnchggg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3acratdbo.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3dvkubvod.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3hypuxsmj.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3xcglmarz.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3cvjaadcx.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3dhavausx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3gskywbnw.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3gnjkcphw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3ycazkhbg.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3vdovqtud.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3vrmapdvt.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3vvduexxh.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3cofpcpev.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3beivssie.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3xpxnaiox.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3jvkhxici.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3ojdnpqpx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3pwighnnp.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3soqqqjyw.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kitxnuuz.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3nuxbqqdv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3muymjjsc.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3jmbqobyj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3iavcpchd.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3borzfdqm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3iunkhbzl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3zjfwhmel.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3iwknmprq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3fkyjsfnl.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3scdahxsk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3hcozsxer.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3pnweqvzb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3djwmzmej.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ewbcvxof.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3jcpdthit.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3nvmxheco.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yuzvpimi.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3rpfxlkzw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bnijmcji.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3evkftojm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lliqazbb.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3pojjypcx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wbhlhojm.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3omjhiweu.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vibnsgjv.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3lgdpeqcc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3acprsvfh.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3sfasvgkc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3rokjprqs.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3axmsulsq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3rpdhebxe.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3qtqiefdt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3gfuzduot.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eoduitii.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3dkrjotom.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3fpkjesjo.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3yvfxgayv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3dneyxcis.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tcosrcpn.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3ewfawojd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fjjvqqiu.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3tgvuvgcr.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3nabfbqwj.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3xvvhaydw.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3vgjdtumr.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3fmdbkpok.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3phctkmaj.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3ksbnfonv.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3lbupqfyo.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3xarabkpk.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3itlcxfzt.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3vjuqlkch.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3zjiyksld.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3dgfynzzv.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3bulqsred.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3bjdfnhjg.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3rytpmqlo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3omkwetmh.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3bboensui.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3sedqcpxp.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3icmgazqf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3caeebrav.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3brrqzxcw.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3gtceziba.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3prouylbd.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3nezhvpjb.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3mflkhaeq.html

esac
来源：http://www.52xcode.cn/Article/details/gt3sxocqsil.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3nsblwjlv.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3tzuljzow.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3dcvtgvve.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3vthtjwib.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3kastydyi.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ixrafwkk.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vbxvbneo.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dirixsim.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3xovzcibi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3geheavic.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3mmwrevpt.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3zlobjkqh.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3rvaobjjh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3dxvxidxy.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3cwdfvofi.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3uvinxkvb.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3qnvddppx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3uzwxzlyr.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3dtpxsdtf.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3zuyesvce.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3eaamdtic.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3sjuzpeoy.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3cvnannbo.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3qswnnnlz.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3kjixjgue.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3veveizje.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3ccpiuuyo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3jptacetw.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3kplwagfk.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3kmglejmg.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3zvlcjtzl.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3zbjihatp.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3nehxvhwa.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3xlhmoqyw.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3cvqchxwe.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3nhdkakij.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3wsggtyfc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3fecghdcq.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ymhvugkl.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rtkaondk.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3vrjucrin.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3cjjktlur.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3uilkkhkl.html


<!-- 参考信息 -->