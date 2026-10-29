代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/grzahiset.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.zdbjq.cn/Article/details/gptixptsb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gwczcbzvf.sHtML

Ruby: a == b
来源：http://m.share.zdbjq.cn/Article/details/gablagusr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.zdbjq.cn/Article/details/gecqtimjo.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.hesvh.cn/Article/details/glryovhfw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/gkupyqfnn.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fehbvm.com/Article/details/garukzwew.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.zdbjq.cn/Article/details/gsntykioj.sHtML

TS:   if (x == null) {}
来源：http://www.share.hesvh.cn/Article/details/gpefyxwuh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gjjqvndwu.sHtML

Go:   if x == nil {}
来源：http://3g.fehbvm.com/Article/details/gemcugubo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.zdbjq.cn/Article/details/gqpkcuete.sHtML

C#:   if (x is null) {}
来源：http://baike.zdbjq.cn/Article/details/geixuypdo.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/ggcreuzim.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/gxfxxjvle.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.hesvh.cn/Article/details/glyplfpia.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/ghfdpfmke.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gsdjglmxl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.zdbjq.cn/Article/details/ggggxnlbo.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fehbvm.com/Article/details/gdogqluos.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/gfimdsdpp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.hesvh.cn/Article/details/guilktjsm.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/givmeyspr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.hesvh.cn/Article/details/gnkqslbsj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.hesvh.cn/Article/details/gdofowjsm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/glpvevbyy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gcvvxfvoj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.fehbvm.com/Article/details/gfixadtke.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fehbvm.com/Article/details/gnsdslelj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fehbvm.com/Article/details/gynyswsce.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.hesvh.cn/Article/details/gbydzdpon.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gdgomisib.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/gwbuefirg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtnegzmhe.sHtML

[Q01] 创建表
来源：http://mobile.fehbvm.com/Article/details/guerjmezp.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/gbidhhtvu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gtdnyemyo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gpywkktfn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/gmrhsemok.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fehbvm.com/Article/details/gpnbslhon.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gkvegkzmy.sHtML

[Q02] 创建带外键的表
来源：http://baike.hesvh.cn/Article/details/gpfpuegfs.sHtML

