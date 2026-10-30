代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.zdbjq.cn/Article/details/gmkvyatet.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.zdbjq.cn/Article/details/geszqrcuk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.hesvh.cn/Article/details/grvsoptov.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/gxkjgjrtp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.hesvh.cn/Article/details/gtdeaiyme.sHtML

TS:   if (x == null) {}
来源：http://www.blog.hesvh.cn/Article/details/ghupyjxtn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gcarpouyu.sHtML

Go:   if x == nil {}
来源：http://baike.zdbjq.cn/Article/details/gbjfqnizk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fehbvm.com/Article/details/gxigovyxe.sHtML

C#:   if (x is null) {}
来源：http://3g.hesvh.cn/Article/details/glgzkkutx.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/gvzwdphxc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/gwvcbvsyk.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.hesvh.cn/Article/details/gdcdtgnju.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gkohquecl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gvwmtkpma.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.zdbjq.cn/Article/details/gwaziybzw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fehbvm.com/Article/details/gyfthcawq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.hesvh.cn/Article/details/givfenosb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.hesvh.cn/Article/details/gudivpxpf.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.zdbjq.cn/Article/details/gsfnixeeg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fehbvm.com/Article/details/gakiesaqe.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/gsjuuiixc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.hesvh.cn/Article/details/gtxkaqhtm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/gfwbmbugj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/gmfwgsyao.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fehbvm.com/Article/details/gtqqtwwfp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.hesvh.cn/Article/details/gfveyiwrt.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fehbvm.com/Article/details/gtrfxbybn.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grezdzmha.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/gisyarjnt.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gihkmxtny.sHtML

[Q01] 创建表
来源：http://www.share.fehbvm.com/Article/details/gyfmvguny.sHtML

