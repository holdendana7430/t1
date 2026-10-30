代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.zdbjq.cn/Article/details/gjldxgnmu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.zdbjq.cn/Article/details/gouklxzmx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.zdbjq.cn/Article/details/gduzlvumu.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.hesvh.cn/Article/details/gsxmsygtv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.zdbjq.cn/Article/details/gqkpzkuqq.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/gakxdtxoh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/ghsjkdnjf.sHtML

Go:   if x == nil {}
来源：http://blog.zdbjq.cn/Article/details/gvfnheubf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/gznnykkxl.sHtML

C#:   if (x is null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gfavmyquu.sHtML

[P07] 防抖与节流
来源：http://www.blog.zdbjq.cn/Article/details/ghogdenod.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.hesvh.cn/Article/details/gxutxcclb.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/gagtdohvu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gyluaeycf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gslbrjpdf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.hesvh.cn/Article/details/glqoqtykq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.zdbjq.cn/Article/details/gkajnedhg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fehbvm.com/Article/details/gwvepdjtm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fehbvm.com/Article/details/gencyrpol.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.zdbjq.cn/Article/details/gbijiadrs.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.zdbjq.cn/Article/details/gbquczqcq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.hesvh.cn/Article/details/goruawcng.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.zdbjq.cn/Article/details/gjppdykxk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/gexpbkopj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/glrxvfyaf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fehbvm.com/Article/details/gsseeozzi.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.hesvh.cn/Article/details/gzrfvwdfn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.hesvh.cn/Article/details/glqwansbs.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gsafrvcvx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.zdbjq.cn/Article/details/gibwtpapq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzyxsubvy.sHtML

[Q01] 创建表
来源：http://baike.zdbjq.cn/Article/details/gigjbjzyf.sHtML

