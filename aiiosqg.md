代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://wap.zdbjq.cn/Article/details/ggtonkrzw.sHtML

Go:   len(arr);  len(m)
来源：http://wap.hesvh.cn/Article/details/gxfuxmecf.sHtML

Ruby: x.length;  x.size
来源：http://read.share.zdbjq.cn/Article/details/gaofyrnkr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/gyzwsekvb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/gjnlzognm.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fehbvm.com/Article/details/gbrphgopx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fehbvm.com/Article/details/geedpsdnk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.hesvh.cn/Article/details/gvoxoahvq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gqjaaydmt.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fehbvm.com/Article/details/gzkxofxug.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gghibcpwr.sHtML

Ruby: a == b
来源：http://mobile.hesvh.cn/Article/details/gvrzqsnwi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/gskpyksol.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/gjdvqpevh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.zdbjq.cn/Article/details/grufyiogq.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/gqrxbrdbw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.zdbjq.cn/Article/details/gvigmetqs.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwdjesdwd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gbccousng.sHtML

Go:   if x == nil {}
来源：http://www.blog.fehbvm.com/Article/details/gicpaeiuh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/glivtkscy.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gghpysgao.sHtML

[P07] 防抖与节流
来源：http://read.share.zdbjq.cn/Article/details/gdenzvyib.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/gcrchtple.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.hesvh.cn/Article/details/gpssfdwog.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/grvcfnivi.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gvjupkvms.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.zdbjq.cn/Article/details/glnjvpwuo.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/gjarvhcpr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.zdbjq.cn/Article/details/gvdukagrs.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.zdbjq.cn/Article/details/gevsawcax.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.zdbjq.cn/Article/details/gsqttwpqe.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.zdbjq.cn/Article/details/gpyflyoqq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/grtuqvgfx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/gbnzwakox.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/gcthmqknx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.zdbjq.cn/Article/details/gokscscfq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.hesvh.cn/Article/details/gydeaxxox.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.zdbjq.cn/Article/details/gluahmuiy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/gdmieiaul.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbabamsgt.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fehbvm.com/Article/details/gvlelsonm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcwcqumvw.sHtML

[Q01] 创建表
来源：http://read.share.zdbjq.cn/Article/details/gjtxscsli.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/gvfdcfmxo.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gsqbcwwco.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gwapyrtsr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.hesvh.cn/Article/details/gskhzgfjd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.hesvh.cn/Article/details/gehllduec.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gvvngwpqa.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fehbvm.com/Article/details/gnzsjiozk.sHtML

