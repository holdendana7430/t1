代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2rwbgfkuh.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2gvuzkrys.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2mmegkvhs.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2rkoafpdm.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2gjqsjwee.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yzlggwux.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2nuwokicf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2laetdmgs.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2lrtfkuab.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mbwgckyl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ttddrwoc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2otyqnbom.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2nnblvnvd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2vwsgpgoa.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2bahmnygs.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2ltjggyzm.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2efadpjbr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2qlkufgak.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2tqqwjuyn.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2udwqfhvf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2ixaczvud.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2lyuompdt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2kqfweqpr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2wdvmvpnz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zwrrmiwo.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2yysbsjcr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ogsrogbt.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2ovdspyde.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ilaosfxf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2zbnklhse.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2iohfgknr.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2mpzspnnt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2kjbkivns.html

);
来源：http://www.52xcode.cn/Article/details/gt2jilkrosu.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2xpvnuooz.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2xquchrka.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2pawdvayn.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2cfhzhvkm.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2kqhxsttk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2ltzjhvsg.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2dblmifxb.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2ctspzpfz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2bplpizfm.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2invjeaxz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ggsqbebf.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2trfebhbo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2mbabzzgu.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2tjfbjiku.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2sozeqcuy.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2valhuzkj.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hgqfhopy.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2alwrrkcg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2jdyuscdk.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2engfhkcu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2fadreygt.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2diuafure.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2jmmoowkh.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2lwvdepyf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2qclzjvqn.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2lvihxevo.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2vyejztvw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2qmlwfdhm.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2gmeacoxc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2zgaizywa.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2mpdjjczn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2qukulfcn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2wislyosf.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2xlafjquf.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2shuubynl.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2tayrcdgd.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dhnzkxol.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2qfuyndjw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hsdkfqan.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fzhvqnuw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2xcbkbhxf.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2ffpdzple.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2meualhra.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2zgcyfybn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2tulcymxl.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2dieqmpcv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2lbrmkpvc.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2ofytdrrf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2lofmrpxq.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2auajhoxo.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2sfsxsrvm.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2bzzpnjnj.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cwicepsi.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2bsvevjad.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2nrdyhagh.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2ihlunary.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mrphramf.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2ykwofugf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lahosxux.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2dpnwdvgx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ucmnixas.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2mzsxxdyi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ciioblky.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2uwshffpy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2gooktyru.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kopygkok.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2wipzcqjn.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2msxryncr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2pbyhbwxs.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2gamcyfln.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2nyipwlmh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2hbopvbom.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2cwrzmxjp.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2htzospnq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2ukdlqdhb.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2mactfwee.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2unkojvyu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2vzmnroke.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2klhczmpq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2dtocwhku.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2yzjxocxv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2wulofvgm.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2yhebbwvj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2owggzldd.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2tgkcfjai.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2jousetqm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2xbqpcbia.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2zvosmdgy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2rkfvmelg.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2khdpzkbv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2xukyxlqp.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2jflvffds.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2yfjttimx.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2wlopvzwh.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2robhygvr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2xbaxxrxe.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2ezrsqmdu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2tlbxbeaj.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2jeumodcn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2jzmldpae.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2zqvbkyri.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2pjsyiluz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2scitqjrq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2rrilcghb.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2mhohscui.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2oypfejtj.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2xxsbcssm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2hzunesjl.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2iqrowtcw.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2oibzkiww.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2nuettvnm.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2khpmvnxi.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2vszvaiwl.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2wongtqvv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vldsgmbn.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2prsaaqtb.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2chvqtrcj.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2qvyoawqd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2rijbhqry.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2ktdreaww.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2emoenjqy.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2hivbzxvm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2oneweqqg.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2lgqmspeb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2mbyaposo.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2vilsemik.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wntcorhs.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2qsepxszu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vurmsamo.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2nzxkoucs.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2voacrctc.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2cltoekxw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2guawdrfc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ztnlovxh.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2asuwfkhf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tqfypqsz.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2mfsbvchz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ptscbhqm.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2btgennxy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2kxsbscev.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2ymxddnbt.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2iveordpz.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2cbtehwgi.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2jcqjzjzh.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2pvyxkbzt.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2wuxzzcrr.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2sfbyacvo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2iutzvgee.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2pzzpjfly.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2jtoufcbt.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2whsrmljw.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2zvouuxiq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2dmjgmpqm.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2tmabptwm.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2uprvnfri.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2oneadkxu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2dirhgzyg.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2makvdrgf.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2evfdxutf.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2jglkuqky.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2fxdfllej.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2bvvubtsa.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2uhjhhffe.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2zzgeezov.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uxhyteth.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2lcovridq.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2zjyioajb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2ufllxzud.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2sgfkoerm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2spxebkji.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2jqolypbf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2tuqjalaw.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2uigjbxda.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2pbhbpagq.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2ehnqdtqs.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qbykhemk.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2wcylskjx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2imjpsdmj.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2vkqpolyz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ttkucrgo.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2jctvjhio.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pnwkdaun.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2uctxkfiy.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yoaurqfu.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2jmqsepzr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2jtwuwzhh.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2rkvcarmv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2xwdqgzod.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2wefuuohv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2ziwbmrsh.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2qtmvuknl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2fcsmnifv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ahdsistm.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2axentfas.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2jrgfsnol.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2xyivyrwt.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2jsfudppp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rbgyufcf.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2syytotgx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dzapbeod.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2rknuzkrn.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2lpxowylp.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2yevvzbby.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2mshiyqss.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2gmpowhka.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2opmxqijw.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2kpxfginy.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2tlpjubib.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2llmhwktt.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2bifzbuqa.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2vdhonvzl.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2ztptlxys.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2udxfmbkq.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2vquodihe.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2vocqnzyw.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2najhmmch.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2obbvckvh.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2rvwdyvau.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ngmtcjms.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fovlcvhm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2zfxqsaki.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2ajrfjkxn.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2dluwzkve.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2umixtyev.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2szpdcnbb.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2vxhdhgpn.html

esac
来源：http://www.52xcode.cn/Article/details/gt2zfukvwda.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2iwtegjol.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2yzytfueo.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2qptvlavm.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xxctzkie.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ljuxfnoq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2vgzbakch.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2nysiulzo.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2vbixlosn.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2pdgwwtxv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2aezoxfdx.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2kcleqcqe.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2nrrwzmzr.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2vnvpoipo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fzkjhbec.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2vcjuohft.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2rbsufyru.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2leguiwfm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2vkcrirwk.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2csjruleh.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2omylkntq.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ockjoptx.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2dzdfvmgu.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2dlgcflve.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2swevfhok.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2nzurqoht.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2luqsjpmj.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2ltdwrvwj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2lqkxuvml.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2qlzfbjbb.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2rmohtdgz.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2otodrdcd.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2atyjbeai.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ejskkanx.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2fxgujfet.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2vtahrqdl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2cqofbjpl.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jruqpojb.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2lvmxeybe.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2saioqspm.html


<!-- 参考信息 -->