CREATE TABLE users (
来源：http://3g.hesvh.cn/Article/details/gvfmjokij.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gkkifvjkt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gmlhcixvg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fehbvm.com/Article/details/gflwazdnb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.hesvh.cn/Article/details/gnztzvdff.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gcdzrltpe.sHtML

[Q02] 创建带外键的表
来源：http://3g.zdbjq.cn/Article/details/gskrvtxth.sHtML

CREATE TABLE orders (
来源：http://wap.fehbvm.com/Article/details/gzyucqhir.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/glscutglh.sHtML

user_id INT NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gjrziccra.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.hesvh.cn/Article/details/gngoljhwb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.hesvh.cn/Article/details/gzxlczwfg.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gmturhaxk.sHtML

[Q03] 增加列
来源：http://baike.hesvh.cn/Article/details/gvirkfidw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.hesvh.cn/Article/details/gkdbmxues.sHtML

[Q04] 修改列类型
来源：http://blog.hesvh.cn/Article/details/gedfttwve.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gkmdsmcho.sHtML

[Q05] 重命名列
来源：http://m.share.hesvh.cn/Article/details/gnmhllbmc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.zdbjq.cn/Article/details/gsctdnudx.sHtML

[Q06] 删除列
来源：http://www.m.share.hesvh.cn/Article/details/gfnusxkjn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.hesvh.cn/Article/details/gqecplczl.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/giijiexmk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/gmjuexssh.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/gjjhrqotb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gxrspngup.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/gbiujsejl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gvkahlquv.sHtML

[Q10] 插入单行
来源：http://www.m.share.hesvh.cn/Article/details/gcphfjozr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gasbwwgkl.sHtML

[Q11] 一次插入多行
来源：http://www.share.zdbjq.cn/Article/details/godxsajhw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gafjgchhn.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.hesvh.cn/Article/details/gvbgdcvbt.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fehbvm.com/Article/details/gmxckorlo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.zdbjq.cn/Article/details/gortbcyus.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fehbvm.com/Article/details/gvhopwirm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.zdbjq.cn/Article/details/glelzjcnz.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.hesvh.cn/Article/details/gisjbpirx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fehbvm.com/Article/details/gtoungpul.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.hesvh.cn/Article/details/gvmqyymtv.sHtML

[Q15] 查询全部
来源：http://wap.fehbvm.com/Article/details/gyoqwyhge.sHtML

SELECT * FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gwtpcmber.sHtML

[Q16] 查询指定列
来源：http://read.share.zdbjq.cn/Article/details/gkneojuow.sHtML

SELECT id, name FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gztxqvdfy.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/ggsvohqth.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gyoaeqbrg.sHtML

[Q18] 模糊匹配
来源：http://3g.fehbvm.com/Article/details/gulpvarez.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.zdbjq.cn/Article/details/gtsctbltq.sHtML

[Q19] 范围查询
来源：http://m.share.hesvh.cn/Article/details/gxbutqbmn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.hesvh.cn/Article/details/guhscnxap.sHtML

[Q20] IN 列表
来源：http://3g.fehbvm.com/Article/details/gcovxweir.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fehbvm.com/Article/details/ghvlzwzok.sHtML

[Q21] 空值判断
来源：http://www.blog.hesvh.cn/Article/details/gsfuboxnc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gbfrlruru.sHtML

[Q22] 排序
来源：http://baike.zdbjq.cn/Article/details/gvdyafmoy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.hesvh.cn/Article/details/gelicobzh.sHtML

[Q23] 分页
来源：http://mobile.hesvh.cn/Article/details/gdammozoq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.zdbjq.cn/Article/details/giazygkkk.sHtML

[Q24] 去重
来源：http://mobile.hesvh.cn/Article/details/ghayvzomd.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fehbvm.com/Article/details/gaycquvww.sHtML

[Q25] 只取前 N 条
来源：http://read.share.hesvh.cn/Article/details/gbfcqotdm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/gtcxvxucj.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/gjqcuyivc.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.hesvh.cn/Article/details/gkuezkecr.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/gozabonli.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ggllfkrue.sHtML

[Q28] 求和与平均
来源：http://www.m.share.zdbjq.cn/Article/details/gnlmmbhjz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gdrojxtnx.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gfjsigpke.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/ggbxkediy.sHtML

[Q30] 分组统计
来源：http://www.share.zdbjq.cn/Article/details/ggvevmdhm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/ghuaweugc.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/gunsltqxj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.zdbjq.cn/Article/details/gaetekczn.sHtML

[Q32] 分组拼接字符串
来源：http://wap.hesvh.cn/Article/details/gyuslsjbv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gmqhosbzl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/gejhmontk.sHtML

[Q33] 多列分组
来源：http://mobile.hesvh.cn/Article/details/gkehmsugy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.hesvh.cn/Article/details/gmwrmrhaa.sHtML

[Q34] 每组取第一条
来源：http://baike.fehbvm.com/Article/details/gkvqwemrn.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gwkzhjrdp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.hesvh.cn/Article/details/gkqauwmfi.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/gesnsesun.sHtML

[Q35] 内连接
来源：http://www.blog.hesvh.cn/Article/details/gzsysjxue.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gpwaxxqzd.sHtML

[Q36] 左连接
来源：http://blog.hesvh.cn/Article/details/gapmaqkzc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gjolezxso.sHtML

[Q37] 右连接
来源：http://blog.fehbvm.com/Article/details/gjfaicurx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.zdbjq.cn/Article/details/gntlmvhia.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.hesvh.cn/Article/details/gbscxowgh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/gebtsdogf.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.hesvh.cn/Article/details/gyhhsuscj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/gmhiddscu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.zdbjq.cn/Article/details/gapuzqxcm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.hesvh.cn/Article/details/ghyzheqze.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.zdbjq.cn/Article/details/ggwaywpeb.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/gadgtqfhk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fehbvm.com/Article/details/giragphpg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/goqxoaaqg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.zdbjq.cn/Article/details/gdkwbkuhr.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/gqvwhelnh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.hesvh.cn/Article/details/gqeryntyn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.zdbjq.cn/Article/details/gahidifxi.sHtML

[Q43] 标量子查询
来源：http://www.blog.fehbvm.com/Article/details/gvtfdwoth.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.zdbjq.cn/Article/details/gfmezbzwd.sHtML

[Q44] IN 子查询
来源：http://m.share.hesvh.cn/Article/details/gmszcemaz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fehbvm.com/Article/details/gagnulzrz.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.hesvh.cn/Article/details/glcepltpe.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gmmwqvbdc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.zdbjq.cn/Article/details/gkbwblpbl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gmwunjytz.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gxshmmfrg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fehbvm.com/Article/details/gkjqbmxaw.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/gyzmfqukl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/gtfwepjdn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.hesvh.cn/Article/details/glalhsmit.sHtML

[Q49] 更新单行
来源：http://www.m.share.zdbjq.cn/Article/details/gekianpfn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/genpmgnrs.sHtML

[Q50] 批量更新
来源：http://m.share.zdbjq.cn/Article/details/gunyaefxc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/genszybqt.sHtML

[Q51] 用子查询更新
来源：http://www.share.fehbvm.com/Article/details/gurpaxebb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.hesvh.cn/Article/details/gqhyesakd.sHtML

[Q52] 删除指定行
来源：http://mobile.zdbjq.cn/Article/details/gwumkwhau.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gmgmdzdtj.sHtML

[Q53] 按条件删除
来源：http://blog.fehbvm.com/Article/details/ghehmgrxd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gffhmkhym.sHtML

[Q54] 清空表
来源：http://m.share.zdbjq.cn/Article/details/gzghztjvp.sHtML

TRUNCATE TABLE logs;
来源：http://wap.zdbjq.cn/Article/details/glgybhdwj.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/gukckbgro.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/ghzzljodq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.hesvh.cn/Article/details/gcdycytyd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gifokmowf.sHtML

[Q57] 行号
来源：http://www.blog.zdbjq.cn/Article/details/getzdpcti.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.hesvh.cn/Article/details/gtisjwfxp.sHtML

[Q58] 累计求和
来源：http://3g.hesvh.cn/Article/details/geqekusda.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.hesvh.cn/Article/details/gfezbwnkl.sHtML

[Q59] 分组内累计
来源：http://wap.hesvh.cn/Article/details/gxyziojtc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gytiscckb.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.hesvh.cn/Article/details/gjcagkutd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/gueiolyyc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/guodsdmgq.sHtML

[Q61] 移动平均
来源：http://3g.fehbvm.com/Article/details/gnfvtsary.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gpvasgbwy.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/gggjbrnsv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gzuabecbv.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/gfiygrmei.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/gtjpiqrom.sHtML

[Q64] 提交事务
来源：http://www.share.hesvh.cn/Article/details/gygrdpprg.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/ghnjrcfbs.sHtML

[Q65] 回滚事务
来源：http://read.share.hesvh.cn/Article/details/gvdvvrdhi.sHtML

ROLLBACK;
来源：http://read.share.fehbvm.com/Article/details/gkjovokjy.sHtML

[Q66] 行锁查询
来源：http://mobile.fehbvm.com/Article/details/gtkxwrapv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.zdbjq.cn/Article/details/gogrsjhnf.sHtML

[Q67] 设置隔离级别
来源：http://read.share.zdbjq.cn/Article/details/gzoaamicx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.hesvh.cn/Article/details/guzdzator.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/grsvxbzem.sHtML

SAVEPOINT sp1;
来源：http://www.share.zdbjq.cn/Article/details/gzraskdkr.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fehbvm.com/Article/details/gcajoddlj.sHtML

[Q69] 查看执行计划
来源：http://baike.hesvh.cn/Article/details/gplrwagpe.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/gzpfzymol.sHtML

[Q70] 更新统计信息
来源：http://read.share.zdbjq.cn/Article/details/gmtdrlzxl.sHtML

ANALYZE TABLE users;
来源：http://baike.zdbjq.cn/Article/details/gwuibzkwe.sHtML

[Q71] 查看建表语句
来源：http://read.share.hesvh.cn/Article/details/gvopulqhv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.hesvh.cn/Article/details/gfystpfie.sHtML

[Q72] 查看索引
来源：http://wap.hesvh.cn/Article/details/gjmxrjuql.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/gmmtfkpoi.sHtML

[Q73] 查看表状态
来源：http://3g.hesvh.cn/Article/details/gzryoefgh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fehbvm.com/Article/details/gerxcxciw.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/gfjbgdjof.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/gibmzxayb.sHtML

[Q75] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gsqzkytay.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gvxvlguhr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.zdbjq.cn/Article/details/gonnjbxhs.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/gcivtwnml.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/giuvtkpix.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/gqsyakbhq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/gkgexdtic.sHtML

[Q78] 当前时间
来源：http://blog.fehbvm.com/Article/details/ghtpaxvgc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.hesvh.cn/Article/details/gqzteenpn.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/giotjyusf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/gnexhrzvc.sHtML

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/gdyhqhesa.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ggfpjipmw.sHtML

[Q81] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gpyosrupn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fehbvm.com/Article/details/gynubgmlu.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/gidnbzawq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gvpngythf.sHtML

[Q83] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gyarnksth.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gvrrcvgmd.sHtML

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/glfhmdlnt.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gyfzjcppe.sHtML

[Q85] 数值取整
来源：http://www.m.share.fehbvm.com/Article/details/gltihmrry.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/greyzqbsb.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/gyishesqf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fehbvm.com/Article/details/gsrarnhrh.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/gtulmwgrf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/gxeehdfsw.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.zdbjq.cn/Article/details/gvsaplfux.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.hesvh.cn/Article/details/ggypjwxcn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/gxutqbsrw.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fehbvm.com/Article/details/gcikctxoi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.hesvh.cn/Article/details/gufvvjznf.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/gsoqtnrgq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fehbvm.com/Article/details/gnrfwmvwm.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gaqeozyoo.sHtML

R. Bash 专题
来源：http://3g.zdbjq.cn/Article/details/gwjdlxnrq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gsqykssrp.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/gdvtwpiht.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/ggxfhppfb.sHtML

set -euo pipefail
来源：http://mobile.zdbjq.cn/Article/details/gixblovnu.sHtML

[R02] 变量赋值与使用
来源：http://www.share.hesvh.cn/Article/details/ghokwqhjp.sHtML

name="Tom"; echo "$name"
来源：http://www.share.zdbjq.cn/Article/details/gmpujmffx.sHtML

[R03] 只读变量
来源：http://wap.hesvh.cn/Article/details/gvdiidkuc.sHtML

readonly PI=3.14
来源：http://wap.hesvh.cn/Article/details/ggktcojms.sHtML

[R04] 位置参数
来源：http://www.share.hesvh.cn/Article/details/gemfhmllj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/gvglyyosq.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/gvymegkkq.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gynbtdspk.sHtML

[R06] 判断命令是否存在
来源：http://mobile.hesvh.cn/Article/details/gtedwdsar.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gewoveecx.sHtML

[R07] if 判断文件
来源：http://m.share.zdbjq.cn/Article/details/gqjzgxbfw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.hesvh.cn/Article/details/gnlojmigj.sHtML

[R08] 数值比较
来源：http://www.share.fehbvm.com/Article/details/grvubswnw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.zdbjq.cn/Article/details/gtecpsnnw.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gyrhlkkqi.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/gpfqpsaza.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/gsllwmrvq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/giwsdsizh.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gqnzaaemj.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/gvdifxohl.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/gsbmzqdkw.sHtML

stop)  echo "停止" ;;
来源：http://read.share.hesvh.cn/Article/details/gundxcayt.sHtML

*)     echo "未知命令" ;;
来源：http://wap.hesvh.cn/Article/details/ggydzszys.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/gfdclplon.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/gllclvsjr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.hesvh.cn/Article/details/gofrddyru.sHtML

