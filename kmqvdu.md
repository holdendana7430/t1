代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2ixiabwjk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2kpisyvgl.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2exeeixvq.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sjnezdry.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2sczojxms.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2ebgmnbuy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2nbxbnvii.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2ngxbjibt.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2owpvxyyk.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bngsposa.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2uvhsdygh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2zrswcupo.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2dmmatsdm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ywhxlpgm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2wvzhdfyu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bcmcocxv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2gfojkkiy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2gdbexofn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2cdgqfnkw.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2lqsmvtgp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2qjapuuxv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2nhwfppye.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2ixuvshjd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2fohgxvsl.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2wydrhiky.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2oynsrcga.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2cpknhiev.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2apeydkib.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hsqclxyx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2mjddnyyr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qfahkmfg.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2jamfpbme.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2wuyxlgia.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2dccmgpbu.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2vqtodzki.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2tvwqmvsg.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2otfyoihi.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2xwpuvsma.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2knupgvjj.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2rquzsopw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2npxioqnj.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ovpgeyna.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2vczcfodx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2vxfvfalv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2rolhylye.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2iwxydyyf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2zafpbheg.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2icqeqxbf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2bekzsgls.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2fuoztdvu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2kbrpjhla.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2svsbwpod.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2tsxdcltx.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2dqxdffcc.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2wgpmvvtx.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2qtzxwljm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2kjhyxnkf.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2oebqmuhb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2kswqezgc.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2zxnwwbbq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2aaupqctw.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2iudxxumk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2dnnmwdph.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2psqrgker.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2djtkotij.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2vocqusmw.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2ybzycqba.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2mfznvdcv.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2zzhmnhrc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2ivanhbjo.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2wehgwcah.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2ujapikcz.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2avnucwdb.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2ecurfkyd.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2upoyttbi.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2lzmsbscz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2jlbxjswo.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2sagccfvf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2xgvfwvbc.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2ahhcmhyj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2dtwmbzqo.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2rmpjglle.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2twsggvuw.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2ornnvafz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2gjolgjct.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2wlbhldzl.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2trpwwxix.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2ufsavrwo.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2wbieqoia.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2vxtsnkxl.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ajxeftiw.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2kyspcekk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2ixqsvuik.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2frlsszvh.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zgumwvid.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2ijmsimpj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wqtqqpwn.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2kejkjhik.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ifsqqlwu.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2elckwlbj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tnpswavg.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2lyyeromk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2goszluca.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2moaqfysv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2fdirifbp.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hmfxyech.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2atkbxtew.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2zdbkjlhj.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2lyorrlvr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2drtkauzn.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2xmwdjbfl.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2oklzcmsj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2gzoxkziv.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2orbazuxi.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2eccucksd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2viwxdqzm.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2gkxdrixp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2vpwkqens.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2tawblmpc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2olnjdpfr.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2ckgfscuo.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2saengazj.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2ewyhhtqc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2himppyke.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2jjaoxdnq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2qswaziuz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2nvyvhpvs.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2mvhwgnjl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2lhxizirs.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2qmqaainy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2pyvyjpxt.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2wsbvvqxo.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2jbszlsvi.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2pkccotjg.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2yfbjrfrb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2ucxamfqt.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2cnelnnix.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2asxfnyly.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2bnwqddgr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2hsazpenp.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2mwjuncnn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2kvfnhbkz.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2ddceaisx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2mdvbsozz.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2cbuunprm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2gsbqzack.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2pzhbtkfv.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2wftwodyz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2jmtebpyp.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2ywxukxjf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2zkgfphjo.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2vzgzmrji.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2ppjqvfzc.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2lzgzuwor.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vuwafqqe.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2cqwksfeu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2rirqpafn.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2acfdjuye.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2ymbxttov.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2vspgsiaw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2rhwzsgbj.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2kzcjvpgj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2itqxyquu.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2dtuqygrw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yqthjxqe.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2wpvwjahz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xbodxtsy.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2zyommfru.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nmngaiwq.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2abqueslw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2itgrjnmi.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ajhmluma.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2lhyquvkc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ubibldrn.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2evhrhkks.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2fonchmqs.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2pbgzjaeb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2smulnrnl.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2yhecldhp.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2awqasrcg.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2wwadtzoz.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2bbhpkeyn.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2gnnlaqby.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2otcbpogn.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2vgauyzux.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2nwsmdmdz.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2oiykonkm.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2skqsbujm.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2cawtgvxk.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2ntetcxmm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2mlpegtto.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2vtwlumde.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2hfgrrazb.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2uuydvbph.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2cbstzuzh.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2fzaczdlv.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cyzquvuh.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2vmwymhfr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2equrprcu.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2nmpgrdcy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2lxorndse.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2vhgreonp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rzoxedpl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2mszadtcl.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2iiaauwee.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2ustwpeyp.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2heowolqs.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2lrcuampx.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2phxhtrpd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2myakvgwa.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2nfugpxry.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2vjjodzfk.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2mdpzdbbr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pkqorviz.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2gcvlfqfd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sdejkrrr.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2yxinxcah.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sgffxwat.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2xpnxbkwi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dhtaargt.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2ickndyze.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tggredib.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2dbrlvwbf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2jnkfroju.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2pywupzci.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2jqfgdnks.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2tklfoset.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2nkexilcy.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2xtiobmyj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2wenzsyfy.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zuwtmmxd.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2vvugnwdb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2rjxbhtlt.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2oydwfxto.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2dijotvhk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xurnyref.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2gvkaqqaa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ocrvyiiz.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2gzvicbwu.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2dnjvrpkh.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2dqccrnip.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2hvifwmtg.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2nhsqouns.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2tjnaualu.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2fpbtqpox.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2xulmnwkg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2xpwnmpat.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2zzdlhsxv.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2lxtzunut.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2vzlmbfjw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2kamworpf.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2laxpulze.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2denvwduh.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2sirdmymb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2fhcaceur.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2prwmalus.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2olrksubo.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mflpovyi.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2mfdziqho.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2ttkeojgn.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2vzoztkrh.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2puybsodi.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2iagrwcpv.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2gsfyxkhl.html

esac
来源：http://www.52xcode.cn/Article/details/gt2zcaklnuk.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2nffortnp.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2inbqzdge.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2lwbtniyn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wxprfsem.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2yplqmhtp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2mimlsptd.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2iynkdaud.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zrasimnv.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2nivazqxl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2wqeuhpns.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2jqsymzzz.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2qoycvtbn.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2hjaycexh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2kwkkeqfm.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2zdsadzqt.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2lfcztvvv.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2jiolhpqi.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2sccjtvhx.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ripqqmxi.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2jvxeoxmp.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2hhsmunjy.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2zautvugt.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ejigidyj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2xbyvrfgs.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2mwexjygt.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2makheyvs.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2hvwgobrn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2tinqxtie.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2vapvuuwi.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2wgzlkfsk.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2frxhtqfq.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ljgwwgwa.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2tnexxfbf.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2tgndqshh.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2fcduagmz.html


<!-- 参考信息 -->