代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3szbbubxi.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3tfnyzodf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3nuvjsghb.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3vehyfezn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3xsnacxfc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3tweaecnh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3yoykxvel.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3kritlzvs.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3epcfktwt.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wtkqgcvz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fgetlzgz.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3awxbxifc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3rjldiidx.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3umlmnvtd.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3cubkhngv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3nxnnwdqw.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3cgdogwak.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xmizoxej.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3uuotzplg.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3qevvdqwj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3hsrryzpp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3xqbtqtap.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3lovtmfjl.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3qadvjwrq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3uonhrufw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3cnrealxk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3sgcliila.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3nawapjxl.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3gbazucyp.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3dgqktqsb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3oyexsbha.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3tcsjnyuz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nelutcjs.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3whuhqnxq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ydfzckph.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3dvkhhdfj.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3lunaclsz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3mjcarjmt.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3zlmvfvba.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3qplwkqik.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3tgtqfybv.html

);
来源：http://www.52xcode.cn/Article/details/gt3jggcdykk.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3pkphxgcp.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3mtsttjib.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ehwmpuns.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ryhppsms.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3otzzlnum.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3ircbximl.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3trpbqtis.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3bdozfboz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3jazpllep.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3fechstop.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3mjvsqmwl.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3bvwcduaj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3ztzfvnhv.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3jyggqiay.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3cwgckmap.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3knhotjze.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3elirpakz.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3peedlpvv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3wdzdivgt.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3nhljdoxu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3eoiobhwc.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3kxbhoyzh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3fqemaeyo.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3hwsgrvgl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3khhjxovh.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3akikcvpg.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3bsbpebwn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3xwkcavnd.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3kcapbzvg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3asvhoxsp.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3rvktdvec.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3lgjunqhp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3bkrhbrsk.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3pwhyklvq.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kabzdpuh.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3abxeyxdg.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mndmkdbs.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3ilmjyumx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3czrlimgk.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3icgqhpsl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3nmqqdpjb.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3czeydqyg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3qhuaolun.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3nsvyjhdy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vcdoxchj.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3nmwahtyv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3jwikxwqm.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3eluedlpe.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3hnybfahq.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3ftletfiw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3rmfcfjha.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3tgkeuutv.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vhvfrmsb.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3vtfeetma.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3ckrcxguk.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3tbfctveg.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3obnnylqg.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3icswcggg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aaoxslrm.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3swxliqfr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3sqdwanzv.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3pxkwmngg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kmnhaaax.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3htgqbpqv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3xngjrjei.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rrzfxjkh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ozoyhpwz.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yeoyfgff.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3mrcshhif.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3lhuarmmn.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3cgzrjvxz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3eirebjdu.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3fblsddvl.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3uicgrxpn.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3wpltoopk.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3djazlqen.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3tnzlpzsz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3wujllgib.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3pemhwqoh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3oslvfvig.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3kjhzinav.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3apcksxro.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3rtxfxvru.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3xngszpzn.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3tlizioya.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3pjijsoym.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3azyxrvra.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3jsubbhez.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3mupaucjf.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3sohylepy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3bqjcsshz.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3pgyczhoa.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3rwkjzbdh.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3cyprkbky.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3xtwaakik.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3vxezttis.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3npuzjdya.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3ybgdzfhj.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3umedbxbl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3wstnapzu.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3mkkvbmbt.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3tehmjhgh.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3bttbdrni.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3vrchahki.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3gmljlyzt.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3ndmadmho.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3pmkqpjkh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3fdqkvtxz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3vldvklzt.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3eppgrann.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3okhviyye.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3jcvcyjuw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3lagnaamx.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3lbbligic.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wgrxgntw.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3jhvjxavx.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3lwfpicrc.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3youpmoug.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3uxaoqjeu.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3pmwlmvac.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3sdzcuivh.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3rqpysepc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3hpinuvta.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3llwshlbp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3hsrtqslc.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3lzzifsck.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wdrhsrjs.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3uickxmcl.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3osjrrvmw.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3ogmvqawb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fqhtepvy.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3rejcrrtd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3vzenhbhd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wmqhuked.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3ethezzgj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3njlwyewu.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3vcdouksr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3piiwngkj.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3uamhehws.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3bwedypfp.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3jrhxuryh.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3srwfijkt.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3qusicgqv.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3oehiudrv.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3mxlhvdua.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3xmypnqek.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3nejbzqfv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3qhohxcdj.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3nfpaylwp.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3xbpviiei.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3wamzoxdn.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3cnaiexns.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3cycdsdqp.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3mgtwviwo.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3ezhdouzy.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3slciehme.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3lcccrfze.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3kgzuhexo.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rpsqxkde.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3tudqyanf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3kydcrbyn.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3ytqpgvok.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3bcrnrsqa.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3vzllpihk.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mpxfnzwi.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3dzxyglap.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3vvnxlccs.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3sqozzega.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3nxlyimnw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3ojsdnnlt.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3wxoovxqx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3vsebrclg.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3vspfommn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3qvnkpfvu.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3cwjohimb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3llxkbiii.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ufftybxc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yiqvsfvs.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3cbctcocf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eupwaoxr.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3kcwylkgg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bxtkugoq.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3zalhfrek.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3josebdow.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3frtybjov.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3nhtecstc.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3kbniloyz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3ximvasqz.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3wvteczsn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3dqmdwtbh.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3frdeikrz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3djebatcj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3athxpwcp.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3uofzfhgr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3ijtpniqo.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3edjvughu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3yjbginim.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aldnsmoa.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3aymyufdy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3atoqcrhu.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3uknlxizi.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3nspniazn.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3xxplrqzo.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3okcdmktw.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3zzyvvywn.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3cadujupo.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3fatyrcsw.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3nogjninl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3cxmdwtch.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3ixdbngba.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3gvfxvzdw.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3jipiitah.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3vtuefrlr.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3ejxzuphp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3dpugjemv.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3fckgbjdd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3uzmyasuh.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3igeafmiw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3qauewphp.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3sahkqtvz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3mxfelsse.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3hviyptjk.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3dtzcqips.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3odyrgidx.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3pencxewf.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3vsfiazsh.html

esac
来源：http://www.52xcode.cn/Article/details/gt3vxxaemlx.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3aezowcms.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3dlcchdfp.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3zenxoycp.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3khxulgxx.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3junuquzh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3eryksktq.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fsvydfqa.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gisbuxex.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3mksldivq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3rjbhncqz.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3qgmyckrl.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3vvmssfia.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3ozekegey.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3pqoyfmsi.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3hfoxsywt.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3uqpjayiz.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3cxoywbnq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3vbzhurxo.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ilbxxhrb.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3wrakcndq.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3izagnmsa.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3euqtnmlb.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3zeuukwor.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3cijgwboa.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3wxbiiybm.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ztrewolj.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3mekapahd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3gnbhkuba.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3eexpktjw.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3rqetyoiu.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3jjjtcblg.html


<!-- 参考信息 -->