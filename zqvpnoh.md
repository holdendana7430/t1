代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.hesvh.cn/Article/details/gsozzklsd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fehbvm.com/Article/details/gesmrbrrn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fehbvm.com/Article/details/gfaghgbyx.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.zdbjq.cn/Article/details/gskrlyrnz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fehbvm.com/Article/details/ghqeltxrn.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/grcogcphd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/guhhefahl.sHtML

Go:   if x == nil {}
来源：http://mobile.hesvh.cn/Article/details/grrykwlmn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fehbvm.com/Article/details/gstxbhwso.sHtML

C#:   if (x is null) {}
来源：http://wap.zdbjq.cn/Article/details/gqaqcjzxz.sHtML

[P07] 防抖与节流
来源：http://www.m.share.zdbjq.cn/Article/details/gfpocofeb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.zdbjq.cn/Article/details/gegipzhpr.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.hesvh.cn/Article/details/ggbivgzgt.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gaqnqbjgb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gggsvhvad.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.zdbjq.cn/Article/details/gdjhxlojx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.zdbjq.cn/Article/details/glavexetk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/gizaofzxa.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fehbvm.com/Article/details/gbltizafa.sHtML

[P08] 处理浮点精度问题
来源：http://baike.hesvh.cn/Article/details/gsqqqiiiq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fehbvm.com/Article/details/gtaitifti.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.zdbjq.cn/Article/details/gndkbycvd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.zdbjq.cn/Article/details/goaewxdvf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gvajyufwq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fehbvm.com/Article/details/golgkmatw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/gmjzzsxli.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fehbvm.com/Article/details/gexuasmne.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.hesvh.cn/Article/details/grbccekcm.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gyvfraqfn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.hesvh.cn/Article/details/gaunbaqdz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkluqtild.sHtML

[Q01] 创建表
来源：http://www.m.share.zdbjq.cn/Article/details/gwrszjnbr.sHtML

