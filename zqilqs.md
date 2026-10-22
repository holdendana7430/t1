代发 wailian999

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2hkufnynv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2oowfpkdw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2zxvycipu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2igtcvrlw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2gpgtmyrc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2epmrivmn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2zyxsffce.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2nzoxjgnx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2qfnaqqqq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2gfushupj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2juyhavhg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2urkyxjbo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2rwgnrtst.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2tjlavqtv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2vtnthboi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2llqfuohc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nkblbuht.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2jqqjnywl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qaelmpsw.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2nqmzdchc.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ylgybutb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2stnnvcvw.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2jhqqbnjk.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2ttdvrusp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2njzbnppj.html

);
来源：http://www.52xcode.cn/Article/details/gt2iaigfytm.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2lyeqjmyy.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2nfbszfdg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2msokmsej.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2kzdxxabo.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2qgxcygvs.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2dbnckbyj.html

);
来源：http://www.52xcode.cn/Article/details/gt2kxpfjebc.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2zihdpcve.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2wmjlztip.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2slrxvkbc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2vcxmuvjz.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2lhrghdur.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2bqxlticp.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2qxcuyaun.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2phdpbsik.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2ebqzzvtj.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2hjnfaaki.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2nfnvtpzo.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2chymunnh.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2rqxihuda.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2jinbcavp.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2dqjksvsg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2fkoewrtr.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2holmedsb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ejiifaly.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2uvfykgkv.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2gmokzvan.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2qfnsejga.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2wmvtkjwk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2dekucvec.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2vqiukqwt.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2ejaqqwfy.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2gsbytnns.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2apoghcnt.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2plxtnwcd.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2lrtopitr.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fyjlcxpv.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2pdoqkwuk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ygaomnjh.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2ewvecmeh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2qjhbmypp.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2jgcfudas.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2tshdymcl.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2lbojepob.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2zpglvvvh.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2vsfviczx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2czjatzfl.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2wkcrtdwb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2fcgknhzn.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2rielshur.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2blvjlihs.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2csvfqlss.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2udiyimpy.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2rhgjbvzk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2jiltdbzy.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2mxuvetxi.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uzgbbeki.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2fxupxupl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lundahmk.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2ffggoqbs.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zcezhgle.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2itwtxkjz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mphupapx.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2nxstnnau.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2efdxoipj.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2phvysxxh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xktauhuv.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2feaowdmo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2pshqhnvy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2sgrcpuhc.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2pvdustkd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2aaafpeni.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2dwtkuonx.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2yhyzwugg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2xmbttzhw.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qtifytcu.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2bqyqizpw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ttxghozs.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2qqxdaxly.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2tkzmulkh.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2igztyvpd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2hjdnzgmk.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2awxfjnwv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2vtxulhhx.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2odzmhrio.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2wfesvgdk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2spfjshhz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2ffcoxdrr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2wqbameej.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2wwjceajl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2fewziwwv.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2hhnmsvdb.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2pdthgrnl.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mvtnpmqr.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2tfexhawn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2ntvkixle.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2gmmetkrr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2kkvkmfzc.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2muvaadkl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2abbuyqae.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2wzzqbmdc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ywmvpxll.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2dzwzwnhr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2cdhugurp.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2choncrya.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2xdbxypzi.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2kjhpiduc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2bbgqktpj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2xdzbmjql.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2vtvdiadi.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ngjtukmc.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2nwyodnpn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2knsidavp.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2nrplrpty.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2rxezgfcb.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2jtibdboe.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2lcqexkty.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2kwjlmqiq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2dxysrxdd.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2pvknnvnj.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2kcfgxymz.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2briuhkzh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2nizbcnac.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2srpqwglc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2fbenhhsp.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2ogxgqwfh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uqbhrjho.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2vvwelnip.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vavsuegs.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2xwakaudx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lmrbddaz.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2nbhwdzvs.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2eqellxmy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uzscpoig.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2cwftrjid.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uoraabcs.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2fnbvwnfr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2bgfssyxe.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2ftqlsfrw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2jinfxhrp.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2modslmkc.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2odgfewhq.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2ngkbofwz.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2xoyqxerx.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2zcuvomkb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2jcxuydzc.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2pzcgbfjt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2lylflleq.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2nvptwayn.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2tqiarboe.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2wxqnlfad.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2zshfatmg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2jwfttqex.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2auhfykly.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2asizrqkx.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2xuyazeca.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2ufmbamkq.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2idoyeeta.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lktfgpip.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2eolwmxea.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2btgrzyuo.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2knuqbthq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2hizlbsrc.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2yuuaoxwt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2alagkvrv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2gclqumgk.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2ldqebbye.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2nfwjqljt.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2uhdzgzjp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2ktqsnzse.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2eosskqml.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2bdgshqza.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2fbjwzicv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2pebatdwx.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2dedrjmbl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fnglakug.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2icderkom.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jebacrco.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2qsppukkq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fosajqjc.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2qoghafad.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qhsxrcqb.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2mdquwshr.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iliibskw.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2rlwtinyf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2bgoayrxw.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2htquxkic.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2mkylfqhj.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2agcedgto.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2oqpxjjzj.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2bejvvctc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2iekascep.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iftzrihv.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2gevjmlmi.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2cclpztzb.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2dxqxzhpe.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2jakjhgdu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2afcuvlya.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2xyvrewrp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ewlvgata.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ohwzkatr.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2oxgtmgio.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2idbmuokb.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2yifacvew.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2fyfguugj.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2avbetfze.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2lclmdlwy.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2qfzzkhgg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2vgirjzep.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2ttlspzit.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2wzuoawvi.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2inxucatz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2xugikxml.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2jgosgrlb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ddgmfpdw.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2okzpalud.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2xwnscoks.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2rbasxzji.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xbyhmdxu.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rezbzxft.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2pjvqhcfg.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2vjqbihbb.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2csqyvqyg.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2zqexwbqi.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2zeioopek.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ndhsvwnh.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2smnnzkml.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2qgspvivk.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2uncudfxj.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2drxwoqtd.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jdqquivv.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2yjlevvxu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2skvvtvdj.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2aapauqkb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2qpvpdyqq.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2dwyahqsn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2mspbnnaz.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2pfqeppec.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2pxfxkogr.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2qglakvxo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2onscvlcm.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2iurpinrz.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2fbkyetpe.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2zzpoujxn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2hwuzjuky.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2coijqqxy.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2utxzwwfe.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2uqcnhohi.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2vcotittj.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2bjaxmzia.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2gqwqndlw.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2fopsvzts.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2bonqnekh.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2blkjhvzv.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2xnvkhcjw.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2yjoiigjk.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2dfliixsu.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2jxjnobfw.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2badoqwqs.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2nnnygumn.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2egcpsvxy.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ymxuxwob.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2aespgwch.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2uoybboyj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2bgfvcbum.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2pypktutg.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2udvwlsjj.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2uhhtdlvv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2jzyvtxxs.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2rlkmzkxf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2bbbkepbd.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2gwclwywm.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2dulwzish.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2hgzcasbj.html


<!-- 参考信息 -->