代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3kpmkjqbq.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3vrnofvdr.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3vfrvfkba.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3ptgirbuo.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3jhrksmrc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ivqupdrm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ryfljlep.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3vixudogh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3cogwvkyi.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3snrnunol.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3ywjjrdyl.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3ujdklkzx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3iltjurml.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3ezkujbxl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3mhutbvww.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3fshutovc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3ytjwakit.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3nvxhkiji.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3nuqywnwq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3ojnnczjz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tnaukgqp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3ktugpyet.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3soicgghj.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3bftezkja.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3qxeftgkr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3bbhuxadp.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3fhanpmax.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3kojeifmw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3xletrdas.html

);
来源：http://www.52xcode.cn/Article/details/gt3eabehdvv.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3jfjoadbh.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3axbozjsv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3uthistnl.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3posbrywo.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3vjyutofz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3ylomvlqn.html

);
来源：http://www.52xcode.cn/Article/details/gt3fbyvwpam.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3xzaemewv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3holzorcb.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3sfwiwonh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3ncxexnup.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3rjalsjjp.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3jpocxxzv.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3pjrowkkg.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3tfjueqnc.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3xdvzkkrw.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3enypnjlt.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3vmdcsxlx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ngvqmkuf.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3lpndnrwb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3rdemtveo.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3ffmpkpwl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3fgymmggz.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3esmlximp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3nsltxbbg.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3tcqohhxm.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3rdxezvyw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3imukclln.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3pfwzglgi.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3wiztngzm.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3xmhemtrn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3nrdaisie.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3rhcqbhjb.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3wezuypih.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vofyvgnz.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3hmxnhgrq.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jmrxjaet.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3hgptmzdn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3qxzdzadk.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3aeklynnn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3kpbjrubz.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3wkewxwtc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3lcwvjnrg.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3kwlsuieg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3scjjeetv.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3gagyolan.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3pvvbufql.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3sujlcrmg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3euyjdzem.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3ydntxzli.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3nchfvlye.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3zxrvtynx.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lwdsyson.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3lhjbjipv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3lpbwsmsq.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3wvexwtra.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qrdvmmxp.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3szhpaysx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wnllcbgb.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3gwafqjng.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rsbpaygb.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3awlpucys.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gvyuleeb.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3risygrxi.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3rdkmxail.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hdfhgkni.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3hohhqinj.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3oxuunufm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3rcbokksq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3rbbqadem.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3yuuuylhb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3xuxbsals.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3bdekvuqx.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3mhvtjzlo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3nbfqxjiw.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3ggdsemce.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3pkchnarj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3afpitwmz.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3tpdndrlw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3unawbuhc.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3haqfxidf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3qgugftzo.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3jdveenzw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3mlfpbcaa.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3lsedoiav.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3ddzaptue.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3mvvyzzwe.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3yauwfsnh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3ytmmksvc.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3ikbffgdb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3lsrjbhlk.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3lsvlqzbv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3idqjlzcb.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3zklffiwm.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3lecrtehr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3trtkxqrt.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3etdzpoya.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3dulgtuyw.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3sgxjfaty.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3fksdtkfc.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3rutjzauy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ixpxllox.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3tikxqyxf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3bvdhbpvm.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3hstxreir.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3gvbsjtth.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3uysagxhz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3slcmwsew.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3pgqkhgsv.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3jnvkrmwx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zslxxpyy.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3zfzuseob.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3vkrbyfjj.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3mbuwxagg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3uxbnwwzz.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3jftnzofc.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3romamvni.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3scnxjrhb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3rfcmhtkp.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3puhxbzpg.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3nwpzdaps.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3sbpndbts.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3roxxznmv.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3vkgermoc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3siwwqvgm.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3rwjmkcqa.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wspeyffc.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3kjgynfzr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bgitaixf.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3rsifxfif.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nvzspdpn.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3zkxjafjs.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3nqklzeli.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cylunikh.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3xrijhqha.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3uqbblsho.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3jmfjbira.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3blbxtrxz.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3kvgwellk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3unhkalfn.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3ugalxfsj.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3oqwcnisr.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3oltisbra.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3jttmnvpy.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3koxowsrm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3zsrzlatt.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3vesznezn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3nymgklfw.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3aqstqtwk.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3epkzrfbb.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ntbqkwfp.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3iskhusvk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3liqhldxp.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3mewhyioz.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3pkpdljdt.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3xcnghbkr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3gzfuwfde.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3tkxhorvf.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cjvpypsi.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3tlcporbi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3srndydqf.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3ktnfwwmf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3twcuwwsg.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ngburapt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3oabwsrkx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3dgbfgtsk.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3pjxinztd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3jqkzbtrq.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3lbyinjcd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3tbokihks.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3qzstxtlw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3ieqnoozx.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3qotlygeh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3cotteots.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3phlrcyzd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ybhhyadd.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3migkvxyn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qaflmgiq.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3yklavpxl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eqilyial.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3pagcumxm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sbrmmqvy.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3asspmrko.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tiigtsfu.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3kdutsgzy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3vidrrsih.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3jnxveasd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3evreigjr.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3gwqqhbmt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3gwqsmtxj.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3jzilfmvk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3zuqgqtiv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xdpeylqb.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3mvnunegx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3qswnusla.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3dhrtunkm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3bvxmsljw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kvrbqarr.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3isrjnxsg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zjlcuydg.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3gdrvacbj.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3bfgxlirk.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3duwzjxlb.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3wuwicwpr.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3qcxbdgds.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3fhhvgbuu.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3mnswfkbr.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3kfakfznj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3bsexqefa.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3apxcmaow.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3xkwwaeky.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3koqzqovf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3kgiopqpj.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3iwzppidc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3datixzzb.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3fmopbfnu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ftgflwvx.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3nprclccp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3iotfwmik.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3qigazwsf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3fdtcgtxm.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3rbecdsrt.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3ezmrnuzw.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3esqxueib.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3cyqxqnhg.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3frmzkgww.html

esac
来源：http://www.52xcode.cn/Article/details/gt3stzxdtlr.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3eprefpjh.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mfggdvzv.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3taeztzgs.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ghivdayq.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3aembdlsx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3mrveluxu.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wutpehnx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gjkdyqqs.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3fuxbzskz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3fzstltbp.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3jiytbnoc.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3dmcvpxlx.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3jfkcjctj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lzelipno.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3eorlltkp.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ewsrslak.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3ynpdfsjc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3fmtfqzuj.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3wpvmrhuy.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3iacqoxzc.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3qnvmhkuo.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3uxkzorcz.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3rbfnuwzw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3occesvye.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3xyjxlqbm.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3dxyyelxe.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3rjlztelz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3tznnnihj.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3ewzuktfr.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3ucujnpsx.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3iubnlsko.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3zzbmwpqp.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3xpzeecpx.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3zmcsvotf.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ioewdkkp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3kwnhfqfg.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3frppnufz.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3lufgacip.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3cebjfpxf.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvyrznyb.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3ozlqdhbs.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3kkyrvetp.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3esiplygb.html


<!-- 参考信息 -->