CREATE TABLE orders (
来源：http://mobile.zdbjq.cn/Article/details/gffjimorw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gcdaakdaf.sHtML

user_id INT NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gsjmservu.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fehbvm.com/Article/details/gfuqqntio.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.zdbjq.cn/Article/details/gxmalbnda.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gawdogekl.sHtML

[Q03] 增加列
来源：http://read.share.hesvh.cn/Article/details/gxgtsactg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.zdbjq.cn/Article/details/gerrgoibw.sHtML

[Q04] 修改列类型
来源：http://3g.zdbjq.cn/Article/details/gkwlaxtyx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.hesvh.cn/Article/details/gkqdsnfsw.sHtML

[Q05] 重命名列
来源：http://blog.zdbjq.cn/Article/details/gbjreijbm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.hesvh.cn/Article/details/gezrcwkkm.sHtML

[Q06] 删除列
来源：http://wap.fehbvm.com/Article/details/gevxxmnsz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fehbvm.com/Article/details/gbhwrgzrj.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/ghjjvuplx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.zdbjq.cn/Article/details/gzzuimzvy.sHtML

[Q08] 创建普通索引
来源：http://www.share.fehbvm.com/Article/details/gkimedoci.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gxxapzzpd.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/gdaaqnave.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gisckjmct.sHtML

[Q10] 插入单行
来源：http://mobile.hesvh.cn/Article/details/gobdxznlb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.hesvh.cn/Article/details/gffxsvucu.sHtML

[Q11] 一次插入多行
来源：http://wap.hesvh.cn/Article/details/gafoahsuq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gqrqmxsip.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.hesvh.cn/Article/details/gvojvwctj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.hesvh.cn/Article/details/gckfcnbwu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.zdbjq.cn/Article/details/gfdvnsscw.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/gxilzlify.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gcdkikdua.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.zdbjq.cn/Article/details/gyuepeqfr.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/gxbsllcqn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.zdbjq.cn/Article/details/gqiislpuu.sHtML

[Q15] 查询全部
来源：http://www.m.share.fehbvm.com/Article/details/gppmzkalg.sHtML

SELECT * FROM users;
来源：http://blog.fehbvm.com/Article/details/gjwwefcsb.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/gbgktlesd.sHtML

SELECT id, name FROM users;
来源：http://www.share.fehbvm.com/Article/details/grqvmcagp.sHtML

[Q17] 条件查询
来源：http://www.blog.fehbvm.com/Article/details/gozjdpulx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gcgslnyer.sHtML

[Q18] 模糊匹配
来源：http://read.share.zdbjq.cn/Article/details/getmukeer.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fehbvm.com/Article/details/gkoaukbqu.sHtML

[Q19] 范围查询
来源：http://www.share.fehbvm.com/Article/details/gzjiattnz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fehbvm.com/Article/details/gcfgfrihy.sHtML

[Q20] IN 列表
来源：http://mobile.zdbjq.cn/Article/details/gasacatvf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/gwsynnlyy.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/gfowkxwit.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.hesvh.cn/Article/details/ggucfmntz.sHtML

[Q22] 排序
来源：http://baike.zdbjq.cn/Article/details/gvqtqdqab.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.hesvh.cn/Article/details/gkmuvefda.sHtML

[Q23] 分页
来源：http://wap.zdbjq.cn/Article/details/gjencqwdy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fehbvm.com/Article/details/glwqskmhf.sHtML

[Q24] 去重
来源：http://mobile.fehbvm.com/Article/details/gbtbjaygo.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.zdbjq.cn/Article/details/grfgnowmc.sHtML

[Q25] 只取前 N 条
来源：http://baike.hesvh.cn/Article/details/gtctitgho.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/guiqfykjq.sHtML

[Q26] 计数
来源：http://www.blog.fehbvm.com/Article/details/guiljctbg.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fehbvm.com/Article/details/gpollqwqk.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/gwoejofod.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/gylfgomjm.sHtML

[Q28] 求和与平均
来源：http://blog.zdbjq.cn/Article/details/gtxqxhtxc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gyoumsqey.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/gvzzfropb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.hesvh.cn/Article/details/goqwexiif.sHtML

[Q30] 分组统计
来源：http://mobile.hesvh.cn/Article/details/gqgeqisic.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gmefeuxek.sHtML

[Q31] 分组后过滤
来源：http://baike.zdbjq.cn/Article/details/gaklqcteq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.hesvh.cn/Article/details/gqecmrmif.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gmxsxuxzk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gzelccnrc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/gqnjgoiwm.sHtML

[Q33] 多列分组
来源：http://www.blog.zdbjq.cn/Article/details/gpdcjvkya.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fehbvm.com/Article/details/gnakgfjfs.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/gnzihpock.sHtML

SELECT * FROM (
来源：http://www.share.zdbjq.cn/Article/details/gaqmcsgdu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.hesvh.cn/Article/details/gfjksqbeg.sHtML

) t WHERE rn = 1;
来源：http://3g.zdbjq.cn/Article/details/gmhirfsdg.sHtML

[Q35] 内连接
来源：http://m.share.hesvh.cn/Article/details/gwigrmztu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gjojkkrdw.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/gbaubunip.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gvtezcccu.sHtML

[Q37] 右连接
来源：http://blog.zdbjq.cn/Article/details/gsmsmyebe.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.hesvh.cn/Article/details/gvctizglf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.hesvh.cn/Article/details/gbiibmcer.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fehbvm.com/Article/details/gosyobvcx.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.zdbjq.cn/Article/details/gtjpjvvnm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/gkeejyqha.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.zdbjq.cn/Article/details/giprkmolt.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/grexeemhe.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.hesvh.cn/Article/details/ggasxbiju.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/gsrsffrfh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fehbvm.com/Article/details/gtvpmbukd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/gnxqepmzk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/gikxaewvm.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.hesvh.cn/Article/details/gxkndtrgo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.hesvh.cn/Article/details/gtbycvbuq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fehbvm.com/Article/details/gecabnxnk.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/gewquiafz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/gffumzzwf.sHtML

[Q44] IN 子查询
来源：http://blog.zdbjq.cn/Article/details/gqwzwsyxg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.zdbjq.cn/Article/details/gwtznwwel.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/gydwjpsdz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gpsrgeezs.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/ghehvjdqh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gzmjnrfbx.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/gdmgrwjlt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.zdbjq.cn/Article/details/gmrqtaubg.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.hesvh.cn/Article/details/gkcvjqcfn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fehbvm.com/Article/details/grjvrtvqk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gxcewkdfb.sHtML

[Q49] 更新单行
来源：http://mobile.hesvh.cn/Article/details/gjpqqpjjb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/grwttwavr.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gcpdybtid.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.hesvh.cn/Article/details/grgwmgojr.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/gllduixtx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.zdbjq.cn/Article/details/gfguptchc.sHtML

[Q52] 删除指定行
来源：http://baike.fehbvm.com/Article/details/gpihjsmhv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/grvemrkrn.sHtML

[Q53] 按条件删除
来源：http://baike.zdbjq.cn/Article/details/ggmwrtpsp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/gginevxvk.sHtML

[Q54] 清空表
来源：http://wap.zdbjq.cn/Article/details/gwfnhbylf.sHtML

TRUNCATE TABLE logs;
来源：http://blog.zdbjq.cn/Article/details/ghfskfnwk.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.zdbjq.cn/Article/details/gwfnptzfy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fehbvm.com/Article/details/gipfslmbo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fehbvm.com/Article/details/gyobwlpss.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gbupzyoyr.sHtML

[Q57] 行号
来源：http://www.m.share.hesvh.cn/Article/details/goixetchr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/guxhpkuyg.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gtqqsdtuz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gwcptcrzn.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/gnmrywwof.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gvmlzsbyz.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.hesvh.cn/Article/details/guwvxcily.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/gvuqvtmwf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gmnizxirh.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/ghhtdtril.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.hesvh.cn/Article/details/grhjxizeu.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/gpxxjyaqk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/glvbwvdfd.sHtML

[Q63] 开启事务
来源：http://read.share.fehbvm.com/Article/details/gewcibouw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fehbvm.com/Article/details/goohbqbho.sHtML

[Q64] 提交事务
来源：http://www.m.share.fehbvm.com/Article/details/gsxftrkwt.sHtML

COMMIT;
来源：http://www.m.share.fehbvm.com/Article/details/grynzaeqa.sHtML

[Q65] 回滚事务
来源：http://mobile.zdbjq.cn/Article/details/gtwblbrgb.sHtML

ROLLBACK;
来源：http://blog.hesvh.cn/Article/details/glnuxirpu.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/ghytvsjuq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fehbvm.com/Article/details/gpkyljlyp.sHtML

[Q67] 设置隔离级别
来源：http://baike.fehbvm.com/Article/details/gmwaugdns.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.zdbjq.cn/Article/details/gfhhpqccz.sHtML

[Q68] 保存点
来源：http://www.m.share.fehbvm.com/Article/details/ggwzhupiq.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/gjcdcwotq.sHtML

ROLLBACK TO sp1;
来源：http://read.share.zdbjq.cn/Article/details/gmbbcqfjp.sHtML

[Q69] 查看执行计划
来源：http://baike.fehbvm.com/Article/details/gaaladedo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.hesvh.cn/Article/details/gsootnbqi.sHtML

[Q70] 更新统计信息
来源：http://www.blog.zdbjq.cn/Article/details/glyuaeoex.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.zdbjq.cn/Article/details/gbhgllkxj.sHtML

[Q71] 查看建表语句
来源：http://mobile.hesvh.cn/Article/details/gorquxvsh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.zdbjq.cn/Article/details/ganttjbhj.sHtML

[Q72] 查看索引
来源：http://www.share.hesvh.cn/Article/details/gnzngvqec.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gricrcqfi.sHtML

[Q73] 查看表状态
来源：http://m.share.fehbvm.com/Article/details/giikcvcob.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.zdbjq.cn/Article/details/gsbnzusyf.sHtML

[Q74] 强制使用索引
来源：http://baike.hesvh.cn/Article/details/garaenuen.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fehbvm.com/Article/details/gtbufmqln.sHtML

[Q75] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gdemovhpz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gibrstxrk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/gtvcluhxk.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/ghtykhozp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.zdbjq.cn/Article/details/ghhrdqohq.sHtML

[Q77] 时间加减
来源：http://www.m.share.fehbvm.com/Article/details/gqlebvqkf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fehbvm.com/Article/details/ggwrkdbty.sHtML

[Q78] 当前时间
来源：http://3g.hesvh.cn/Article/details/gtfdnbcgs.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fehbvm.com/Article/details/gmxrlucgp.sHtML

[Q79] 字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gctmdmtzo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/gpfinzxbs.sHtML

[Q80] 字符串截取
来源：http://blog.hesvh.cn/Article/details/gmpsvrzpr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gfjdlbrti.sHtML

[Q81] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gpnvlnvvc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.hesvh.cn/Article/details/gsjpfveer.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/gjjrhyshz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gzdwhwjax.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/giuxrbbyb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/getjnpuoo.sHtML

[Q84] 去除首尾空格
来源：http://www.share.zdbjq.cn/Article/details/gxaqepxbv.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gmjgeqcna.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/gngnczpfc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.hesvh.cn/Article/details/grmwffmzz.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.zdbjq.cn/Article/details/gmuvdyxjd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fehbvm.com/Article/details/gtjcrjvxx.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gazfmztmd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/gogohqsvj.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.hesvh.cn/Article/details/gqstyayem.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/gmjgwoaph.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.hesvh.cn/Article/details/glorgisxe.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/gzuvgdtyg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/gosbvfrxt.sHtML

[Q90] 生成序号列
来源：http://read.share.zdbjq.cn/Article/details/gqoxgyhmw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.hesvh.cn/Article/details/gfucvvixw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvyhwcqkl.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/gwjatbkkk.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gegoshsbr.sHtML

[R01] shebang 与严格模式
来源：http://m.share.hesvh.cn/Article/details/gnqlajsho.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/gyubwrvny.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gjwnerwrm.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/gnsoabqzd.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/gojladhvz.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/gdozjifgf.sHtML

readonly PI=3.14
来源：http://wap.fehbvm.com/Article/details/gudrjqdkt.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/gvghfcskt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/giikezdcy.sHtML

[R05] 参数默认值
来源：http://www.share.zdbjq.cn/Article/details/gqgqwsmwj.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/gawcmtjzy.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/gmiebdpaz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gyxwagghe.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gscrwbnye.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/gpekspwpz.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/gkuehiari.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gvfriapvy.sHtML

[R09] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gsfzgzfxr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gzjypdtam.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/gpexzqeqv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/gqdfuzhfk.sHtML

[R11] case 多分支
来源：http://blog.fehbvm.com/Article/details/ghwtlblfj.sHtML

case "$1" in
来源：http://m.share.fehbvm.com/Article/details/ghqbzmoyt.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/gtlqesunh.sHtML

stop)  echo "停止" ;;
来源：http://read.share.zdbjq.cn/Article/details/gyjxgggil.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gwaofxgki.sHtML

