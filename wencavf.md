代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.fehbvm.com/Article/details/glwytvqxu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/guirvtlog.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gxsnukepn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gfxigiopn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gnpnftxoo.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/gawgezzti.sHtML

Ruby: x.length;  x.size
来源：http://blog.hesvh.cn/Article/details/gftcocjip.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gwjvqukas.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/ghmuwnytq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/gezttybjo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.zdbjq.cn/Article/details/gmwdfqgai.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.hesvh.cn/Article/details/gpabcehud.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gpypzpgly.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fehbvm.com/Article/details/gnnfasnes.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.hesvh.cn/Article/details/gsuskujjz.sHtML

Ruby: a == b
来源：http://www.blog.zdbjq.cn/Article/details/grwiphkpb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/gpptzczbr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/gynxqceoo.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/gxudeilcb.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fehbvm.com/Article/details/gpoxnztco.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.zdbjq.cn/Article/details/gpbkwvejh.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fehbvm.com/Article/details/gjtysgjjk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gzumtseuo.sHtML

Go:   if x == nil {}
来源：http://baike.hesvh.cn/Article/details/gbzthqfux.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fehbvm.com/Article/details/gepquzbii.sHtML

C#:   if (x is null) {}
来源：http://www.blog.hesvh.cn/Article/details/gqhsmqnvt.sHtML

[P07] 防抖与节流
来源：http://blog.fehbvm.com/Article/details/gnpltaasw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.zdbjq.cn/Article/details/guyazhlui.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.hesvh.cn/Article/details/gdkomjssv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/ghsadwjnn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gwrmftzzp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.hesvh.cn/Article/details/gdfrurxjg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fehbvm.com/Article/details/ghcfhqbgo.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/gnjrgujij.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.hesvh.cn/Article/details/gdndxlzgx.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fehbvm.com/Article/details/gaqjbjowe.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.hesvh.cn/Article/details/gyjypzlhc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/gsvhirvqd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/gwojcdyjd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/glilylmbj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.zdbjq.cn/Article/details/gxzsoqfsw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fehbvm.com/Article/details/gvanyjrsy.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.zdbjq.cn/Article/details/gwqrtuyqg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/gsglwdrxl.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grykroghr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/guyloaliq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/geezuiuca.sHtML

[Q01] 创建表
来源：http://3g.fehbvm.com/Article/details/gynsbdvmb.sHtML