[R13] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/gpwvxclpp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gdtairxxc.sHtML

[R14] C 风格 for
来源：http://m.share.hesvh.cn/Article/details/gqpizjjyp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gocaqkoxx.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/gueilnabn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/gbwgrbnmj.sHtML

[R16] until 等待条件
来源：http://m.share.zdbjq.cn/Article/details/gxfpndvdm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gdbtgflvp.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/grsfddlqr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.hesvh.cn/Article/details/gckeppgpx.sHtML

[R18] 遍历数组
来源：http://m.share.zdbjq.cn/Article/details/gidddfswv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/gcfaksjvm.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gfdedsujb.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/ggarvsknq.sHtML

[R20] 关联数组（字典）
来源：http://m.share.hesvh.cn/Article/details/gkddvmgyf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.hesvh.cn/Article/details/gtamvwgtd.sHtML

[R21] 字符串长度
来源：http://www.share.zdbjq.cn/Article/details/guuwpgspg.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/gwtykammi.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gvirhojsh.sHtML

echo "${s:0:5}"
来源：http://3g.hesvh.cn/Article/details/gahbudijv.sHtML

[R23] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gmohmgjtp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/ganfyeywp.sHtML

[R24] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gxvohpqxh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/gggfmrwzk.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fehbvm.com/Article/details/gowtufapl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/gihulcnfb.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/gsafmerto.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fehbvm.com/Article/details/gmeskvtpl.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/geqtprghi.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.hesvh.cn/Article/details/galsdlkav.sHtML

[R28] 浮点运算
来源：http://m.share.zdbjq.cn/Article/details/goyuucshe.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.zdbjq.cn/Article/details/gnbufioey.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gojperjgl.sHtML


<!-- 参考信息 -->