esac
来源：http://read.share.fehbvm.com/Article/details/gmwonudqt.sHtML

[R12] for 遍历文件
来源：http://baike.zdbjq.cn/Article/details/grdiombta.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/gzrjwoyuy.sHtML

[R13] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/guboautto.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gqorbfbsr.sHtML

[R14] C 风格 for
来源：http://read.share.zdbjq.cn/Article/details/gailgllur.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gtnpxgktz.sHtML

[R15] while 逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gbjhsjoqb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.hesvh.cn/Article/details/guvblcnyr.sHtML

[R16] until 等待条件
来源：http://baike.hesvh.cn/Article/details/gjhedbzrf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gtdbhqgfx.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/gfbuyatep.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/galueqabz.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/goiuiyzjk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.hesvh.cn/Article/details/gfgvulgrm.sHtML

[R19] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gimoxlsmu.sHtML

echo "${#arr[@]}"
来源：http://baike.hesvh.cn/Article/details/gyluoihdr.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/ggdawtgqb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/ggtoohdro.sHtML

[R21] 字符串长度
来源：http://3g.hesvh.cn/Article/details/gxdyykwnc.sHtML

echo "${#s}"
来源：http://wap.fehbvm.com/Article/details/gvkbsfzlh.sHtML

[R22] 截取子串
来源：http://baike.fehbvm.com/Article/details/gukrmdyiz.sHtML

echo "${s:0:5}"
来源：http://read.share.hesvh.cn/Article/details/gynduefkr.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gxxonpxol.sHtML


<!-- 参考信息 -->