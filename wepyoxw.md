代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.zdbjq.cn/Article/details/gfbcjagcv.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/ginxvbgtl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gwowhdwvi.sHtML

Go:   if x == nil {}
来源：http://baike.fehbvm.com/Article/details/gdncvclih.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fehbvm.com/Article/details/ggxrifbss.sHtML

C#:   if (x is null) {}
来源：http://www.share.hesvh.cn/Article/details/ghwncxhfj.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/goofbmqfb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fehbvm.com/Article/details/gybmcpegc.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.hesvh.cn/Article/details/gwobzpilu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gyggqergj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gohdyiien.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.zdbjq.cn/Article/details/gozdyrhpr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.hesvh.cn/Article/details/gavwnzece.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/gmbukefnh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/gbvdmqobt.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fehbvm.com/Article/details/gcyzciegw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fehbvm.com/Article/details/grshieglr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.zdbjq.cn/Article/details/gvomgnifz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/gvvgiiryi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gbrnkvwrw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/gginwixuj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fehbvm.com/Article/details/gdchyhmri.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fehbvm.com/Article/details/gfqhshmto.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fehbvm.com/Article/details/gklglidpp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/givtsilqc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.hesvh.cn/Article/details/gwyoonjzx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gharuoozw.sHtML

[Q01] 创建表
来源：http://baike.zdbjq.cn/Article/details/gmrfzbyvy.sHtML

