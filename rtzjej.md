代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2qvuvpngt.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2tvwiknxf.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2ogmsypcj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2upswmmhf.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2xdpevtyn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2qfheyihw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2rayjfepn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ljqpmnrp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2ipfzjlna.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2uwegsube.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2dtiymsnd.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2mtpmxzkj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2gcnusaqe.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hhcvqubs.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2unrfikej.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vxxvwnne.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2ztmpzxov.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2uwqzbtof.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2bkjstwqn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2ogclcqsh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eqvswzwh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2mwemnecc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ckvkbard.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2xejsetnk.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2rkfzqqia.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2sassowmg.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2vukbfyek.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2pmnavgxg.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2lbuxpssr.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2oqbhlmsl.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2mofwszuq.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2eezdostv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2nzcyuuse.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2kzayptwl.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2ztootzcu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2oliwmvog.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2rukgbwmz.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2dxxfgabq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2cpnryods.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2hlcdysbo.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2xlkjiiub.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2pdrlxpcr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2yzfpzktv.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2qcdyeush.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2oluahzja.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2vlqrwklp.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2hbxjntmy.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2ivyivlwz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2zbmjalhu.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2sbgspoib.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2xjupzemw.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2vexzepfl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2bdgrpxpn.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2uidngykx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2fkeodauj.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2htxqiqqf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2hlthmozc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2hzwiwnoa.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2hxprbfcg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2liqplkrl.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2zlmdmuya.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2qnlvgfyx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2crfftedt.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2agwqmkpo.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kkbcfpin.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2dotbbltb.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nlicqgxq.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2fekhcovg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xoohgcld.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2icgsegvv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2trejzjcw.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2tygjfoae.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2wnjsgxwe.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2xflxdafh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2nqearfyd.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2stliifqz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2xufxkgjz.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2svhpkjhp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2atdfhlyw.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2uawvqrgd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2pqqpwshd.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2ozillcwr.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2elmutsfh.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2qbwctsye.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2blgwqqqb.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2zgkuulhb.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hofrbzkv.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2moskhpka.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vhkyprea.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2jtohknxi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lyedqjbw.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2hiidfetp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sfoizvxp.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2shspiehg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2qvuehtiw.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2qricciqu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jolvvadv.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cpyvmwcy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ismvhsje.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2qftixddm.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2trkcwzhl.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2lmskoiqm.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2thpheuxy.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2nvnpqvzq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2zjiormey.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2ocjhvrgr.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2byilqzzl.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2milixzwo.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2ucwbakgn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2xynkakcb.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2joemaaiu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2jiqcihst.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2uwxkxtav.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2fjhgxhns.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2wxvuntwy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2aosdvzvc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2fuvehgco.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2zzkcawxx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2xtsjtmpz.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2ipplfwyv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2zvwklyns.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2gqesosst.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2utkjtsqd.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2cyxjjpgo.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2txlfrutf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ranpftgz.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2yjueqrzm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2jxnmkgas.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2uumcuisf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2kglkuysq.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2mxxalvoj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2uebndikk.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2imssugmm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2uheqsdok.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2dzxahroa.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2abwnkdyn.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2qwpbdotw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2iclriznl.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2jdwrevda.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2rgildajr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2youthxgr.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2vrfhkowf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2yrspybvt.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2eilzpqih.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2hskxvuvq.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2mtxbbkzp.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2myzhlkcl.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2yqgqsyhz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2utepnriy.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2mnrseuen.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2kaefwpyb.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2kwejntnh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2qbkwggvd.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2tiwrkeui.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2tyshwgvy.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2mwjhrcug.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nuvttoai.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2ryokfnjo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2iogazboj.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2egkztpsl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2emwxiswo.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2pajzfwpr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2ifvfmywz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2aainacqf.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2upghpbsh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nsmulums.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2iadsurcl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2cggvbbcg.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2iuorktyr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2licoyjuq.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2jvlnwzek.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2snfjdxss.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2tbmgcned.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2mabulouy.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2abmcmvrv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2mvhrntgm.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2tpjgdxqs.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ibphzhoy.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2korxcowr.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2cdhsusvn.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2oqeunjka.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2knnznpdz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2okvhljup.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2bwszcqff.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2bjxasrxn.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2hwrjyapt.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2dgdwbhri.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2ikhsjewf.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kjfoazht.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2grdtgnnn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2qikykcig.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2nmrsdfqw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2heengwmd.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2yugmqgdb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fipjkfvd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2pmlwbmxz.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2oybgmpyg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2fmeiuiss.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2pfboxphl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2xvzujtrp.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2cupcpogk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2nlhjsfoh.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2zhwfcrgv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2vqicpuzx.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2agxmvyjy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ccgcxrnp.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2cirwdeww.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rhpeomoz.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2auiwhfeg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rljedokn.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2gvrampwt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ldrltfru.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2ywmuvwqo.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tmhtreaf.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2eijzmvbo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2evnqhizs.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2cqnyesgb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2lpwyecuw.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2nlaixxvu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2jolyrloc.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2vrqoxzbj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2frhgvlxc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sxzjhqid.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2mupfuaxr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2cuxaofwv.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2jsnhxsii.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2qtdiddpw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dsvmtrph.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2mmgabmdq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mfsqdmwy.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2nvwhlifc.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2pwnxaiqq.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2lrlstupb.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2obbmdmqw.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2lhkqgqpz.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2hbtbqjme.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2xvbydbwr.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2eshesogr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2lgvscbiz.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2cfepjxca.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2mqasakvk.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2xsfnwrjn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2uvejzoih.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2yjaklypd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2yjhktgrz.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2dyjmdjig.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2bwwxrivm.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2qfxpvshj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2nahorywh.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zmhoehns.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2rhgedbrg.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2npfzgefd.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2uvikxnme.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2ckxntlye.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2dewviivm.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2fhwbomid.html

esac
来源：http://www.52xcode.cn/Article/details/gt2cvrgpvvr.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2sbjdxoex.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2mhtvxbls.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2vdojnnav.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2taeretjw.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2hetckcob.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2fuzcdbqm.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dqupyeoz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2crnakapg.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2ylglmtux.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2gdxuqbks.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2gcxrtgst.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2eszbyztk.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2meovbmrq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xzcanpui.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2uzpcvwyp.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2hoyiksvs.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2nvviwhco.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2viwwsnec.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2qsgrzdku.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2ccxqxtzh.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2aleyidwa.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2jjdjftan.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2fvclgurx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2rldgkqzk.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ncxveuvu.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2xevnkwra.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2qxogegzl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2vhhxfpbz.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2jantncqp.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2lizdeupy.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2kllmkifa.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2twmtnorj.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2amuyzopm.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2iktmipeu.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2sclytdwx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2xpiseqge.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2nblvwfql.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2aydbhnjw.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2vdmaofyt.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ngdfohec.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2zvsonefo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2qnpjptdz.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2ipietfmb.html


<!-- 参考信息 -->