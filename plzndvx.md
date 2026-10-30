代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fanxiaobao.xyz/Article/details/gwojwbpot.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fanxiaobao.xyz/Article/details/guvxlhrun.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fanxiaobao.xyz/Article/details/gjaokxnht.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fanxiaobao.xyz/Article/details/guybskvgb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fanxiaobao.xyz/Article/details/gaoqjvgru.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgsszswb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gtjgsblpa.sHtML

Go:   if x == nil {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbezgpey.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fanxiaobao.xyz/Article/details/glhnachpq.sHtML

C#:   if (x is null) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcuseqyc.sHtML

[P07] 防抖与节流
来源：http://wap.fanxiaobao.xyz/Article/details/gvgqscpuu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fanxiaobao.xyz/Article/details/glcqcrqyd.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijvxzfzl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxajsiagt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fanxiaobao.xyz/Article/details/geccqpgrs.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbygbudr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkpheeal.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzawkmhaf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujsflsxy.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fanxiaobao.xyz/Article/details/gajnkqdug.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzsvhzpt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gthxmpfuo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fanxiaobao.xyz/Article/details/gjskzscdz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gajtzxhzb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesfdmbjf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fanxiaobao.xyz/Article/details/gwlbhpbbx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fanxiaobao.xyz/Article/details/gdhevvhiw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fanxiaobao.xyz/Article/details/garueeqhg.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gjcjckvlt.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fanxiaobao.xyz/Article/details/gmprovuvy.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gxhikghks.sHtML

[Q01] 创建表
来源：http://m.share.fanxiaobao.xyz/Article/details/gktozyfme.sHtML

CREATE TABLE users (
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwjdiusf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fanxiaobao.xyz/Article/details/gdaslrimh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fanxiaobao.xyz/Article/details/gopflpbql.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfvsyhcd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fanxiaobao.xyz/Article/details/gdkhwbvbh.sHtML

);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpuzjsfc.sHtML

[Q02] 创建带外键的表
来源：http://blog.fanxiaobao.xyz/Article/details/gmxnmwdqf.sHtML

CREATE TABLE orders (
来源：http://www.share.fanxiaobao.xyz/Article/details/gorxqnqop.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fanxiaobao.xyz/Article/details/ghunuaxgv.sHtML

user_id INT NOT NULL,
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwieunoi.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fanxiaobao.xyz/Article/details/gmcjhfopr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghficylhp.sHtML

);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhjokjdp.sHtML

[Q03] 增加列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gducgscbg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvarflirj.sHtML

[Q04] 修改列类型
来源：http://blog.fanxiaobao.xyz/Article/details/gugawrtaw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fanxiaobao.xyz/Article/details/gulpqbgtu.sHtML

[Q05] 重命名列
来源：http://mobile.fanxiaobao.xyz/Article/details/gphmscewe.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fanxiaobao.xyz/Article/details/gfbcgeieq.sHtML

[Q06] 删除列
来源：http://blog.fanxiaobao.xyz/Article/details/gkxnzbilf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fanxiaobao.xyz/Article/details/grceshmfl.sHtML

[Q07] 删除表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqrvgphy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gacxqudbm.sHtML

[Q08] 创建普通索引
来源：http://blog.fanxiaobao.xyz/Article/details/gehtqqmmq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqqdvpbe.sHtML

[Q09] 创建唯一索引
来源：http://baike.fanxiaobao.xyz/Article/details/gkrqzyosv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtboetji.sHtML

[Q10] 插入单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqklpyzfe.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fanxiaobao.xyz/Article/details/gugdvcxzo.sHtML

[Q11] 一次插入多行
来源：http://wap.fanxiaobao.xyz/Article/details/gxcodxyfw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fanxiaobao.xyz/Article/details/gbptboxhj.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fanxiaobao.xyz/Article/details/gdormejwn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fanxiaobao.xyz/Article/details/gozlflyer.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fanxiaobao.xyz/Article/details/gdlfubprt.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcanchdt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhfccknn.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fanxiaobao.xyz/Article/details/gpvxmkjrf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fanxiaobao.xyz/Article/details/gokjkhqed.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fanxiaobao.xyz/Article/details/gokpguxyp.sHtML

[Q15] 查询全部
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnhcyyeu.sHtML

SELECT * FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/ggdmnedjl.sHtML

[Q16] 查询指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gwcqjthpi.sHtML

SELECT id, name FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmmlabmp.sHtML

[Q17] 条件查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqmwdksh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/giyebwowp.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvvdagzm.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fanxiaobao.xyz/Article/details/gtoucynfg.sHtML

[Q19] 范围查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnxyijvb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcwgflce.sHtML

[Q20] IN 列表
来源：http://blog.fanxiaobao.xyz/Article/details/gslsvphyu.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gqilwuiwk.sHtML

[Q21] 空值判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvzxlxzh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fanxiaobao.xyz/Article/details/gwngvkrpu.sHtML

[Q22] 排序
来源：http://wap.fanxiaobao.xyz/Article/details/gutebqysh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fanxiaobao.xyz/Article/details/gofixxkdr.sHtML

[Q23] 分页
来源：http://mobile.fanxiaobao.xyz/Article/details/gryumrroy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fanxiaobao.xyz/Article/details/goowgdcsf.sHtML

[Q24] 去重
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhjbphgg.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebyxtqve.sHtML

[Q25] 只取前 N 条
来源：http://3g.fanxiaobao.xyz/Article/details/grjijhfdm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fanxiaobao.xyz/Article/details/ghqbpiaog.sHtML

[Q26] 计数
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjbeaske.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gedxlhbxh.sHtML

[Q27] 条件计数
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzxdblsm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gqyxximom.sHtML

[Q28] 求和与平均
来源：http://www.share.fanxiaobao.xyz/Article/details/glrnnicye.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclkkjbky.sHtML

[Q29] 最大最小值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdxhmvlm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbowpxat.sHtML

[Q30] 分组统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gaehhihmy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvmuinyp.sHtML

[Q31] 分组后过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gkyyetyka.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/guzjnaeak.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnscgfcxi.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grilathcp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzckzdxf.sHtML

[Q33] 多列分组
来源：http://blog.fanxiaobao.xyz/Article/details/gijfgoqxk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fanxiaobao.xyz/Article/details/ggebyfjfd.sHtML

[Q34] 每组取第一条
来源：http://m.share.fanxiaobao.xyz/Article/details/gpboowqud.sHtML

SELECT * FROM (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqneahdeb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fanxiaobao.xyz/Article/details/gvyyvhpnp.sHtML

) t WHERE rn = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/ggnodcjlq.sHtML

[Q35] 内连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqwgacpz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/golpxcefz.sHtML

[Q36] 左连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggsbygwrx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzhxpjrz.sHtML

[Q37] 右连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gonkrdsxq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gutlqujwu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fanxiaobao.xyz/Article/details/gsdmeanbt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/grwxbjzcu.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fanxiaobao.xyz/Article/details/gilcyrkbt.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgqhugwk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gfhvgxyga.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fanxiaobao.xyz/Article/details/gohckevdp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fanxiaobao.xyz/Article/details/gdfxnbqvg.sHtML

[Q41] 多表连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcqvxrbx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfncbnjug.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimkdotao.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyukdsdme.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxrigkaj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fanxiaobao.xyz/Article/details/guayqngod.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjtbrkam.sHtML

[Q43] 标量子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gojieezca.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fanxiaobao.xyz/Article/details/goanlmzej.sHtML

[Q44] IN 子查询
来源：http://wap.fanxiaobao.xyz/Article/details/gigceuwfn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fanxiaobao.xyz/Article/details/gdonrzdmp.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fanxiaobao.xyz/Article/details/gwtqilxhr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/grbhpbhcd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvekxznp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gexvsmdpr.sHtML

[Q47] 与平均值比较
来源：http://baike.fanxiaobao.xyz/Article/details/guuxlytwb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkuhsdfl.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gosyuaecv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fanxiaobao.xyz/Article/details/gmdmguljh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gxiynhmjp.sHtML

[Q49] 更新单行
来源：http://3g.fanxiaobao.xyz/Article/details/grdxwdyei.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxpxtggd.sHtML

[Q50] 批量更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giuxgtozd.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkrumomh.sHtML

[Q51] 用子查询更新
来源：http://blog.fanxiaobao.xyz/Article/details/glwrknrkn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtbtcttf.sHtML

[Q52] 删除指定行
来源：http://baike.fanxiaobao.xyz/Article/details/gtyamkkec.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkcvhsjz.sHtML

[Q53] 按条件删除
来源：http://www.share.fanxiaobao.xyz/Article/details/glajsrvmf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/gnrogiezt.sHtML

[Q54] 清空表
来源：http://wap.fanxiaobao.xyz/Article/details/gqnrbkoua.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsvrgomh.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gldevdjlz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfykqxhx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/garlzmpmh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gymauvjxg.sHtML

[Q57] 行号
来源：http://blog.fanxiaobao.xyz/Article/details/gaogltvzl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gljxriicd.sHtML

[Q58] 累计求和
来源：http://blog.fanxiaobao.xyz/Article/details/gddavgtav.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gyfxnbweh.sHtML

[Q59] 分组内累计
来源：http://wap.fanxiaobao.xyz/Article/details/gkitpkufk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gzegfdyxa.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gothmznmp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gboayqkrl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdbqlutq.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsnvxqmi.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gdmrlpcow.sHtML

[Q62] 分组占比
来源：http://read.share.fanxiaobao.xyz/Article/details/gzipzrnii.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkoqxoxp.sHtML

[Q63] 开启事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gmupadybc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzwckwiu.sHtML

[Q64] 提交事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gljvccrmi.sHtML

COMMIT;
来源：http://wap.fanxiaobao.xyz/Article/details/gokjmcfqk.sHtML

[Q65] 回滚事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxgxwkat.sHtML

ROLLBACK;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjguacee.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexibnssi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fanxiaobao.xyz/Article/details/gkdiszeyw.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fanxiaobao.xyz/Article/details/grfhrrnij.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/glsotvzei.sHtML

[Q68] 保存点
来源：http://baike.fanxiaobao.xyz/Article/details/gwmpplekz.sHtML

SAVEPOINT sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gefgdspkt.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/givzcpfeg.sHtML

[Q69] 查看执行计划
来源：http://blog.fanxiaobao.xyz/Article/details/glmlvdmph.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqlhqdzs.sHtML

[Q70] 更新统计信息
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqapgves.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyanikxho.sHtML

[Q71] 查看建表语句
来源：http://read.share.fanxiaobao.xyz/Article/details/gehqvvcbi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpdxmpdg.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/glqkvwivl.sHtML

SHOW INDEX FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gvntlwetu.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/gjssnxdvp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guixzxloz.sHtML

[Q74] 强制使用索引
来源：http://blog.fanxiaobao.xyz/Article/details/gseormgwp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhbxzxsm.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsakrqvrw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmxnorzn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fanxiaobao.xyz/Article/details/gvngecvij.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/gajfhxhao.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtyjaispz.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/gzajfbcwf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fanxiaobao.xyz/Article/details/ghmkhvjhb.sHtML

[Q78] 当前时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpmhsdhb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcvcxnqx.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnhaioun.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fanxiaobao.xyz/Article/details/gygpcdkcw.sHtML

[Q80] 字符串截取
来源：http://blog.fanxiaobao.xyz/Article/details/gaiqrnzls.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gdmplzcad.sHtML

[Q81] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gepvlmnoy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskhwrcul.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgqhswke.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/goybpfxtm.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfyuqggx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gkpylgjpm.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklntiffg.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gixikhzho.sHtML

[Q85] 数值取整
来源：http://wap.fanxiaobao.xyz/Article/details/gjqcjydyi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/gftojegsl.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/giyfaabuu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/grqsbazdz.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/ghkfnojwi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/gjmosqjoh.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/giykvsgqe.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/gqtsnvumx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gznvvigqw.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/grakjtlwl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gxckhmxxl.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/gxyytkcjf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/gsikcgrww.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ghnyjnkjl.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gavnpmrlb.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxwykmyf.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gvdqymjar.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/gsncqdjkt.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvamhhtcl.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gqvhlacey.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/gypofmnom.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhhedaif.sHtML

readonly PI=3.14
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjzhfden.sHtML

[R04] 位置参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdeupjme.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/glhgdakvc.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gitnonghu.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/gvaswjpaq.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/goftbpunh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnzmfxbt.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtotdbpdv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gijuwijmj.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/glktbbyjq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gadqdjowh.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gaevlzzil.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gsdhkvant.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gwgblqrda.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gswcwpdxv.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngtfcdgx.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvepwzkoe.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/grxzeqgwx.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gvahjskns.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdrrwjai.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvojkywi.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjxscsiy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gebjfmkwx.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedetcdpg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gbikfqqkt.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgcapeac.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdifbisw.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gchlvwucb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gppojftwb.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/glklhmzco.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrvhzgzx.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkokrgylm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gydmlpnsl.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqrgclbq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gccicopuf.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/glxokfjcq.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/ghaojwipx.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/gjvdohyhy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gqtbewhmh.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gdusqnllb.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gnxlknhkz.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbglbdkbi.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnyohoin.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gfseitlji.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/ggjfnbnlj.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gebskyygu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gclbvetwe.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/grisoctcu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gobzymtoj.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gcignnaps.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/grcibyxrs.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gmeuwikii.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gqynapzvr.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehtsvkrk.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gsnxqggnm.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzudfhsb.sHtML


<!-- 参考信息 -->