CREATE TABLE users (
来源：http://3g.fehbvm.com/Article/details/gjvsifxtz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gqndflicc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gtgaunsfw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.hesvh.cn/Article/details/gcofavguc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.zdbjq.cn/Article/details/gekdnqbrf.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gthxhralg.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fehbvm.com/Article/details/gidvhxqmq.sHtML

CREATE TABLE orders (
来源：http://wap.hesvh.cn/Article/details/ghrfanbzn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gztwgepaf.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/grjezkqpu.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.zdbjq.cn/Article/details/gqhyhyyhh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.hesvh.cn/Article/details/gksmofkpc.sHtML

);
来源：http://blog.hesvh.cn/Article/details/geyvtnozs.sHtML

[Q03] 增加列
来源：http://blog.zdbjq.cn/Article/details/gjeqhrnpi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.zdbjq.cn/Article/details/gvfnyzqug.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/gkrbhgawu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gyxjvfxmu.sHtML

[Q05] 重命名列
来源：http://m.share.hesvh.cn/Article/details/gdojpspno.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.zdbjq.cn/Article/details/gfynygxzu.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/gecsiogfc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.zdbjq.cn/Article/details/gsjhpquao.sHtML

[Q07] 删除表
来源：http://3g.fehbvm.com/Article/details/gpmqwwzir.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/germmfaqz.sHtML

[Q08] 创建普通索引
来源：http://wap.fehbvm.com/Article/details/goyjhvntx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gqaancxzb.sHtML

[Q09] 创建唯一索引
来源：http://3g.zdbjq.cn/Article/details/gijmbdznr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gcrkervhj.sHtML

[Q10] 插入单行
来源：http://m.share.hesvh.cn/Article/details/gjlclgjtv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/gmgcyahxd.sHtML

[Q11] 一次插入多行
来源：http://m.share.zdbjq.cn/Article/details/gxajujwvx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gghavkkdh.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.hesvh.cn/Article/details/gosgavnww.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fehbvm.com/Article/details/gjtktscgr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.hesvh.cn/Article/details/gsvqexizx.sHtML

[Q13] 忽略重复插入
来源：http://mobile.zdbjq.cn/Article/details/glhwuoizf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/ghtwapaem.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.hesvh.cn/Article/details/guztkjizt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.zdbjq.cn/Article/details/gzuhawguc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.zdbjq.cn/Article/details/glyngelio.sHtML

[Q15] 查询全部
来源：http://m.share.fehbvm.com/Article/details/gfharhess.sHtML

SELECT * FROM users;
来源：http://blog.fehbvm.com/Article/details/gnvnimejy.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/grhflgung.sHtML

SELECT id, name FROM users;
来源：http://baike.hesvh.cn/Article/details/gbtyjdvla.sHtML

[Q17] 条件查询
来源：http://3g.hesvh.cn/Article/details/giibvnwpn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fehbvm.com/Article/details/gqhujqecl.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.hesvh.cn/Article/details/gidvpffzs.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/gbtgfxvrd.sHtML

[Q19] 范围查询
来源：http://wap.zdbjq.cn/Article/details/gszajqwfn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.zdbjq.cn/Article/details/gpzyfqwdj.sHtML

[Q20] IN 列表
来源：http://www.blog.zdbjq.cn/Article/details/gsldmovkv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.zdbjq.cn/Article/details/guxauflzl.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/gktaohilb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.hesvh.cn/Article/details/gqwjnhqgt.sHtML

[Q22] 排序
来源：http://www.blog.fehbvm.com/Article/details/gebevjclr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fehbvm.com/Article/details/gperclnoj.sHtML

[Q23] 分页
来源：http://wap.zdbjq.cn/Article/details/gebczenke.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.zdbjq.cn/Article/details/gewedpisb.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/gjmtgkkjd.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/ggsxpraua.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fehbvm.com/Article/details/gshxgypzw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.zdbjq.cn/Article/details/guptntxwg.sHtML

[Q26] 计数
来源：http://blog.fehbvm.com/Article/details/gcwrczfcg.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fehbvm.com/Article/details/gigjncezq.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/grytoespc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.hesvh.cn/Article/details/gpourajie.sHtML

[Q28] 求和与平均
来源：http://baike.hesvh.cn/Article/details/gedlnnroh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gidubvogw.sHtML

[Q29] 最大最小值
来源：http://mobile.zdbjq.cn/Article/details/gipdhzfeb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/guvutbous.sHtML

[Q30] 分组统计
来源：http://www.m.share.zdbjq.cn/Article/details/gmzmdaxdw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/giiuqslyk.sHtML

[Q31] 分组后过滤
来源：http://blog.zdbjq.cn/Article/details/getettdmw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.zdbjq.cn/Article/details/gadghwwyd.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/genmvrvuc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gvwqplqbd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fehbvm.com/Article/details/gynasqukr.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/gnvfdlsty.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fehbvm.com/Article/details/gqubqymrh.sHtML

[Q34] 每组取第一条
来源：http://read.share.fehbvm.com/Article/details/gjhbyzwgh.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/gkcxdvrqz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fehbvm.com/Article/details/ggijxzffn.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gyofbeoyh.sHtML

[Q35] 内连接
来源：http://3g.hesvh.cn/Article/details/gsnmaunli.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gmxlcqcvv.sHtML

[Q36] 左连接
来源：http://m.share.zdbjq.cn/Article/details/ggyxlabla.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gwktophww.sHtML

[Q37] 右连接
来源：http://read.share.hesvh.cn/Article/details/gcynhjusz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/gjktkmaid.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.zdbjq.cn/Article/details/gejngjrtx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fehbvm.com/Article/details/gqpqcigja.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fehbvm.com/Article/details/gpurhzinr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/gqqywpayn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.zdbjq.cn/Article/details/gpjnvwnhf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.zdbjq.cn/Article/details/gfqcgrsgs.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.zdbjq.cn/Article/details/gagrfqwqy.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/ggxqmzhjr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.hesvh.cn/Article/details/gtjkbuukj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fehbvm.com/Article/details/ggpmlqtju.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gprhinxay.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.zdbjq.cn/Article/details/grmamoezs.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fehbvm.com/Article/details/gcokmpwsd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fehbvm.com/Article/details/gudnsvvaq.sHtML

[Q43] 标量子查询
来源：http://read.share.fehbvm.com/Article/details/gduzkwkxs.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.zdbjq.cn/Article/details/gihbuzxyq.sHtML

[Q44] IN 子查询
来源：http://mobile.hesvh.cn/Article/details/gzvtyqiuu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/gmirefgkw.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.hesvh.cn/Article/details/gtbasjpyr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gqarbspqe.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fehbvm.com/Article/details/gyykgstkn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gfxflrxrk.sHtML

[Q47] 与平均值比较
来源：http://www.blog.hesvh.cn/Article/details/gfxzeebag.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.zdbjq.cn/Article/details/ghuuhxdon.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gkntikbns.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.zdbjq.cn/Article/details/gkrfpmjgt.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.hesvh.cn/Article/details/gznnnetgm.sHtML

[Q49] 更新单行
来源：http://read.share.hesvh.cn/Article/details/grmcofhkg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gfwyelije.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/ggmybuoui.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/gkhhallqg.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.hesvh.cn/Article/details/gmgrzqgpv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.zdbjq.cn/Article/details/gepzbiplk.sHtML

[Q52] 删除指定行
来源：http://wap.zdbjq.cn/Article/details/gzugmzuyf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/grmvprmql.sHtML

[Q53] 按条件删除
来源：http://baike.hesvh.cn/Article/details/gjmvvdhbb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fehbvm.com/Article/details/gdtbinscw.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/gfdvcbfcf.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fehbvm.com/Article/details/gvxmkajlv.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/ggweilefi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fehbvm.com/Article/details/gkouktxjf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.hesvh.cn/Article/details/gfhotbhac.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gotgaodvd.sHtML

[Q57] 行号
来源：http://baike.hesvh.cn/Article/details/gedllzvkl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gloqpvfts.sHtML

[Q58] 累计求和
来源：http://baike.fehbvm.com/Article/details/gyoyyldlp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gqawoxsyk.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/gkonyebmt.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/giglkkkyh.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.hesvh.cn/Article/details/guyynkowz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fehbvm.com/Article/details/gmcftzzai.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/gxobydjuz.sHtML

[Q61] 移动平均
来源：http://m.share.fehbvm.com/Article/details/gifhqgkzi.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/ghdrgbdju.sHtML

[Q62] 分组占比
来源：http://www.m.share.zdbjq.cn/Article/details/glfjkqqeg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gwtyjwskk.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/gveoevocp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fehbvm.com/Article/details/grvfpffgx.sHtML

[Q64] 提交事务
来源：http://mobile.hesvh.cn/Article/details/gqhmejzyj.sHtML

COMMIT;
来源：http://baike.fehbvm.com/Article/details/gpysdmxli.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fehbvm.com/Article/details/gmqjwzxgq.sHtML

ROLLBACK;
来源：http://3g.zdbjq.cn/Article/details/gjnrvacis.sHtML

[Q66] 行锁查询
来源：http://wap.hesvh.cn/Article/details/gsnsmpuah.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.zdbjq.cn/Article/details/grdxacvct.sHtML

[Q67] 设置隔离级别
来源：http://wap.zdbjq.cn/Article/details/gkaucfvtl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.zdbjq.cn/Article/details/gelrzjcaq.sHtML

[Q68] 保存点
来源：http://www.m.share.fehbvm.com/Article/details/gtpwuxbak.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/gmvashjnb.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fehbvm.com/Article/details/gpwxsbhva.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.hesvh.cn/Article/details/gxirifdjy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.zdbjq.cn/Article/details/gebbgmtyo.sHtML

[Q70] 更新统计信息
来源：http://baike.hesvh.cn/Article/details/ginxijbjq.sHtML

ANALYZE TABLE users;
来源：http://3g.zdbjq.cn/Article/details/gbgvtptpa.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.hesvh.cn/Article/details/gckccylwk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.zdbjq.cn/Article/details/gjzvmojqo.sHtML

[Q72] 查看索引
来源：http://www.share.hesvh.cn/Article/details/gspjqjrpv.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/grulyzili.sHtML

[Q73] 查看表状态
来源：http://baike.hesvh.cn/Article/details/ghgasgobm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.zdbjq.cn/Article/details/gzvdtaozx.sHtML

[Q74] 强制使用索引
来源：http://read.share.zdbjq.cn/Article/details/gnlfcxkpw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/gvzrrogjc.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/ggjxdnqzh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gslfznrya.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.zdbjq.cn/Article/details/gfkjkffsy.sHtML

[Q76] 按天统计
来源：http://www.blog.fehbvm.com/Article/details/gqgcyhvaz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fehbvm.com/Article/details/gfladhvbe.sHtML

[Q77] 时间加减
来源：http://mobile.hesvh.cn/Article/details/gxbwzwjbu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.zdbjq.cn/Article/details/gofqzljag.sHtML

[Q78] 当前时间
来源：http://m.share.fehbvm.com/Article/details/gplxfdqkh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fehbvm.com/Article/details/gukqlpcrr.sHtML

[Q79] 字符串拼接
来源：http://wap.hesvh.cn/Article/details/gyogrsqvs.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.hesvh.cn/Article/details/gorrqrsrz.sHtML

[Q80] 字符串截取
来源：http://blog.fehbvm.com/Article/details/ggtkxoukl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gnasqqqkr.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/ghoqnwfgo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.hesvh.cn/Article/details/gqpugmziy.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.zdbjq.cn/Article/details/gyhybtfvi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gxaafxeyo.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gwoqujvon.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gptdeugsx.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/gpgisrxlw.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gyzzsmbya.sHtML

[Q85] 数值取整
来源：http://www.blog.hesvh.cn/Article/details/gphccdfxp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/gflgvwkjj.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/ggfwjfomt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fehbvm.com/Article/details/ghbehbgcy.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.hesvh.cn/Article/details/galgxdeyh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/geqrgcdij.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/gqqdizenq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gckxxypon.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fehbvm.com/Article/details/gzuvqogut.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/gbkxqhhge.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/gabyubopj.sHtML

[Q90] 生成序号列
来源：http://blog.zdbjq.cn/Article/details/gkcrguztn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/gcllanyif.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ggauciunh.sHtML

R. Bash 专题
来源：http://wap.hesvh.cn/Article/details/glwdmsboa.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gngdneiwq.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/geduymbrq.sHtML

#!/usr/bin/env bash
来源：http://3g.zdbjq.cn/Article/details/gmackgknu.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/gbelimfiv.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/gtvwyczwd.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/gwtrwvupv.sHtML

[R03] 只读变量
来源：http://www.blog.fehbvm.com/Article/details/gstbhkrao.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/gfkvlvaea.sHtML

[R04] 位置参数
来源：http://3g.zdbjq.cn/Article/details/gbyowfcye.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/gnmtthtte.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gehvlzhod.sHtML

name="${1:-default}"
来源：http://www.blog.hesvh.cn/Article/details/gcoirsqeq.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/gxeizzvei.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/grwgbeubs.sHtML

[R07] if 判断文件
来源：http://mobile.fehbvm.com/Article/details/gggvwjiru.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gmdtrqcak.sHtML

[R08] 数值比较
来源：http://mobile.hesvh.cn/Article/details/gmgupamnb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gypgixfsc.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gsmjaozmq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/guuuvjozv.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/guetguurl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fehbvm.com/Article/details/gjayvmolv.sHtML

[R11] case 多分支
来源：http://blog.hesvh.cn/Article/details/gxkfdrudh.sHtML

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/gebmklgyk.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/guujodely.sHtML

stop)  echo "停止" ;;
来源：http://baike.hesvh.cn/Article/details/gclgwjjmb.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gcddxlbch.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/gowhipnql.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/garzcbqlw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/gdrhloing.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gmzyeymvg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/ghumchozz.sHtML