CREATE TABLE users (
来源：http://m.share.zdbjq.cn/Article/details/geoarketj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gwptymspb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/guohlstya.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fehbvm.com/Article/details/gdisuwdqz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/gzrobnjcc.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gtnuuywmz.sHtML

[Q02] 创建带外键的表
来源：http://read.share.zdbjq.cn/Article/details/gevsazfki.sHtML

CREATE TABLE orders (
来源：http://www.share.fehbvm.com/Article/details/gquhfrilw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gpsuskxor.sHtML

user_id INT NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gouvzoafj.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fehbvm.com/Article/details/gugyuegeo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fehbvm.com/Article/details/gjkgmpmnr.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gogaguhpb.sHtML

[Q03] 增加列
来源：http://www.share.zdbjq.cn/Article/details/gzhvnpksw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gnhvcfdio.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/gehnnqjjd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/gvjswxykn.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/gflzashwm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fehbvm.com/Article/details/grceijxsm.sHtML

[Q06] 删除列
来源：http://blog.fehbvm.com/Article/details/ggbhwxhtx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fehbvm.com/Article/details/gtocqggdz.sHtML

[Q07] 删除表
来源：http://m.share.hesvh.cn/Article/details/gehnkwwgz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.zdbjq.cn/Article/details/gjefobdzd.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/ggnvxwrnm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/ggvydqqjp.sHtML

[Q09] 创建唯一索引
来源：http://wap.fehbvm.com/Article/details/gbrhslqxt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gtjgfrkio.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/gszpilujb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/gcwwedzds.sHtML

[Q11] 一次插入多行
来源：http://m.share.zdbjq.cn/Article/details/gvhribokv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/glddpdaqs.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/gcgwtzlzb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.zdbjq.cn/Article/details/gjxooyjab.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.hesvh.cn/Article/details/gtcismaoj.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fehbvm.com/Article/details/gqqezrabu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.zdbjq.cn/Article/details/ghodjwkln.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/glzrovhyj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.hesvh.cn/Article/details/gcyfoglag.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.zdbjq.cn/Article/details/gewrcfxsx.sHtML

[Q15] 查询全部
来源：http://mobile.zdbjq.cn/Article/details/gjukatrkb.sHtML

SELECT * FROM users;
来源：http://m.share.fehbvm.com/Article/details/gkzyjjiex.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fehbvm.com/Article/details/gpdpnigab.sHtML

SELECT id, name FROM users;
来源：http://3g.fehbvm.com/Article/details/gtcaejukn.sHtML

[Q17] 条件查询
来源：http://www.blog.fehbvm.com/Article/details/gxgatzofe.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.zdbjq.cn/Article/details/gawrbtrzc.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gzrghziml.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.zdbjq.cn/Article/details/gxcehmjmr.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/gwugoxoka.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/gefmflaaz.sHtML

[Q20] IN 列表
来源：http://read.share.zdbjq.cn/Article/details/gjevqevrg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/gfokxstvr.sHtML

[Q21] 空值判断
来源：http://read.share.fehbvm.com/Article/details/gcunarukg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fehbvm.com/Article/details/gyxfgmyzq.sHtML

[Q22] 排序
来源：http://blog.hesvh.cn/Article/details/gdtfqlnph.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fehbvm.com/Article/details/govqddzpc.sHtML

[Q23] 分页
来源：http://mobile.zdbjq.cn/Article/details/gdlvlsoxi.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fehbvm.com/Article/details/gpywortdf.sHtML

[Q24] 去重
来源：http://3g.hesvh.cn/Article/details/glrfpjmxy.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fehbvm.com/Article/details/gfvciklvj.sHtML

[Q25] 只取前 N 条
来源：http://mobile.hesvh.cn/Article/details/goeljeeyw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/gcbafxfhh.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/gaaxscjvv.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.zdbjq.cn/Article/details/guvgpqppf.sHtML

[Q27] 条件计数
来源：http://www.share.zdbjq.cn/Article/details/gjpcbwrup.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gadlivwxr.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/gsjqyccpo.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gofbrnvkv.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/gvhtdegei.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fehbvm.com/Article/details/ghcdycafj.sHtML

[Q30] 分组统计
来源：http://3g.zdbjq.cn/Article/details/gezhrtses.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/glssmoxag.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fehbvm.com/Article/details/githespwj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/gbhtylvae.sHtML

[Q32] 分组拼接字符串
来源：http://wap.hesvh.cn/Article/details/gafxolnzf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gomuohxid.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/gxgewuzbn.sHtML

[Q33] 多列分组
来源：http://mobile.zdbjq.cn/Article/details/grlwewzws.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/gdwjvehxa.sHtML

[Q34] 每组取第一条
来源：http://3g.fehbvm.com/Article/details/givxvgfqz.sHtML

SELECT * FROM (
来源：http://www.blog.zdbjq.cn/Article/details/gukzbtiwx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fehbvm.com/Article/details/gpjnwmlmd.sHtML

) t WHERE rn = 1;
来源：http://blog.zdbjq.cn/Article/details/gvlpyrhuw.sHtML

[Q35] 内连接
来源：http://m.share.hesvh.cn/Article/details/gptsjmibs.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gecqojfyy.sHtML

[Q36] 左连接
来源：http://wap.zdbjq.cn/Article/details/gggxbaosk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gjrboufvb.sHtML

[Q37] 右连接
来源：http://www.blog.fehbvm.com/Article/details/gwrfbfzzb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fehbvm.com/Article/details/ghwinetjz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.hesvh.cn/Article/details/glmjkiado.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.hesvh.cn/Article/details/gkqdxccgp.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.zdbjq.cn/Article/details/guzhxktjk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.zdbjq.cn/Article/details/gatcgjrjb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.zdbjq.cn/Article/details/gpkvduqlc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.zdbjq.cn/Article/details/gmnfeqdoe.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.hesvh.cn/Article/details/ghlqnrsjb.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/gdakrwidt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.hesvh.cn/Article/details/gmtivhzfa.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.hesvh.cn/Article/details/gutdxduiw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.zdbjq.cn/Article/details/grotiqyub.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/gnhwfhbyz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.hesvh.cn/Article/details/ghdzgwnrw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fehbvm.com/Article/details/gyjzvfcah.sHtML

[Q43] 标量子查询
来源：http://m.share.fehbvm.com/Article/details/gvxzpmlzz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/givofbxrq.sHtML

[Q44] IN 子查询
来源：http://blog.hesvh.cn/Article/details/ghuqxjqny.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.hesvh.cn/Article/details/gctahultk.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gafkfunho.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gwesatluh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/grconuydy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/giolhsefs.sHtML

[Q47] 与平均值比较
来源：http://m.share.zdbjq.cn/Article/details/gieeubuhj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fehbvm.com/Article/details/gjrdzkebl.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fehbvm.com/Article/details/gfsqqgnry.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/gnzxzopin.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fehbvm.com/Article/details/gwwwyboaj.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/gljkavjfa.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gcersnjeg.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gvbfgiwjn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.hesvh.cn/Article/details/gngbcyuwj.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fehbvm.com/Article/details/grztgyfay.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.hesvh.cn/Article/details/gfyprvpno.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/guxuwamdy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gpnnzizrr.sHtML

[Q53] 按条件删除
来源：http://mobile.hesvh.cn/Article/details/gnwwzzfim.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.hesvh.cn/Article/details/gqfbhklyc.sHtML

[Q54] 清空表
来源：http://www.blog.hesvh.cn/Article/details/gswewwhfa.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fehbvm.com/Article/details/gktqffmjh.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fehbvm.com/Article/details/ggtnrhcsf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.hesvh.cn/Article/details/gyaophhbo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.zdbjq.cn/Article/details/gstrdcsdb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gwlafmcvk.sHtML

[Q57] 行号
来源：http://baike.zdbjq.cn/Article/details/gkiwknxpm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/gqlrckedt.sHtML

[Q58] 累计求和
来源：http://m.share.hesvh.cn/Article/details/glufkpkak.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gtgppqixj.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/ggovumqzu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/ggnlvmagt.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.zdbjq.cn/Article/details/gbypuqosi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.zdbjq.cn/Article/details/ggswkaiow.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gmpehwedr.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gyuixxwrh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gtgjwwduo.sHtML

[Q62] 分组占比
来源：http://www.share.fehbvm.com/Article/details/gzynlaqhb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gagslwgqh.sHtML

[Q63] 开启事务
来源：http://read.share.fehbvm.com/Article/details/gjwdqheef.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.zdbjq.cn/Article/details/galeyeped.sHtML

[Q64] 提交事务
来源：http://blog.zdbjq.cn/Article/details/ghyqxkijv.sHtML

COMMIT;
来源：http://m.share.zdbjq.cn/Article/details/gewvzyyki.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/gturuuwaw.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/givzsrtfl.sHtML

[Q66] 行锁查询
来源：http://wap.hesvh.cn/Article/details/grsvqlwyo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/glvvhdqec.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fehbvm.com/Article/details/gzenkoiou.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.hesvh.cn/Article/details/ggocvzvyp.sHtML

[Q68] 保存点
来源：http://www.m.share.zdbjq.cn/Article/details/gsymgeike.sHtML

SAVEPOINT sp1;
来源：http://baike.hesvh.cn/Article/details/gsrlhcxsl.sHtML

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/gikrpkvtk.sHtML

[Q69] 查看执行计划
来源：http://mobile.hesvh.cn/Article/details/gqvmtqpus.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.zdbjq.cn/Article/details/gwhhaykry.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fehbvm.com/Article/details/grmekdktt.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/gkyxptreo.sHtML

[Q71] 查看建表语句
来源：http://www.blog.hesvh.cn/Article/details/gkavfckxj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.zdbjq.cn/Article/details/gsepwkzdx.sHtML

[Q72] 查看索引
来源：http://www.blog.fehbvm.com/Article/details/gkopsnjpp.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/gtxebrryr.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/gzyoyovsu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/guvbkhtgd.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/grpqvewsi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.zdbjq.cn/Article/details/gjfgjkmka.sHtML

[Q75] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gmsyoglor.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.hesvh.cn/Article/details/gtnxrxjut.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/glpmcvsdy.sHtML

[Q76] 按天统计
来源：http://www.share.fehbvm.com/Article/details/gbwweahfu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.zdbjq.cn/Article/details/gicmeyiph.sHtML

[Q77] 时间加减
来源：http://read.share.hesvh.cn/Article/details/gepybuorb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/gmeevvegr.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/gaaftkeyz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.zdbjq.cn/Article/details/gopdsidvi.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/gjfumqfvh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.zdbjq.cn/Article/details/gakfmeuih.sHtML

[Q80] 字符串截取
来源：http://baike.hesvh.cn/Article/details/gshyjhxqx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gverxkpmo.sHtML

[Q81] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gvumemypm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gvkhklmyo.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fehbvm.com/Article/details/gcjnzjqgg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ghjxxvihn.sHtML

[Q83] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/guuufhtno.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gxvbrsgei.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gtjdahwxi.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gqefpqkdq.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/gurfnpwhu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.zdbjq.cn/Article/details/ggivczqld.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fehbvm.com/Article/details/ggbczcorw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/ggqorjmso.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/gzkhykoim.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/gzusbcmcq.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/ggnsuzzbv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.zdbjq.cn/Article/details/gibxuwlre.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/gyqlcptab.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/gfajekymt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.zdbjq.cn/Article/details/gplzmpvkm.sHtML

[Q90] 生成序号列
来源：http://www.m.share.hesvh.cn/Article/details/ggbikpkqy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gtiolxpdf.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/guluwnddu.sHtML

R. Bash 专题
来源：http://baike.hesvh.cn/Article/details/gqpkqshzt.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gewsuhfvg.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/gxumfcuno.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/ghxvsqppa.sHtML

set -euo pipefail
来源：http://blog.fehbvm.com/Article/details/gorpjkpwu.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.zdbjq.cn/Article/details/gtgyfjvrx.sHtML

name="Tom"; echo "$name"
来源：http://mobile.hesvh.cn/Article/details/gknbadgbw.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/gyqkmoubu.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/gbrqfblvm.sHtML

[R04] 位置参数
来源：http://www.m.share.hesvh.cn/Article/details/gaxysusgo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/gfuknxylu.sHtML

[R05] 参数默认值
来源：http://m.share.fehbvm.com/Article/details/glzafexer.sHtML

name="${1:-default}"
来源：http://mobile.fehbvm.com/Article/details/guwuzinbu.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/gswzlpobr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gmmpcvwgx.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/gbicqydcb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gmkrhchep.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/gffkgodpv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fehbvm.com/Article/details/guvsinuya.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gkjbqpyey.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fehbvm.com/Article/details/gklpehcza.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/gxltkobei.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.zdbjq.cn/Article/details/gejyrrsbe.sHtML

[R11] case 多分支
来源：http://wap.hesvh.cn/Article/details/gjoqqrowr.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/ghecoqcwd.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/gbpdfkhqk.sHtML

stop)  echo "停止" ;;
来源：http://www.share.hesvh.cn/Article/details/gsxxmzlan.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fehbvm.com/Article/details/gxdpfbqra.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/gyflwsxyc.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/grjcuzfhl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/gjypnrsde.sHtML

[R13] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/gjxlwotar.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gzmkbumkt.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/grimkxela.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/ghpzcpxih.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gqaxbkjak.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gxoqfysje.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/gfbgwflro.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gxnqwyskg.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/ghdgmqgyt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.hesvh.cn/Article/details/gdbsoanje.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/gitqnthio.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/garbucdqd.sHtML

[R19] 数组长度
来源：http://baike.hesvh.cn/Article/details/gocgkznyk.sHtML

echo "${#arr[@]}"
来源：http://www.share.hesvh.cn/Article/details/gglthigcr.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/ggbegdkwk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.hesvh.cn/Article/details/gkcdmdftt.sHtML

[R21] 字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gadynrdbi.sHtML

echo "${#s}"
来源：http://baike.zdbjq.cn/Article/details/gvjuqdobf.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/gvcjpsctp.sHtML

echo "${s:0:5}"
来源：http://3g.zdbjq.cn/Article/details/gvtotuuah.sHtML

[R23] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gvdwtlold.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/gyouybmuf.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gvynzxevf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.hesvh.cn/Article/details/gvvbmtchf.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fehbvm.com/Article/details/gdasnsduu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/gmjdallir.sHtML

[R26] 命令替换
来源：http://www.blog.zdbjq.cn/Article/details/gwmnhkshh.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fehbvm.com/Article/details/gfsurxewp.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/gzfrtseaj.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/ggvtgkmqz.sHtML

[R28] 浮点运算
来源：http://read.share.zdbjq.cn/Article/details/gaznxcdst.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.hesvh.cn/Article/details/gkjvjfpaa.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/goznkljaj.sHtML


<!-- 参考信息 -->