代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.zdbjq.cn/Article/details/gvxhtljby.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/grshqrmew.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.zdbjq.cn/Article/details/gyyxwxqeg.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/guvgnxxgw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.zdbjq.cn/Article/details/gupewleyj.sHtML

TS:   if (x == null) {}
来源：http://www.share.zdbjq.cn/Article/details/gusvcldxv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gqxijvdqz.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/ghxnyrcua.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fehbvm.com/Article/details/gkymrxwjn.sHtML

C#:   if (x is null) {}
来源：http://mobile.zdbjq.cn/Article/details/glplzzpzr.sHtML

[P07] 防抖与节流
来源：http://blog.hesvh.cn/Article/details/gqojvkgsf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/ggtgdnuzf.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.zdbjq.cn/Article/details/gfzholwhe.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gdfmrnrmd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/garafvkeg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.hesvh.cn/Article/details/gpgqlgjhs.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fehbvm.com/Article/details/gfytfhadw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.zdbjq.cn/Article/details/glkpkqqyl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/gifjgdpro.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.zdbjq.cn/Article/details/glywdoirs.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/gistwuabe.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/gmfkiydzq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fehbvm.com/Article/details/gjldagcvl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gmxfbxvcy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.zdbjq.cn/Article/details/ggkluboya.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fehbvm.com/Article/details/gvwvtrxjx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.hesvh.cn/Article/details/gdvcombjf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.hesvh.cn/Article/details/guzobugde.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkcqwzywh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.hesvh.cn/Article/details/gkxwfpjbs.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gifbutqgd.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/gtfivklnk.sHtML