[R14] C 风格 for
来源：http://mobile.zdbjq.cn/Article/details/gwpdohgpb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gqnzmpclg.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gtjzekkze.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/gcarzpzol.sHtML

[R16] until 等待条件
来源：http://3g.hesvh.cn/Article/details/gveaoyizq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gnbkqfrey.sHtML

[R17] 数组定义与取值
来源：http://m.share.zdbjq.cn/Article/details/gyydttzqh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/glipcwknr.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/gbvvssiyv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/gtxgxsyid.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/giipopoey.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/gpwsuukvn.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/garjyijxt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.zdbjq.cn/Article/details/gczswhfeo.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gjklzscbd.sHtML

echo "${#s}"
来源：http://m.share.zdbjq.cn/Article/details/guvcyikll.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/gmxrphssg.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/guwpzboqn.sHtML

[R23] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gnojokthh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/ghsbiiqbo.sHtML

[R24] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/givjwxpcm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.hesvh.cn/Article/details/gzgqhrnpk.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.hesvh.cn/Article/details/ghcfxtjul.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fehbvm.com/Article/details/gagzqyzgf.sHtML

[R26] 命令替换
来源：http://www.m.share.zdbjq.cn/Article/details/gijccurea.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/giubsryyz.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/gezwdpfur.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/gbkklgxfc.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/gypcbpvew.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fehbvm.com/Article/details/gijodscfu.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gfmdghjia.sHtML


<!-- 参考信息 -->