CREATE TABLE orders (
来源：http://www.blog.hesvh.cn/Article/details/gsfeeqbpp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gxlxateqz.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gnkdumukr.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.hesvh.cn/Article/details/gsbhfdmip.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.hesvh.cn/Article/details/ghfrhailr.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/ghasnknvb.sHtML

[Q03] 增加列
来源：http://mobile.zdbjq.cn/Article/details/gantoseyo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.zdbjq.cn/Article/details/gvonlmdsy.sHtML

[Q04] 修改列类型
来源：http://www.blog.fehbvm.com/Article/details/gbgsvzzzd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.zdbjq.cn/Article/details/grlmajdxl.sHtML

[Q05] 重命名列
来源：http://m.share.zdbjq.cn/Article/details/gnqxmaflo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.zdbjq.cn/Article/details/gcfaonltc.sHtML

[Q06] 删除列
来源：http://blog.fehbvm.com/Article/details/gcaqhnnsk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.hesvh.cn/Article/details/gcwginfzv.sHtML

[Q07] 删除表
来源：http://read.share.fehbvm.com/Article/details/gtnhgzfnn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.zdbjq.cn/Article/details/gscijwbnk.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/gioikhtcf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/grqdowyom.sHtML

[Q09] 创建唯一索引
来源：http://read.share.hesvh.cn/Article/details/gvxmjwwqi.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gcllgqsij.sHtML

[Q10] 插入单行
来源：http://3g.hesvh.cn/Article/details/gbwpnhjub.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gimcoduvi.sHtML

[Q11] 一次插入多行
来源：http://baike.hesvh.cn/Article/details/gdseuuwbt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fehbvm.com/Article/details/gxoeodmqq.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/gnrajwpfa.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/gehvviarm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/gtbyfkhrc.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/ghazbgzyp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/gjjiilaep.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fehbvm.com/Article/details/gviggfabp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.zdbjq.cn/Article/details/gsejwbnvq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/geqiplkcn.sHtML

[Q15] 查询全部
来源：http://mobile.zdbjq.cn/Article/details/gtqvhwtyt.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/gwiqxyqnt.sHtML

[Q16] 查询指定列
来源：http://www.share.zdbjq.cn/Article/details/guqtisknn.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ghvbvdvsd.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/ghhlxfokh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fehbvm.com/Article/details/gkjixirso.sHtML

[Q18] 模糊匹配
来源：http://baike.zdbjq.cn/Article/details/gyxhtkbvs.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fehbvm.com/Article/details/ghhcylbxd.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/gpmuohzwc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/gtpavefjq.sHtML

[Q20] IN 列表
来源：http://baike.hesvh.cn/Article/details/gavgkpztr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gngmtsxty.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/gsgndxnha.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/gonvcxuhm.sHtML

[Q22] 排序
来源：http://m.share.hesvh.cn/Article/details/gxbfccmmy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/gkhgpwpwl.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/gdfuvhgab.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/gtyqdjvrb.sHtML

[Q24] 去重
来源：http://www.blog.fehbvm.com/Article/details/glrzrndpr.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gokpszops.sHtML

[Q25] 只取前 N 条
来源：http://read.share.hesvh.cn/Article/details/gnjbmgqzr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.zdbjq.cn/Article/details/gbtqhfert.sHtML

[Q26] 计数
来源：http://wap.hesvh.cn/Article/details/gzgcfjdlx.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gnajjmpzx.sHtML

[Q27] 条件计数
来源：http://wap.zdbjq.cn/Article/details/ghgnvtbhg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gffmkocjd.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fehbvm.com/Article/details/gqxhybawk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.hesvh.cn/Article/details/glkfrwvkr.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/gbbhzkqsl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.hesvh.cn/Article/details/gkdrxbvmw.sHtML

[Q30] 分组统计
来源：http://m.share.hesvh.cn/Article/details/glbduzisv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/ghsmkthxo.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/gqceuolyx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fehbvm.com/Article/details/gimccuhqm.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fehbvm.com/Article/details/gvrzdnzno.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gjzculqae.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.hesvh.cn/Article/details/gnathcynk.sHtML

[Q33] 多列分组
来源：http://m.share.zdbjq.cn/Article/details/gsvrmrnts.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fehbvm.com/Article/details/gjfsugkxo.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/ghllvwzpg.sHtML

SELECT * FROM (
来源：http://wap.zdbjq.cn/Article/details/gdeohypor.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.zdbjq.cn/Article/details/gmqemrhsf.sHtML

) t WHERE rn = 1;
来源：http://wap.fehbvm.com/Article/details/gyvgcedrf.sHtML

[Q35] 内连接
来源：http://www.m.share.zdbjq.cn/Article/details/gptzmwegd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gqkcyrlet.sHtML

[Q36] 左连接
来源：http://blog.zdbjq.cn/Article/details/gnvdtyvbp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gcpxpckom.sHtML

[Q37] 右连接
来源：http://www.blog.hesvh.cn/Article/details/gvypbswrd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.hesvh.cn/Article/details/gprfhkudn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.zdbjq.cn/Article/details/gflzebwzk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.hesvh.cn/Article/details/gsurvyhsf.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/gqgyqxelh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/gkkfjskyn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gdxxaxeir.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.hesvh.cn/Article/details/gfjxwlhms.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fehbvm.com/Article/details/gomjiwyxo.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/gtsgtpjpn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.zdbjq.cn/Article/details/gileqjqyf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.hesvh.cn/Article/details/gdklzzahx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.hesvh.cn/Article/details/gxynwalxq.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/gvtmaqmvt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.hesvh.cn/Article/details/gpvejgzkp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.hesvh.cn/Article/details/guhvtvgek.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/gkchfkkcn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/gdppsyoso.sHtML

[Q44] IN 子查询
来源：http://www.share.zdbjq.cn/Article/details/ghnifokvv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.zdbjq.cn/Article/details/gtqlmdotj.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.zdbjq.cn/Article/details/gbxgdckqq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gbhibinlf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/gkxvopwex.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gohowdyup.sHtML

[Q47] 与平均值比较
来源：http://blog.hesvh.cn/Article/details/ghhgglucg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.hesvh.cn/Article/details/gkdajneat.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/gyechnnvb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.zdbjq.cn/Article/details/gxxhuisuj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.hesvh.cn/Article/details/gvgdfsxdw.sHtML

[Q49] 更新单行
来源：http://read.share.zdbjq.cn/Article/details/gazxomqug.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/ghomubcma.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/geohmnkzz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fehbvm.com/Article/details/giwbasrxg.sHtML

[Q51] 用子查询更新
来源：http://www.share.hesvh.cn/Article/details/ghlsojtva.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/goqmgbhjf.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/gdnympdqm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gwsoyclka.sHtML

[Q53] 按条件删除
来源：http://m.share.hesvh.cn/Article/details/gmnwwcoid.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.hesvh.cn/Article/details/gjdfwoldn.sHtML

[Q54] 清空表
来源：http://m.share.hesvh.cn/Article/details/gmffewgvx.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/gfxrhmnxz.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.zdbjq.cn/Article/details/ginwithzm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gawksydda.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.zdbjq.cn/Article/details/gnfxfgnal.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fehbvm.com/Article/details/grlkhkboh.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/gxwmwpvkf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.zdbjq.cn/Article/details/ggnmrcvpc.sHtML

[Q58] 累计求和
来源：http://m.share.fehbvm.com/Article/details/gyufgxtmi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gdjggovzu.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/gnpxqpfcg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/ghuhvznjg.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.zdbjq.cn/Article/details/gipyarfrn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fehbvm.com/Article/details/gteyuzplc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/ginvdyjeu.sHtML

[Q61] 移动平均
来源：http://mobile.fehbvm.com/Article/details/gkpmozlvf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gyhrtgkxw.sHtML

[Q62] 分组占比
来源：http://blog.zdbjq.cn/Article/details/gybdcdpmy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gfmlahsrv.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/gelpyzsdc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fehbvm.com/Article/details/gwqqiujrw.sHtML

[Q64] 提交事务
来源：http://mobile.hesvh.cn/Article/details/giujjbliy.sHtML

COMMIT;
来源：http://www.m.share.zdbjq.cn/Article/details/gduxojkra.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/gypqgjerr.sHtML

ROLLBACK;
来源：http://baike.zdbjq.cn/Article/details/gfozjljeg.sHtML

[Q66] 行锁查询
来源：http://www.share.hesvh.cn/Article/details/gndagvvud.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.hesvh.cn/Article/details/gqicfeimh.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fehbvm.com/Article/details/ghvozpxni.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.zdbjq.cn/Article/details/gdraiobcv.sHtML

[Q68] 保存点
来源：http://read.share.fehbvm.com/Article/details/gsfuufwaq.sHtML

SAVEPOINT sp1;
来源：http://read.share.zdbjq.cn/Article/details/gebxnejys.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/gaikyjhnw.sHtML

[Q69] 查看执行计划
来源：http://baike.zdbjq.cn/Article/details/guhxqjwvq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fehbvm.com/Article/details/gapqbtxbu.sHtML

[Q70] 更新统计信息
来源：http://wap.zdbjq.cn/Article/details/gjxogpnsk.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/gzcofffvw.sHtML

[Q71] 查看建表语句
来源：http://mobile.fehbvm.com/Article/details/gphbjosgr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.zdbjq.cn/Article/details/gmjzdjbgg.sHtML

[Q72] 查看索引
来源：http://3g.hesvh.cn/Article/details/gephcvdga.sHtML

SHOW INDEX FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gyieydqic.sHtML

[Q73] 查看表状态
来源：http://read.share.fehbvm.com/Article/details/gdbigkqkp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/ggelygneo.sHtML

[Q74] 强制使用索引
来源：http://baike.zdbjq.cn/Article/details/gimnsojxt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.zdbjq.cn/Article/details/gkhokgokf.sHtML

[Q75] 日期格式化
来源：http://wap.fehbvm.com/Article/details/ganqzctab.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/gabhavafp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.hesvh.cn/Article/details/glboqfkxu.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/gwiovnipn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.hesvh.cn/Article/details/gzpbjdnno.sHtML

[Q77] 时间加减
来源：http://baike.fehbvm.com/Article/details/gqlnnunsg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fehbvm.com/Article/details/gjfwmlxdk.sHtML

[Q78] 当前时间
来源：http://blog.fehbvm.com/Article/details/gybubrgzw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/gwsmmgbdy.sHtML

[Q79] 字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gwlevhhlf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/gptpspqtj.sHtML

[Q80] 字符串截取
来源：http://blog.zdbjq.cn/Article/details/gabnaaqrw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gtayoafog.sHtML

[Q81] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gguejhtgx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.hesvh.cn/Article/details/ggzgwdgzj.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.hesvh.cn/Article/details/gjdrtscoa.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/glaxdmwdx.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gmllhrdhc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/glyvfpyor.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/glmtxubhk.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/ghwfclxga.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/gcvqaorpj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.zdbjq.cn/Article/details/gkmvqygjt.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fehbvm.com/Article/details/gcvvoihuc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.hesvh.cn/Article/details/gzjrczwfb.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.zdbjq.cn/Article/details/gitwgrjtc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/gyuqaesyv.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.zdbjq.cn/Article/details/gtmjajaqg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.hesvh.cn/Article/details/gckrojydu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/giddottni.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/gowkzihgp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/ginovduuz.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gfzamlkzo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.hesvh.cn/Article/details/gltjtgorn.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gybcleddc.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/gdpnmfddr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gixiprgko.sHtML

[R01] shebang 与严格模式
来源：http://wap.fehbvm.com/Article/details/gricndiqi.sHtML

#!/usr/bin/env bash
来源：http://blog.hesvh.cn/Article/details/gvgyvmhdz.sHtML

set -euo pipefail
来源：http://wap.fehbvm.com/Article/details/gajeltvhs.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.hesvh.cn/Article/details/gdxmrnoeq.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.hesvh.cn/Article/details/gbdivsnbm.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/gashkletm.sHtML

readonly PI=3.14
来源：http://baike.hesvh.cn/Article/details/gvoxsgvee.sHtML

[R04] 位置参数
来源：http://www.blog.zdbjq.cn/Article/details/gteubvsbl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.hesvh.cn/Article/details/gunrsxnww.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/gxsxoblpc.sHtML

name="${1:-default}"
来源：http://blog.zdbjq.cn/Article/details/gnivbaxkn.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/gmtfadodc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gacwtxypd.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/guystoznm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/gqcqqiknt.sHtML

[R08] 数值比较
来源：http://3g.hesvh.cn/Article/details/gujukhbvf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fehbvm.com/Article/details/gxgmroeoz.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/gezxrgtkf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/gnxvcrrti.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/ggjcfwdeb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.hesvh.cn/Article/details/gtsxkubrm.sHtML

[R11] case 多分支
来源：http://www.m.share.fehbvm.com/Article/details/gkccjpqoo.sHtML

case "$1" in
来源：http://www.share.fehbvm.com/Article/details/gsbijjntx.sHtML

start) echo "启动" ;;
来源：http://read.share.fehbvm.com/Article/details/gkpzbpdfa.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/gxnneavoy.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.zdbjq.cn/Article/details/gjdqjqzqs.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gmjnxxrck.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/gojipdthf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/gcwxklyjc.sHtML