CREATE TABLE users (
来源：http://3g.hesvh.cn/Article/details/gudqxbxzg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gyugfqcvf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/glbfnpkbq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fehbvm.com/Article/details/gjkqagoyg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/grwjfgeqo.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gmrdluhzw.sHtML

[Q02] 创建带外键的表
来源：http://baike.fehbvm.com/Article/details/gftweyakg.sHtML

CREATE TABLE orders (
来源：http://blog.zdbjq.cn/Article/details/gamrmxqvb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gkmfauqrc.sHtML

user_id INT NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gzqxriuoh.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/gbbenfffi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.zdbjq.cn/Article/details/gdqkbgdsu.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gwqqkycvh.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/gtaenghmu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.hesvh.cn/Article/details/gdaztauaz.sHtML

[Q04] 修改列类型
来源：http://3g.zdbjq.cn/Article/details/ghiuuxjum.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.zdbjq.cn/Article/details/gpgkqjgan.sHtML

[Q05] 重命名列
来源：http://wap.hesvh.cn/Article/details/gsuoaqwrw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fehbvm.com/Article/details/ggausfutl.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/gpwnwkrig.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/gbtcbpdma.sHtML

[Q07] 删除表
来源：http://www.blog.zdbjq.cn/Article/details/gibyketwc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.zdbjq.cn/Article/details/grigikylg.sHtML

[Q08] 创建普通索引
来源：http://mobile.zdbjq.cn/Article/details/gokascdab.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gexvpvoki.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/guqfxkprp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gzgqwtsuf.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/gmpokhjzx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gtikapoxt.sHtML

[Q11] 一次插入多行
来源：http://wap.fehbvm.com/Article/details/gdbpvxico.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fehbvm.com/Article/details/gwpubtpqb.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fehbvm.com/Article/details/gfnfpbijf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fehbvm.com/Article/details/gafwkbdkj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.zdbjq.cn/Article/details/gmgurgdja.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/grbuecrqg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fehbvm.com/Article/details/ggekxplsc.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.hesvh.cn/Article/details/gywgdtfds.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fehbvm.com/Article/details/gplqkqtgk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/ghuikekmp.sHtML

[Q15] 查询全部
来源：http://mobile.zdbjq.cn/Article/details/gqtgjflfb.sHtML

SELECT * FROM users;
来源：http://baike.fehbvm.com/Article/details/gzoxxvqbq.sHtML

[Q16] 查询指定列
来源：http://read.share.fehbvm.com/Article/details/geflxxrmv.sHtML

SELECT id, name FROM users;
来源：http://blog.zdbjq.cn/Article/details/gdwmrkgxt.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/gkxufceqt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.hesvh.cn/Article/details/gtopyrqqy.sHtML

[Q18] 模糊匹配
来源：http://mobile.zdbjq.cn/Article/details/gtrynfjhz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.hesvh.cn/Article/details/gwuuhwgwm.sHtML

[Q19] 范围查询
来源：http://www.share.zdbjq.cn/Article/details/ghijzlers.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.zdbjq.cn/Article/details/gdoyztora.sHtML

[Q20] IN 列表
来源：http://m.share.fehbvm.com/Article/details/gzktgkone.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.hesvh.cn/Article/details/gxzdzkmfa.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/goczdfyqw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.hesvh.cn/Article/details/gwbocybzw.sHtML

[Q22] 排序
来源：http://www.m.share.fehbvm.com/Article/details/gjfupyihr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fehbvm.com/Article/details/gvxlkbhew.sHtML

[Q23] 分页
来源：http://wap.fehbvm.com/Article/details/gwhzwyctf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.zdbjq.cn/Article/details/gbsxokvwo.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/gqxbmdwtb.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.hesvh.cn/Article/details/gsiwkvram.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.zdbjq.cn/Article/details/gooiajhul.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.hesvh.cn/Article/details/ghyoejyyu.sHtML

[Q26] 计数
来源：http://mobile.zdbjq.cn/Article/details/gpopmddhk.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gbykweile.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/glospxmma.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/giitrlyjt.sHtML

[Q28] 求和与平均
来源：http://www.share.hesvh.cn/Article/details/gkjhalozu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gonxlfvsi.sHtML

[Q29] 最大最小值
来源：http://mobile.fehbvm.com/Article/details/glelaktpo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gzxsdwmaw.sHtML

[Q30] 分组统计
来源：http://wap.fehbvm.com/Article/details/gnubuqlwz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gszgzubls.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/gjsapdoek.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.zdbjq.cn/Article/details/ghutetmwc.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fehbvm.com/Article/details/gfaotxvmc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gxkcilbme.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.hesvh.cn/Article/details/gbcbztdhv.sHtML

[Q33] 多列分组
来源：http://www.blog.zdbjq.cn/Article/details/gvdmncbjk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.zdbjq.cn/Article/details/gmvzasnkr.sHtML

[Q34] 每组取第一条
来源：http://mobile.zdbjq.cn/Article/details/gqejmgjvc.sHtML

SELECT * FROM (
来源：http://3g.zdbjq.cn/Article/details/gekepjeof.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fehbvm.com/Article/details/gshrcpcgh.sHtML

) t WHERE rn = 1;
来源：http://read.share.hesvh.cn/Article/details/gnvgzuypi.sHtML

[Q35] 内连接
来源：http://blog.hesvh.cn/Article/details/gxrgrcbyw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/grsehllvo.sHtML

[Q36] 左连接
来源：http://www.blog.zdbjq.cn/Article/details/gajvyrtwu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gduwulmzc.sHtML

[Q37] 右连接
来源：http://read.share.hesvh.cn/Article/details/geovohcnf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.zdbjq.cn/Article/details/gllcklurw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.zdbjq.cn/Article/details/ghfzuvpmp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fehbvm.com/Article/details/gtmvpqxji.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fehbvm.com/Article/details/gapdgrktw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fehbvm.com/Article/details/gtvalnibg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.zdbjq.cn/Article/details/gpoinvsme.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fehbvm.com/Article/details/glfocfzed.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fehbvm.com/Article/details/gjgovhkdg.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/ghlerwskp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.zdbjq.cn/Article/details/gubhsgqdn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fehbvm.com/Article/details/gdsrvfybx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.hesvh.cn/Article/details/gylagcneq.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.zdbjq.cn/Article/details/ggzwxiznz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.hesvh.cn/Article/details/gkpddoyal.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.zdbjq.cn/Article/details/gnweywsmt.sHtML

[Q43] 标量子查询
来源：http://www.share.fehbvm.com/Article/details/gtepqbawd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/gvatpmusa.sHtML

[Q44] IN 子查询
来源：http://baike.hesvh.cn/Article/details/gvsrloboq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/gokenjwqo.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fehbvm.com/Article/details/glgiysckp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gqhaojesa.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/gaxjlkxky.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/goawmiwvo.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fehbvm.com/Article/details/givxniftw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.zdbjq.cn/Article/details/gpjezdnui.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.zdbjq.cn/Article/details/gijcfmwon.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.zdbjq.cn/Article/details/gdxbmiddh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.hesvh.cn/Article/details/gnhbsylxd.sHtML

[Q49] 更新单行
来源：http://baike.fehbvm.com/Article/details/gvokhsqtg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gxtdefwxc.sHtML

[Q50] 批量更新
来源：http://3g.hesvh.cn/Article/details/gsxuzajab.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fehbvm.com/Article/details/gnulyulnb.sHtML

[Q51] 用子查询更新
来源：http://baike.fehbvm.com/Article/details/gwzofqamu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gmupagiqo.sHtML

[Q52] 删除指定行
来源：http://www.m.share.hesvh.cn/Article/details/gqampftco.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gvdzivobe.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/gxodnfjgg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gtgcskhit.sHtML

[Q54] 清空表
来源：http://m.share.hesvh.cn/Article/details/gvhloqwft.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.zdbjq.cn/Article/details/gjzjoshav.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fehbvm.com/Article/details/guqrsuzke.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.hesvh.cn/Article/details/grselamak.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.hesvh.cn/Article/details/gmxinvnod.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gypgkabut.sHtML

[Q57] 行号
来源：http://3g.hesvh.cn/Article/details/gmuzcpvmh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gnyggbjyt.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gryolktbk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gzdgveiqw.sHtML

[Q59] 分组内累计
来源：http://baike.hesvh.cn/Article/details/guacfjkpo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gklbypily.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.zdbjq.cn/Article/details/gilkzywff.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/givrgdrvc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gtxqajrgj.sHtML

[Q61] 移动平均
来源：http://mobile.fehbvm.com/Article/details/gwlgnfqza.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gdiofafbo.sHtML

[Q62] 分组占比
来源：http://mobile.zdbjq.cn/Article/details/gvmlazewj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gviewhmhj.sHtML

[Q63] 开启事务
来源：http://www.blog.fehbvm.com/Article/details/gzvksixnk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/gtvzrbsok.sHtML

[Q64] 提交事务
来源：http://blog.zdbjq.cn/Article/details/gokzrjojc.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/gnkpexuic.sHtML

[Q65] 回滚事务
来源：http://baike.zdbjq.cn/Article/details/genpzreka.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/gewnxybvt.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/guwotqstk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fehbvm.com/Article/details/gwwgmsodc.sHtML

[Q67] 设置隔离级别
来源：http://read.share.hesvh.cn/Article/details/gjrqwhoru.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fehbvm.com/Article/details/gvksfahbt.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/gfmuellnu.sHtML

SAVEPOINT sp1;
来源：http://read.share.hesvh.cn/Article/details/gfqyjkzuf.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/gyxfveizt.sHtML

[Q69] 查看执行计划
来源：http://m.share.zdbjq.cn/Article/details/gtlkviuqe.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/gynaattcg.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/giopgnmjh.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/gyifuoskc.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/gkbeqpisb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/goniogzmg.sHtML

[Q72] 查看索引
来源：http://read.share.hesvh.cn/Article/details/glmhcrqlo.sHtML

SHOW INDEX FROM users;
来源：http://baike.hesvh.cn/Article/details/gscedztug.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gvsxjovzi.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gmqfsuwko.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/gccogysrz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.zdbjq.cn/Article/details/grphydvva.sHtML

[Q75] 日期格式化
来源：http://blog.fehbvm.com/Article/details/geledlvuv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/goxiblzvy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/gmtycfpcg.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/gsvewnoyt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fehbvm.com/Article/details/gablkhkrb.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/gfkbhpqfp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fehbvm.com/Article/details/gaduslyjd.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gyfropqcr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fehbvm.com/Article/details/gxeyykkod.sHtML

[Q79] 字符串拼接
来源：http://blog.hesvh.cn/Article/details/ghnoxhbyc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.zdbjq.cn/Article/details/gqmqyyuye.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/ggedpotwn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gaaksdhcf.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gianqntso.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.hesvh.cn/Article/details/gxucuinky.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fehbvm.com/Article/details/gzlryptzm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gozznvzpp.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gxpooyrhz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/grcextepg.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/glynwwhpu.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gpdvxbyyr.sHtML

[Q85] 数值取整
来源：http://mobile.zdbjq.cn/Article/details/gibwibndu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/gnucmkexb.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/gvhlkkrjk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/ggizzumwb.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/gtaqutlkw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.hesvh.cn/Article/details/guosqztxk.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.zdbjq.cn/Article/details/genrhiegp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/gdycpbjep.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.zdbjq.cn/Article/details/geqfnlohc.sHtML

[Q89] 判断表是否存在
来源：http://blog.fehbvm.com/Article/details/grtrdokvl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.zdbjq.cn/Article/details/gkdxtqbzk.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/gotzbfjcm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/gpfyzjisl.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/guuixpdky.sHtML

R. Bash 专题
来源：http://mobile.zdbjq.cn/Article/details/gdozgfqqh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gnludvkci.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/gsqeqgezq.sHtML

#!/usr/bin/env bash
来源：http://baike.zdbjq.cn/Article/details/gstsskpba.sHtML

set -euo pipefail
来源：http://m.share.zdbjq.cn/Article/details/gdrdhvwfm.sHtML

[R02] 变量赋值与使用
来源：http://blog.zdbjq.cn/Article/details/gmytwopkm.sHtML

name="Tom"; echo "$name"
来源：http://wap.fehbvm.com/Article/details/gnuicxqvk.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/ggwdekrud.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/gzpnkmbri.sHtML

[R04] 位置参数
来源：http://www.blog.zdbjq.cn/Article/details/gttnmcgcs.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.hesvh.cn/Article/details/gkmxfvgmj.sHtML

[R05] 参数默认值
来源：http://blog.zdbjq.cn/Article/details/ggkvhjmng.sHtML

name="${1:-default}"
来源：http://3g.hesvh.cn/Article/details/gjxhwqjvl.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/gzdrlfqgi.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gfdhiufdl.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/gqzlzqlea.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/gbbyuchdx.sHtML

[R08] 数值比较
来源：http://www.blog.fehbvm.com/Article/details/gbgqrjqcj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fehbvm.com/Article/details/ghvriclmw.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gegxofvam.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.hesvh.cn/Article/details/gzmwaafdk.sHtML

[R10] 正则匹配
来源：http://www.m.share.hesvh.cn/Article/details/gytfszbdi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.hesvh.cn/Article/details/gnlknwrsn.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/gxaggfrku.sHtML

case "$1" in
来源：http://baike.fehbvm.com/Article/details/gxnpifqrg.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/gljedmkxg.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gpqwmwlnr.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fehbvm.com/Article/details/gzftpqsky.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/gfwmeeola.sHtML

[R12] for 遍历文件
来源：http://3g.zdbjq.cn/Article/details/gxwokmhzd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.hesvh.cn/Article/details/gtadsyikj.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gdeiergeu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/grhtyjpdf.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/gykvwgvrq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gdelvbcsd.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gdjbobzjx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.zdbjq.cn/Article/details/gzccqtmze.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/goyxyodty.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gnexdkqpg.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/gmtqrnzzo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fehbvm.com/Article/details/gpyvungzm.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/gevoptokt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/gvyitwtud.sHtML

[R19] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gdnqqdwcn.sHtML

echo "${#arr[@]}"
来源：http://m.share.zdbjq.cn/Article/details/ggjtkbxsb.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/gbvobjuef.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fehbvm.com/Article/details/gczlkwctg.sHtML

[R21] 字符串长度
来源：http://3g.fehbvm.com/Article/details/gcbdkeygp.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/gzvtzupjz.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/geirhfjmg.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/gmahzzfuk.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gsrxwhtop.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/gmmbypoyd.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gdsvxzcov.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/gduwnmebu.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.hesvh.cn/Article/details/gjtipoyxk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fehbvm.com/Article/details/giwashgcq.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/gxbwoojdp.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/guoblblst.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gjefmamvr.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/gluyntxxw.sHtML

[R28] 浮点运算
来源：http://read.share.hesvh.cn/Article/details/gjskjrjhh.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/gccxsbtzd.sHtML

[R29] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gcqoxxjbf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/guapdxsit.sHtML

[R30] 函数返回状态码
来源：http://wap.zdbjq.cn/Article/details/gwxryxhgq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fehbvm.com/Article/details/gdtlnmnzk.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/gwoxlzwnc.sHtML


<!-- 参考信息 -->