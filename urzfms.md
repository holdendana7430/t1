代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2bzwfjhjr.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mkccatqw.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2pnsysjjd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2mzxcmspl.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2igpjwioo.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tqnqlsod.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2jcpcmqyr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xjsflepz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2sgoncrrw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2beysllfe.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2qproiuhg.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2mwbdpsya.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2gscfxdsn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2cwauyvgo.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2sgcgudqv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2bwpdgbuq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2ekvqirix.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2lhuslvyq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2gzzswoav.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2bogdqcag.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hdkcbzed.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2tqjnooro.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sclpbzqy.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2fchflsox.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2pnilxxdn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2cjbidhiw.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2icabiqhm.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2mekdgngp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2jsiguxjv.html

);
来源：http://www.52xcode.cn/Article/details/gt2igdjvoqv.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2egahbbxk.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2jjxkomnx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2gmwnkzma.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2wradhvsv.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2whqdpfqp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2bggijrpw.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2cwsggccc.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2fwlirwyx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2mbiuwlvp.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2wdqcbnny.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2abcfliob.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2wescvmtn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2fehthhtb.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2hpgxanqr.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2lcouvhzd.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2cjqoblju.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2fcynxjym.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2hyrjjfdv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2cictfrdp.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2csstpccr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2udtdgybm.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2tfklcgps.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2zzrbuyvm.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2kzyfdfwn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2kcuhdycz.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2yfomghyk.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2vkorykew.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2wbibbehj.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2ykobwdau.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2pknloyvc.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2fwcrmweb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2znanvcch.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2wxsuqpqo.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2paoijsar.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nedsrosy.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2qvstblrf.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hlqulmzd.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2plvhthki.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ksvohmjm.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2jcxhjhtt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2ddsjyega.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2boimuzhd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2grufgxhl.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2nlniwghh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jedzdzib.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2xrsfnoyv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2wksarnvo.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2fveldxuy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2rdzkzwil.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2tppvxojv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2qygbyogx.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2mujplaqu.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2okybketd.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2zzehttkg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2abbzpeha.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2jsnoxgdr.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nyvudbnd.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2tvmjagnd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xxztwbij.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2fgklkcwb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hrzopnbp.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2rxzhcepm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ekkldqmc.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2xcedvpsc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ijaebwoc.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2uxgkeltm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2rdykbxmy.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2rihacgyb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2asumymgz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2odduirtk.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2oresurgo.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2qggabjkt.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2jeulqsca.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2sisbasfp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2zdotjohf.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dkeyruej.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2yaqworrc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2jraeevag.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2otsdhwwm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2nmqswgdc.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2ywkylrdm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2qxsxtakc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2vpblsgqf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2fvjraqgo.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2vdtscstp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2plskzkpc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2relcnjfb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2ladxenri.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2srdefsou.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2osmertrn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2xusgoupl.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2hwxzbbme.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2szqrxtkp.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2csigalkp.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2vflabmyy.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2cjwbzfip.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2aqosnzcs.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2twnhqrha.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2mnygppgi.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2envxstdp.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2gjsqpyeo.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2spkozhxk.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2gdfytpxm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2cjgqnybz.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2mamglcza.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2tqvmpedb.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2tufhkqhj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2hyvlvyhm.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2peybvynv.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2bzlsdusl.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2jsprgksz.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2nnzqmsbj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2grcxcsng.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2gxsmktjc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2mdolpiij.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2ycutnbom.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2tavbcdhr.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2rdorlsrt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2gvhvxssk.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2vaufgkrq.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2mxpqkklb.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2tcviikte.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2bnytdqcy.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2xpvpomqf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2wxafiiwq.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2gcosbwyp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lovuljye.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2hnwpfmxo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bdqvhikz.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2cwkmpshq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2flrigxiv.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2peuhqoag.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2dgczsbyg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kzfbcpsk.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2xhoymwuv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ufpzxjxx.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2xnulqlsp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2nqvmpzmr.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2srplnorz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2xipiysgu.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2hgnpujgw.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2jcloimtd.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2zurjonwk.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2mpfvnsqg.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2jobghgsw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2kkiaepxu.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2uxxnrenh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2qhpwswnz.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2lgjnkxtz.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2byndakyt.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2hjklbjzz.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2vozdeguw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2frfmevni.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2xjyjzftr.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2cbivwvnx.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2lnwsxiug.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2uimarnyq.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2iaifjqat.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qramklfg.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2pwfgoblp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2axvjqpcf.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2grkegdsi.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2kbsjlqbb.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2yauwfqkp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zrdmfqvh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2mxmiveph.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2qypgzcsh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2oyzdtlpe.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2rygmwmbt.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2muglzors.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2repihsjc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2ywvxszpc.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2uqysjsxo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2blbvoufg.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2vppurdlc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tmkvqlyj.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2kdrzvhlf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qxjlwkow.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2geihoueb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wadwhqwg.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2yghxdyig.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qedkhlvf.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2sqkkjbwb.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ymhbhxpw.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2dqgfpuev.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2cgmcnvyb.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2uazdfqww.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2fhwzqpmf.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2xoydkaea.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2ctbcyoim.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2vydgqpjc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2bndyxtyd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uhbhollh.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2guyeayee.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2knyucwvt.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2owciswje.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2gxljvoyn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vmbfwpyr.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2akbkddhb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2igdzlzno.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2jbvrupso.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2bxheolfd.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2jhvzosbt.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2esptfzlf.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2xbflpnni.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2imhcveju.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2njtvvwgx.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2wdywmymt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2zvulbyeh.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ngyzfkql.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2kvypxhfd.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2qwxcwvdk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2jnmtfukk.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2muhbchoy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2losxsjmz.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2eyrvxdwv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2xcqtdvtx.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2oeejpejx.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2iaaohoji.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ncnlhffh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2cwbebflc.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2ndbysxjg.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2favyieli.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2kzpahqya.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ffzykvfm.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2blhvhxst.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2ldhhrcuc.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2rmenesdo.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2mhyxanjr.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2alpehfvj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2lmuwaujg.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2wbthbnwq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rwqpqmiy.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ufdkgesb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2parviexh.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2iizqijvl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2soaddibz.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2afpnmlib.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2vmhgosei.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2wwghpmlk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2urgfsiwo.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2gdhpzozi.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2aqzypkbv.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2leyidmcc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2pvawicwm.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2nyyrqjqg.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2ogumuhny.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2asatyytc.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2paedvtox.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2hlekwyko.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2ebsrexhn.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2oxyysyxd.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2pfsdhkrw.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2ftuhkszk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2sluplrgx.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2myxmbbpf.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2lxtjqdln.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2elknvhin.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2wzsvaoxd.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2unblvsot.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2elybwhut.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2fqfgqdzs.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2qithsciw.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2nqoqwruw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2kubjacrx.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2xjdzhbpg.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2qozfrtdk.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2vzqrbmla.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2trzfmskc.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2cpbsrsqg.html


<!-- 参考信息 -->