CREATE TABLE users (
来源：http://mobile.zdbjq.cn/Article/details/gdtvgabfk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gopxgsckg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gbaqhrtqn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.hesvh.cn/Article/details/gnidhuyli.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.hesvh.cn/Article/details/gpptxokja.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gulsmkzvc.sHtML

[Q02] 创建带外键的表
来源：http://baike.hesvh.cn/Article/details/gsopvozbu.sHtML

CREATE TABLE orders (
来源：http://m.share.zdbjq.cn/Article/details/gdlstxwyy.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gplxgrtbn.sHtML

user_id INT NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gmjoiwybi.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fehbvm.com/Article/details/gksbbyxhq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.hesvh.cn/Article/details/gkzfdkzoa.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gliwphafa.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/gkwrzcjnw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.zdbjq.cn/Article/details/gsojvsnik.sHtML

[Q04] 修改列类型
来源：http://mobile.hesvh.cn/Article/details/gnfpexcsu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fehbvm.com/Article/details/gfztnrctb.sHtML

[Q05] 重命名列
来源：http://www.m.share.zdbjq.cn/Article/details/gblirikhx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fehbvm.com/Article/details/gkzztflxs.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/ghfynokik.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fehbvm.com/Article/details/gvuipxjyr.sHtML

[Q07] 删除表
来源：http://www.share.zdbjq.cn/Article/details/gnbfmgphu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.hesvh.cn/Article/details/gvostpdtw.sHtML

[Q08] 创建普通索引
来源：http://read.share.fehbvm.com/Article/details/gvixpqens.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gehtvybcb.sHtML

[Q09] 创建唯一索引
来源：http://www.share.zdbjq.cn/Article/details/gqhwlopxg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gevfqxqbi.sHtML

[Q10] 插入单行
来源：http://www.blog.zdbjq.cn/Article/details/gmszotfrh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fehbvm.com/Article/details/gfeaenvdj.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/gqgabhoek.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gxgrsnfvx.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/gdkncqpmb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.zdbjq.cn/Article/details/gnizwdcjy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.hesvh.cn/Article/details/gozqllpue.sHtML

[Q13] 忽略重复插入
来源：http://wap.zdbjq.cn/Article/details/gletfheck.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.zdbjq.cn/Article/details/gcqqkboia.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fehbvm.com/Article/details/gssofskaa.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fehbvm.com/Article/details/gpnldwtlg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.hesvh.cn/Article/details/grdtnmgwa.sHtML

[Q15] 查询全部
来源：http://www.m.share.fehbvm.com/Article/details/ghuwyldpe.sHtML

SELECT * FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gzkkeqlla.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/gtctqzgxh.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gqhelelzx.sHtML

[Q17] 条件查询
来源：http://mobile.fehbvm.com/Article/details/gfyejyrrv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.hesvh.cn/Article/details/gkgokhkbi.sHtML

[Q18] 模糊匹配
来源：http://www.share.hesvh.cn/Article/details/gyomlnssi.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.hesvh.cn/Article/details/gsirlbhld.sHtML

[Q19] 范围查询
来源：http://m.share.zdbjq.cn/Article/details/gbsbclslr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fehbvm.com/Article/details/ggsmqcsxs.sHtML

[Q20] IN 列表
来源：http://blog.zdbjq.cn/Article/details/guxxmsogq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.hesvh.cn/Article/details/gcurgapdd.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/gwzvbqtru.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/gwgpickmp.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/gthsfrhsv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gjzciqylk.sHtML

[Q23] 分页
来源：http://m.share.hesvh.cn/Article/details/gdkttuhbl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.hesvh.cn/Article/details/genryjoxx.sHtML

[Q24] 去重
来源：http://mobile.hesvh.cn/Article/details/gjtzznhtl.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fehbvm.com/Article/details/gusfcqjsf.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/gedzfcbeo.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.hesvh.cn/Article/details/gtfiffeik.sHtML

[Q26] 计数
来源：http://mobile.zdbjq.cn/Article/details/gassjseva.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/gkqxrxmle.sHtML

[Q27] 条件计数
来源：http://baike.zdbjq.cn/Article/details/galdlxqcm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.hesvh.cn/Article/details/gdpfubbva.sHtML

[Q28] 求和与平均
来源：http://www.blog.zdbjq.cn/Article/details/gtccavtle.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gippnxjhg.sHtML

[Q29] 最大最小值
来源：http://baike.hesvh.cn/Article/details/gmaavjfeb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gghvfdmwg.sHtML

[Q30] 分组统计
来源：http://mobile.zdbjq.cn/Article/details/guhxienow.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gpvpnzzia.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/gndglxykc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fehbvm.com/Article/details/ghuqflxiv.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gtxzljiil.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gxayfwkqb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.hesvh.cn/Article/details/gudsaiumj.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/gsttwbdcv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.hesvh.cn/Article/details/gqlcbblol.sHtML

[Q34] 每组取第一条
来源：http://mobile.hesvh.cn/Article/details/gvfsocdbi.sHtML

SELECT * FROM (
来源：http://wap.zdbjq.cn/Article/details/gatuydnqj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fehbvm.com/Article/details/gfnxqbxfk.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/gfnsldfrs.sHtML

[Q35] 内连接
来源：http://read.share.hesvh.cn/Article/details/grsepltoc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gilhuoplb.sHtML

[Q36] 左连接
来源：http://wap.fehbvm.com/Article/details/gptbdgzfe.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gsgrmqfhx.sHtML

[Q37] 右连接
来源：http://www.share.hesvh.cn/Article/details/gezkugxyk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fehbvm.com/Article/details/gallhzupv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/gmxbgwzii.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/gipxizauy.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.zdbjq.cn/Article/details/gdshjnlxe.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fehbvm.com/Article/details/gytzecylp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/gjsrztpfm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.zdbjq.cn/Article/details/gpbbbkrzk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fehbvm.com/Article/details/gpsquacqg.sHtML

[Q41] 多表连接
来源：http://www.blog.fehbvm.com/Article/details/gnbcalvly.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/gydtvfbpe.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.zdbjq.cn/Article/details/gbjhyzski.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/gvgttdiev.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fehbvm.com/Article/details/gwgpgiyzj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fehbvm.com/Article/details/gfpolulzp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/gitivhpbq.sHtML

[Q43] 标量子查询
来源：http://baike.hesvh.cn/Article/details/gnopazgln.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.hesvh.cn/Article/details/gimjteiwc.sHtML

[Q44] IN 子查询
来源：http://mobile.hesvh.cn/Article/details/gkpneomjr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.zdbjq.cn/Article/details/ghqrwecpa.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.hesvh.cn/Article/details/gyrjbvuwe.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gaaszeuuy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/gaphkpyyy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gskcvvyyf.sHtML

[Q47] 与平均值比较
来源：http://m.share.zdbjq.cn/Article/details/ghntgddsq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.zdbjq.cn/Article/details/gtysvcwkz.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.zdbjq.cn/Article/details/gnasurthv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/grogqbzcu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.hesvh.cn/Article/details/gpzxrzith.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/gzhomeepb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gecxfpiga.sHtML

[Q50] 批量更新
来源：http://baike.hesvh.cn/Article/details/ghbuvtazh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.hesvh.cn/Article/details/gcycclrlk.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/gtwzwftue.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gvtkukqlp.sHtML

[Q52] 删除指定行
来源：http://www.m.share.hesvh.cn/Article/details/gdnbpzpkv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gtlgnaika.sHtML

[Q53] 按条件删除
来源：http://wap.zdbjq.cn/Article/details/guxjadczv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gdofzuedn.sHtML

[Q54] 清空表
来源：http://wap.fehbvm.com/Article/details/gdplsfrok.sHtML

TRUNCATE TABLE logs;
来源：http://baike.zdbjq.cn/Article/details/gorkztayp.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.zdbjq.cn/Article/details/gwavzlwzd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gyyczpnzz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.hesvh.cn/Article/details/gvhoukmbf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gftjjdhcc.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/gqihbfzoa.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/gshhrxmed.sHtML

[Q58] 累计求和
来源：http://read.share.fehbvm.com/Article/details/gsjolzdjc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.hesvh.cn/Article/details/ggifykmlk.sHtML

[Q59] 分组内累计
来源：http://mobile.fehbvm.com/Article/details/gaqfeoyyc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gslfoieza.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fehbvm.com/Article/details/gvguonmds.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/gnboghwwe.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fehbvm.com/Article/details/ghtntbtvs.sHtML

[Q61] 移动平均
来源：http://wap.fehbvm.com/Article/details/gmbchgols.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gdnuimrpv.sHtML

[Q62] 分组占比
来源：http://mobile.hesvh.cn/Article/details/gexpptzbv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gvcxyodkw.sHtML

[Q63] 开启事务
来源：http://read.share.fehbvm.com/Article/details/gjcdsoctg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fehbvm.com/Article/details/gkwsyblxi.sHtML

[Q64] 提交事务
来源：http://www.share.fehbvm.com/Article/details/ggktcocwd.sHtML

COMMIT;
来源：http://mobile.hesvh.cn/Article/details/grpfhbcau.sHtML

[Q65] 回滚事务
来源：http://mobile.fehbvm.com/Article/details/gswzqwyvr.sHtML

ROLLBACK;
来源：http://mobile.fehbvm.com/Article/details/gfzhmwdyi.sHtML

[Q66] 行锁查询
来源：http://wap.fehbvm.com/Article/details/gwrzazdvd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/gmudiqxlg.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.hesvh.cn/Article/details/gmuexlvmj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fehbvm.com/Article/details/guqqflzhg.sHtML

[Q68] 保存点
来源：http://wap.hesvh.cn/Article/details/giexyxfpb.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gvghwcang.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/ghgmdmbpa.sHtML

[Q69] 查看执行计划
来源：http://mobile.zdbjq.cn/Article/details/gnfcbxdqm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/gjalrdive.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/gctdgzeai.sHtML

ANALYZE TABLE users;
来源：http://read.share.hesvh.cn/Article/details/gxausixhe.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/gtvcehdsk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.hesvh.cn/Article/details/gpaiqrwww.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/gqomguecb.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gdgernmtc.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/gofdgpakk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.hesvh.cn/Article/details/gzbvnqgbv.sHtML

[Q74] 强制使用索引
来源：http://3g.zdbjq.cn/Article/details/gkljyieru.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.hesvh.cn/Article/details/gxzdbvwhy.sHtML

[Q75] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gcqstsbqs.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fehbvm.com/Article/details/gkfcqalrj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/goeenaldj.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/gvgnjgajd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.zdbjq.cn/Article/details/gdfbmerix.sHtML

[Q77] 时间加减
来源：http://baike.zdbjq.cn/Article/details/gzwuoumxd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/gvnyyejep.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/gtqequeom.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.zdbjq.cn/Article/details/gaqnzhhbb.sHtML

[Q79] 字符串拼接
来源：http://wap.hesvh.cn/Article/details/gioucvtps.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.zdbjq.cn/Article/details/gjaajfous.sHtML

[Q80] 字符串截取
来源：http://3g.hesvh.cn/Article/details/gqecoiphs.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/glnqjjouv.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gmwnvhswn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gtodxdlav.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.hesvh.cn/Article/details/gfwvysmfm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gbjsavdkn.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gitghpjzh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gldewrbpq.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/gmogowppk.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/grrqthwev.sHtML

[Q85] 数值取整
来源：http://blog.fehbvm.com/Article/details/gmemmavcn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.zdbjq.cn/Article/details/gwnfwikps.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/gnuhnoiyy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.hesvh.cn/Article/details/gzasrlvct.sHtML

[Q87] JSON 字段做条件
来源：http://blog.zdbjq.cn/Article/details/gjjyzovba.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fehbvm.com/Article/details/guipmfkja.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fehbvm.com/Article/details/glvogmpmh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/gaukleznm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.hesvh.cn/Article/details/giiszelik.sHtML

[Q89] 判断表是否存在
来源：http://blog.zdbjq.cn/Article/details/gplugwuaa.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gypjjnyoy.sHtML

[Q90] 生成序号列
来源：http://www.m.share.zdbjq.cn/Article/details/gpqumtdfj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.zdbjq.cn/Article/details/grmevxjit.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grfhmutnh.sHtML

R. Bash 专题
来源：http://3g.zdbjq.cn/Article/details/genjktgwr.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/guzgfsdmh.sHtML

[R01] shebang 与严格模式
来源：http://wap.fehbvm.com/Article/details/gsnffcjlm.sHtML

#!/usr/bin/env bash
来源：http://mobile.fehbvm.com/Article/details/goqtcencf.sHtML

set -euo pipefail
来源：http://read.share.hesvh.cn/Article/details/gznuwsikx.sHtML

[R02] 变量赋值与使用
来源：http://wap.fehbvm.com/Article/details/gvlgurjsr.sHtML

name="Tom"; echo "$name"
来源：http://www.share.zdbjq.cn/Article/details/gkojszyqf.sHtML

[R03] 只读变量
来源：http://www.share.hesvh.cn/Article/details/gnkdmsgme.sHtML

readonly PI=3.14
来源：http://wap.fehbvm.com/Article/details/gtngezlnx.sHtML

[R04] 位置参数
来源：http://www.blog.hesvh.cn/Article/details/gtvwqenvk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fehbvm.com/Article/details/gjzcaolwe.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/ggbsujews.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/gizpktton.sHtML

[R06] 判断命令是否存在
来源：http://3g.fehbvm.com/Article/details/gyuwnadrd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gdfdwtnzm.sHtML

[R07] if 判断文件
来源：http://mobile.fehbvm.com/Article/details/gedwhusqu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.zdbjq.cn/Article/details/ghzndwyvl.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/gagtbmbcy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.zdbjq.cn/Article/details/gubvewmft.sHtML

[R09] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/grqaqramq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/gnmpkkkjt.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/gpcjkctzy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.zdbjq.cn/Article/details/gjrqfqgrg.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/gnsuuardk.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/ggazgapbm.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/gdakrsbqb.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/griabfgzy.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fehbvm.com/Article/details/gtysxmnfx.sHtML

esac
来源：http://www.share.fehbvm.com/Article/details/gsiennfpa.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/gxorltczx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fehbvm.com/Article/details/ghowmjtrc.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/glkvwgyim.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gkxexpeki.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/gwekiqjep.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gnckcllhh.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/ghnmglagk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fehbvm.com/Article/details/gdvylpksl.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/gieusklsh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/giqxhbkdm.sHtML

[R17] 数组定义与取值
来源：http://3g.zdbjq.cn/Article/details/gqzoqnkvo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.hesvh.cn/Article/details/glvvifxlm.sHtML

[R18] 遍历数组
来源：http://mobile.fehbvm.com/Article/details/gxowbrwnc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gzjwhwryr.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gjgbumzbx.sHtML

echo "${#arr[@]}"
来源：http://read.share.fehbvm.com/Article/details/gfikikgdf.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/gvmytwrli.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/gkupyvquf.sHtML

[R21] 字符串长度
来源：http://3g.fehbvm.com/Article/details/glmayugmw.sHtML


<!-- 参考信息 -->