CREATE TABLE users (
来源：http://mobile.zdbjq.cn/Article/details/gjetgnxaz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gxmchwenw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gqrqxznii.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.zdbjq.cn/Article/details/gyevhefef.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/gqauqklvz.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gaoqhxtmt.sHtML

[Q02] 创建带外键的表
来源：http://blog.hesvh.cn/Article/details/gskxkgzdp.sHtML

CREATE TABLE orders (
来源：http://www.blog.fehbvm.com/Article/details/gywbgrpwb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gfvrzmhix.sHtML

user_id INT NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/ghzlfhuqx.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fehbvm.com/Article/details/gcbzxxfhq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fehbvm.com/Article/details/gixxwroov.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gmrjhmujd.sHtML

[Q03] 增加列
来源：http://m.share.zdbjq.cn/Article/details/gwalykbfx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.zdbjq.cn/Article/details/geogfkfen.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/gdxfrwvjk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/gwnyxznob.sHtML

[Q05] 重命名列
来源：http://baike.zdbjq.cn/Article/details/genrruqci.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.hesvh.cn/Article/details/gignyjiuh.sHtML

[Q06] 删除列
来源：http://wap.fehbvm.com/Article/details/gmkrwzqwd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.hesvh.cn/Article/details/gaplxeswp.sHtML

[Q07] 删除表
来源：http://mobile.zdbjq.cn/Article/details/glgnyadvc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.hesvh.cn/Article/details/gbrankwoc.sHtML

[Q08] 创建普通索引
来源：http://m.share.fehbvm.com/Article/details/gbgrgxisi.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gbryuyhwg.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/gcjfkahfe.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gdwpeyupv.sHtML

[Q10] 插入单行
来源：http://mobile.fehbvm.com/Article/details/geueyaxvj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gjcrqlqkf.sHtML

[Q11] 一次插入多行
来源：http://blog.fehbvm.com/Article/details/gorikymct.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gffjfpdtx.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/gcikpnkxg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fehbvm.com/Article/details/gaahvhrsi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/gubqcqlno.sHtML

[Q13] 忽略重复插入
来源：http://3g.hesvh.cn/Article/details/gukixrglc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.hesvh.cn/Article/details/gdrbubdrj.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.zdbjq.cn/Article/details/gtvmsltob.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fehbvm.com/Article/details/gnexkggfb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.zdbjq.cn/Article/details/gesplphuh.sHtML

[Q15] 查询全部
来源：http://read.share.zdbjq.cn/Article/details/gfuruzcsf.sHtML

SELECT * FROM users;
来源：http://3g.zdbjq.cn/Article/details/gahavnldo.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gitaooonw.sHtML

SELECT id, name FROM users;
来源：http://www.share.hesvh.cn/Article/details/glsznnfsc.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/gbmqkiebz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fehbvm.com/Article/details/gvlpdsxxh.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.hesvh.cn/Article/details/gxlmuxqeh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.hesvh.cn/Article/details/gynhaswsm.sHtML

[Q19] 范围查询
来源：http://baike.hesvh.cn/Article/details/gcsrbmgfe.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.hesvh.cn/Article/details/gqcymfgnq.sHtML

[Q20] IN 列表
来源：http://www.blog.fehbvm.com/Article/details/ggrnkjbnt.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fehbvm.com/Article/details/gshxtvaio.sHtML

[Q21] 空值判断
来源：http://blog.fehbvm.com/Article/details/gntznqybs.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.zdbjq.cn/Article/details/glpeziauv.sHtML

[Q22] 排序
来源：http://blog.zdbjq.cn/Article/details/gpkxbxhni.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fehbvm.com/Article/details/gflfijywq.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/gwuzdsije.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fehbvm.com/Article/details/gboklaugq.sHtML

[Q24] 去重
来源：http://3g.zdbjq.cn/Article/details/gyhinyjso.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gjkvegccq.sHtML

[Q25] 只取前 N 条
来源：http://wap.hesvh.cn/Article/details/ggeouppct.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.hesvh.cn/Article/details/gqbiglkki.sHtML

[Q26] 计数
来源：http://www.share.hesvh.cn/Article/details/gppbgizrd.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gkehdpmbx.sHtML

[Q27] 条件计数
来源：http://read.share.hesvh.cn/Article/details/gxszivqro.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.hesvh.cn/Article/details/gqbkewbfe.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/grfpteime.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gtssbocdn.sHtML

[Q29] 最大最小值
来源：http://www.share.zdbjq.cn/Article/details/gravrpjqh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gmtdlbdrp.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/gkfppwybk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/guauxpclj.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/goblizjpg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.zdbjq.cn/Article/details/ghzujscie.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/ggbqpqwqe.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gwuwixnfc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.zdbjq.cn/Article/details/ggrfnygrq.sHtML

[Q33] 多列分组
来源：http://www.share.zdbjq.cn/Article/details/gwpcdqlyn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/gawonlvpp.sHtML

[Q34] 每组取第一条
来源：http://baike.fehbvm.com/Article/details/gqgipqvto.sHtML

SELECT * FROM (
来源：http://read.share.fehbvm.com/Article/details/gafkdohoq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/gbsmqfaun.sHtML

) t WHERE rn = 1;
来源：http://3g.zdbjq.cn/Article/details/gckfqftjn.sHtML

[Q35] 内连接
来源：http://www.m.share.hesvh.cn/Article/details/geegshbef.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/groaowoki.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/gjaeewhvz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gzqvuclpc.sHtML

[Q37] 右连接
来源：http://www.blog.zdbjq.cn/Article/details/gujiokrir.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/grwyzhvmr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.zdbjq.cn/Article/details/gaasdzwpf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/ggqozydqc.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.zdbjq.cn/Article/details/gzwestygl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/gptrqshem.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fehbvm.com/Article/details/gpqicsnnm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/gmznphekh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.hesvh.cn/Article/details/gwmfxoprt.sHtML

[Q41] 多表连接
来源：http://www.share.hesvh.cn/Article/details/grzekuvxv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.hesvh.cn/Article/details/guvikhjos.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fehbvm.com/Article/details/gdvatqirr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/gfqyzhbqz.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.hesvh.cn/Article/details/gpgahhrwx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fehbvm.com/Article/details/gemtbywzr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fehbvm.com/Article/details/gtfluyglw.sHtML

[Q43] 标量子查询
来源：http://www.blog.fehbvm.com/Article/details/gilrwsfjy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fehbvm.com/Article/details/gofkoesnr.sHtML

[Q44] IN 子查询
来源：http://www.share.hesvh.cn/Article/details/ggeacrvxv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.hesvh.cn/Article/details/goygzaxwg.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.zdbjq.cn/Article/details/gbddgsmyi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/glvvyrozo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/grsiqcdqs.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gfvktbqvp.sHtML

[Q47] 与平均值比较
来源：http://blog.hesvh.cn/Article/details/gehrhmvsf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fehbvm.com/Article/details/gcwwjuxmu.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gatbnpusi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fehbvm.com/Article/details/grkmtoxfd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.zdbjq.cn/Article/details/gpbalyanl.sHtML

[Q49] 更新单行
来源：http://3g.zdbjq.cn/Article/details/gvcllejel.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gbqjpedxa.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gnnjpzjrc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/ghmbuxhxn.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/gpnrphjxb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.zdbjq.cn/Article/details/gkidqhmkk.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/gdiuznhny.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gzjsfnaal.sHtML

[Q53] 按条件删除
来源：http://read.share.zdbjq.cn/Article/details/gkdddydyc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.hesvh.cn/Article/details/gplthfxcd.sHtML

[Q54] 清空表
来源：http://baike.zdbjq.cn/Article/details/grbyqwmxw.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fehbvm.com/Article/details/guoxjktis.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/gkeewlpad.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.hesvh.cn/Article/details/gnbggcjxz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.zdbjq.cn/Article/details/gmhacutza.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gszpthpjo.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/ggegijmkz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gakiccdmj.sHtML

[Q58] 累计求和
来源：http://wap.zdbjq.cn/Article/details/gsrfvcdjk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/geiwgfqlk.sHtML

[Q59] 分组内累计
来源：http://www.share.hesvh.cn/Article/details/gfydkjlfp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gtwpojjpf.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.hesvh.cn/Article/details/gloahcmmr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.zdbjq.cn/Article/details/gecbeuvoc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gacqijzfm.sHtML

[Q61] 移动平均
来源：http://www.share.fehbvm.com/Article/details/gpilwqhth.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gxmoymzof.sHtML

[Q62] 分组占比
来源：http://mobile.hesvh.cn/Article/details/gduxkyzak.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gjhkymgsn.sHtML

[Q63] 开启事务
来源：http://baike.fehbvm.com/Article/details/gpvsjqwsk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.hesvh.cn/Article/details/gpwmzjqqr.sHtML

[Q64] 提交事务
来源：http://3g.fehbvm.com/Article/details/gwyuowfwc.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/ggtqdfcts.sHtML

[Q65] 回滚事务
来源：http://wap.zdbjq.cn/Article/details/gkxslodsj.sHtML

ROLLBACK;
来源：http://wap.hesvh.cn/Article/details/gvokccsbt.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/gwnyabequ.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.zdbjq.cn/Article/details/gdpfrseqd.sHtML

[Q67] 设置隔离级别
来源：http://baike.zdbjq.cn/Article/details/gifzidfwj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/gerzksmky.sHtML

[Q68] 保存点
来源：http://www.share.fehbvm.com/Article/details/gerhethou.sHtML

SAVEPOINT sp1;
来源：http://www.share.zdbjq.cn/Article/details/gqteehxlr.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gtnkodcwc.sHtML

[Q69] 查看执行计划
来源：http://m.share.fehbvm.com/Article/details/gqdluxzfr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/gsyspkjxl.sHtML

[Q70] 更新统计信息
来源：http://www.share.zdbjq.cn/Article/details/gohanbqww.sHtML

ANALYZE TABLE users;
来源：http://www.share.fehbvm.com/Article/details/gzdwxsxjc.sHtML

[Q71] 查看建表语句
来源：http://www.share.hesvh.cn/Article/details/gxmvxuqrh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/ghnqvzhxq.sHtML

[Q72] 查看索引
来源：http://www.share.zdbjq.cn/Article/details/gltdywiqt.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/gucfcsxoc.sHtML

[Q73] 查看表状态
来源：http://www.blog.zdbjq.cn/Article/details/gklzvvoov.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/gghtegdxk.sHtML

[Q74] 强制使用索引
来源：http://baike.hesvh.cn/Article/details/ggzpbbpvn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fehbvm.com/Article/details/glkvkdpix.sHtML

[Q75] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gdmwpclhy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gndrzszuq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/gqejsewhe.sHtML

[Q76] 按天统计
来源：http://www.m.share.hesvh.cn/Article/details/gvqhzsxtw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/gplljomxd.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/gvoxemfvn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/gaejgjghw.sHtML

[Q78] 当前时间
来源：http://wap.hesvh.cn/Article/details/gftqadnae.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.hesvh.cn/Article/details/garrhursd.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/geymgufhk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.zdbjq.cn/Article/details/gywninvfl.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/glhfkpkga.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/ggpxncpcp.sHtML

[Q81] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gteyxlkav.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.hesvh.cn/Article/details/gzmsfuxve.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gbgonrkrf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gxifecfqm.sHtML

[Q83] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/galbbpfxj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gajxbltcy.sHtML

[Q84] 去除首尾空格
来源：http://mobile.zdbjq.cn/Article/details/gmljkjhfl.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gulkikhfm.sHtML

[Q85] 数值取整
来源：http://www.share.fehbvm.com/Article/details/gkeqqptha.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/gzubpuicp.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.zdbjq.cn/Article/details/gxpbwaeqz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.hesvh.cn/Article/details/gbtzipcpm.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/gwnxeyivh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/gdsoqqwvn.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fehbvm.com/Article/details/gsilpqrlu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/gouvxeqyq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/gvozxtmqy.sHtML

[Q89] 判断表是否存在
来源：http://mobile.zdbjq.cn/Article/details/gsfxhcunw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.zdbjq.cn/Article/details/gropcxraz.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/gwosafoyx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/gxqkocfjd.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gexuelkpj.sHtML

R. Bash 专题
来源：http://baike.hesvh.cn/Article/details/gegfnrcai.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/geechkske.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/gazuuixlg.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.zdbjq.cn/Article/details/gxarzclnb.sHtML

set -euo pipefail
来源：http://www.blog.hesvh.cn/Article/details/gykpihkfg.sHtML

[R02] 变量赋值与使用
来源：http://blog.zdbjq.cn/Article/details/ghfggkcmf.sHtML

name="Tom"; echo "$name"
来源：http://baike.hesvh.cn/Article/details/gdsplgpns.sHtML

[R03] 只读变量
来源：http://blog.fehbvm.com/Article/details/gqezgaurn.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/gvczjhzho.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/gcuqplwnp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.hesvh.cn/Article/details/gocyxvdwf.sHtML

[R05] 参数默认值
来源：http://baike.zdbjq.cn/Article/details/gshlptgtu.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/gimfxzgof.sHtML

[R06] 判断命令是否存在
来源：http://read.share.zdbjq.cn/Article/details/gtgkxcfzl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gvkeuqibi.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/gkzmwdjkh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.zdbjq.cn/Article/details/geaargkpa.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gxmvkipqb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.hesvh.cn/Article/details/giozxtqxa.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gvqlnvjgd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/ggbuybgpr.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/gyyesqkxq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fehbvm.com/Article/details/gijeuixwy.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gleajptrb.sHtML

case "$1" in
来源：http://www.m.share.hesvh.cn/Article/details/gcbpztoyo.sHtML

start) echo "启动" ;;
来源：http://read.share.hesvh.cn/Article/details/gtjgmqeqt.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/gvtzzqfzk.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gdxctkbps.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/gdvfizsjx.sHtML

[R12] for 遍历文件
来源：http://www.blog.zdbjq.cn/Article/details/goxyfxomz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.zdbjq.cn/Article/details/gojgrcfav.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/gspyxxgsm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gncrfxgdd.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/gmbjhzvgw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gznimcuzv.sHtML

[R15] while 逐行读文件
来源：http://mobile.hesvh.cn/Article/details/ghmabysap.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.hesvh.cn/Article/details/ggbxunhsd.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gcvspfnoc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gitaysgnk.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.zdbjq.cn/Article/details/gjoigjrqa.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fehbvm.com/Article/details/grkjrlodw.sHtML

[R18] 遍历数组
来源：http://3g.fehbvm.com/Article/details/grtzqtkjp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/gpqoykaib.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gexysluxz.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/gxplyuqwc.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/gutzllxln.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.hesvh.cn/Article/details/ghdhkycgs.sHtML

[R21] 字符串长度
来源：http://3g.fehbvm.com/Article/details/ghuquzugc.sHtML

echo "${#s}"
来源：http://m.share.zdbjq.cn/Article/details/gtktspble.sHtML

[R22] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gfozbegkx.sHtML

echo "${s:0:5}"
来源：http://3g.hesvh.cn/Article/details/gmqlwubjr.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/glbcsxjsp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/gzyupffbg.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gknolfyct.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fehbvm.com/Article/details/gmcbyahhx.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/gvprhxdii.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/gcbzvffce.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/gmdntckuf.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/gmntqnopo.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/gozjfrzfx.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fehbvm.com/Article/details/glixcetzt.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/gggwnctmr.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.zdbjq.cn/Article/details/gwbbavein.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/gwdivvxsc.sHtML


<!-- 参考信息 -->