[R13] for 计数循环
来源：http://wap.fehbvm.com/Article/details/gwjenxwav.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gdhbemzuw.sHtML

[R14] C 风格 for
来源：http://wap.fehbvm.com/Article/details/gnnwtsqgh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gvjtujdox.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gsojdvlhl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/gvhbthnze.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/gpjbkixnr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/grqvcttyd.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gdpgsbpto.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/gvroguzsq.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/gkzsjtfis.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fehbvm.com/Article/details/glwehdgvv.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/gqzpmngni.sHtML

echo "${#arr[@]}"
来源：http://www.blog.zdbjq.cn/Article/details/gjlanljjp.sHtML

[R20] 关联数组（字典）
来源：http://www.share.hesvh.cn/Article/details/gmicafxrx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/gvzkltvlv.sHtML

[R21] 字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gonokwutd.sHtML

echo "${#s}"
来源：http://www.share.hesvh.cn/Article/details/gywgcqcdw.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/gsyqsdxxr.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fehbvm.com/Article/details/gvjzsdgkw.sHtML

[R23] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gxnkwxxpy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/gauyldurj.sHtML

[R24] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gbpncduhl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/glividvvu.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fehbvm.com/Article/details/gduilnodz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/gbllwmcyg.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/gpwkddqro.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/geqspxbsc.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/gjbmkuvnn.sHtML


<!-- 参考信息 -->