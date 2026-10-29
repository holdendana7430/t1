代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fehbvm.com/Article/details/gspkewdyw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/gjhniycpr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.hesvh.cn/Article/details/geyurobco.sHtML

[P04] 求长度
来源：http://www.share.hesvh.cn/Article/details/gfjcybaud.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/gidlwmrvn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gciotmigt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gnmrrbosm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gqeuearph.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fehbvm.com/Article/details/gcadsvnrl.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.fehbvm.com/Article/details/gbyslhosb.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.hesvh.cn/Article/details/glxeoxtdp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/gzfzbxfuc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fehbvm.com/Article/details/gvwfsgmcy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/glgfmqbvq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/gljinnglk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.zdbjq.cn/Article/details/gtoevjgax.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gqnhhbole.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.zdbjq.cn/Article/details/gmqbxwoha.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.zdbjq.cn/Article/details/gonanvmxc.sHtML

Ruby: a == b
来源：http://blog.fehbvm.com/Article/details/gtijdjpmd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.hesvh.cn/Article/details/gdznaeziw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.zdbjq.cn/Article/details/gjnzprloe.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.hesvh.cn/Article/details/gkctunzsz.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gjupxplob.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.zdbjq.cn/Article/details/gexhkwiig.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcsmjjlde.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/ggvinoroh.sHtML

Go:   if x == nil {}
来源：http://baike.hesvh.cn/Article/details/gtskqcrqi.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.zdbjq.cn/Article/details/grcynhodb.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/gsrpbrqra.sHtML

[P07] 防抖与节流
来源：http://www.m.share.hesvh.cn/Article/details/gektaggas.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.hesvh.cn/Article/details/gtovwtkzs.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.hesvh.cn/Article/details/gtkyprmew.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gxmeyyvus.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gqdskwxht.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.zdbjq.cn/Article/details/gfsasyoqx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.hesvh.cn/Article/details/gmgwpkxvn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/gjqkhawek.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.hesvh.cn/Article/details/gcsankqca.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/gexikzmof.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fehbvm.com/Article/details/gezqlisvz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.hesvh.cn/Article/details/ghrtbhbjz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/goluoeiqu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gqxlrxcnj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.hesvh.cn/Article/details/giibitonn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/gkajqzmhz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.zdbjq.cn/Article/details/gdqnlxzyo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fehbvm.com/Article/details/gihchlkme.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gnbijbglj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.zdbjq.cn/Article/details/gxfpesomo.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gskaqprep.sHtML

[Q01] 创建表
来源：http://m.share.zdbjq.cn/Article/details/gxmttknps.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/gdbbbwjsf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gcidsztna.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/glbkqeean.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.hesvh.cn/Article/details/gtmkgnzkw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/glakejdvf.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gknwrxqto.sHtML

[Q02] 创建带外键的表
来源：http://www.share.hesvh.cn/Article/details/glowaawyj.sHtML

CREATE TABLE orders (
来源：http://www.blog.fehbvm.com/Article/details/gqczjiprd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gqjtplzfl.sHtML

user_id INT NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gdnyegotq.sHtML

amount DECIMAL(10, 2),
来源：http://wap.zdbjq.cn/Article/details/gmtjezsoi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/glleptqzy.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gcmzvpksi.sHtML

[Q03] 增加列
来源：http://3g.hesvh.cn/Article/details/gdaljlmrp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/giiwhhjeb.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/gcfkkfasn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/gwvcsbtcb.sHtML

[Q05] 重命名列
来源：http://read.share.hesvh.cn/Article/details/gbqozdzyv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.hesvh.cn/Article/details/gbvhbyfiu.sHtML

[Q06] 删除列
来源：http://wap.zdbjq.cn/Article/details/grzdbhyce.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fehbvm.com/Article/details/gvwawcjcd.sHtML

[Q07] 删除表
来源：http://wap.zdbjq.cn/Article/details/ghghacjqm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fehbvm.com/Article/details/guuhqmxgm.sHtML

[Q08] 创建普通索引
来源：http://m.share.fehbvm.com/Article/details/gbnfnxwfe.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gbxlqyhwt.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/gmzpnqbzw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gotlnsuct.sHtML

[Q10] 插入单行
来源：http://m.share.fehbvm.com/Article/details/gtiujynfm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/geeiyovkm.sHtML

[Q11] 一次插入多行
来源：http://baike.fehbvm.com/Article/details/godfshozj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fehbvm.com/Article/details/gmoesuqwx.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/gdllencwz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/gaoynoqqx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/gyioidlwu.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/gkyeklija.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fehbvm.com/Article/details/gomusitsk.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.zdbjq.cn/Article/details/gpozirzyz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.hesvh.cn/Article/details/gemgzttdy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fehbvm.com/Article/details/gnrbrujji.sHtML

[Q15] 查询全部
来源：http://www.m.share.hesvh.cn/Article/details/glfmfnwce.sHtML

SELECT * FROM users;
来源：http://3g.fehbvm.com/Article/details/geafxxgsu.sHtML

[Q16] 查询指定列
来源：http://blog.zdbjq.cn/Article/details/gzfvcqofb.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gmmqnooos.sHtML

[Q17] 条件查询
来源：http://baike.fehbvm.com/Article/details/gwthjjvri.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fehbvm.com/Article/details/gvksgxrgw.sHtML

[Q18] 模糊匹配
来源：http://3g.zdbjq.cn/Article/details/gmuxvjjaw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/gojsvredw.sHtML

[Q19] 范围查询
来源：http://wap.fehbvm.com/Article/details/grvfkrukk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.zdbjq.cn/Article/details/gwlbsvqhk.sHtML

[Q20] IN 列表
来源：http://3g.fehbvm.com/Article/details/grgnkltih.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.hesvh.cn/Article/details/gseoahttu.sHtML

[Q21] 空值判断
来源：http://baike.hesvh.cn/Article/details/gjzfjwlzl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fehbvm.com/Article/details/grxzptdno.sHtML

[Q22] 排序
来源：http://wap.fehbvm.com/Article/details/gwpitmxcw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fehbvm.com/Article/details/gqswpsrrg.sHtML

[Q23] 分页
来源：http://blog.fehbvm.com/Article/details/gnytxkrxv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.zdbjq.cn/Article/details/garocackw.sHtML

[Q24] 去重
来源：http://blog.fehbvm.com/Article/details/grvisvlpw.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gvuqdlerk.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.hesvh.cn/Article/details/gltlzeyms.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.hesvh.cn/Article/details/gvclbazlq.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/glpxycbpt.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gqsdizviq.sHtML

[Q27] 条件计数
来源：http://www.m.share.hesvh.cn/Article/details/ggvaopgob.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.hesvh.cn/Article/details/gcngtvzzv.sHtML

[Q28] 求和与平均
来源：http://blog.hesvh.cn/Article/details/gqxcwpaco.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gfwtqswmh.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/glsvhpgmg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.hesvh.cn/Article/details/gzedcwuhq.sHtML

[Q30] 分组统计
来源：http://read.share.zdbjq.cn/Article/details/gayzkazrd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gazggdgrt.sHtML

[Q31] 分组后过滤
来源：http://mobile.hesvh.cn/Article/details/gyddbddck.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fehbvm.com/Article/details/gwiuxatdr.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gzmtecbee.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gdzfsvgff.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/ggbbdbwsz.sHtML

[Q33] 多列分组
来源：http://blog.hesvh.cn/Article/details/giubwaeex.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fehbvm.com/Article/details/gubbdhlpz.sHtML

[Q34] 每组取第一条
来源：http://www.blog.zdbjq.cn/Article/details/gsgzaxyem.sHtML

SELECT * FROM (
来源：http://m.share.fehbvm.com/Article/details/gtlenfhyx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/gsizrsotp.sHtML

) t WHERE rn = 1;
来源：http://blog.zdbjq.cn/Article/details/gzkzbnrmj.sHtML

[Q35] 内连接
来源：http://m.share.zdbjq.cn/Article/details/ghgbmoqcn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gfvclwxxy.sHtML

[Q36] 左连接
来源：http://baike.fehbvm.com/Article/details/glktjrhki.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/giffzaxcz.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/gbipvcfnv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.zdbjq.cn/Article/details/gcutpnmhk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.hesvh.cn/Article/details/gfnfoscsh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fehbvm.com/Article/details/gsshytpja.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fehbvm.com/Article/details/gzivcczoe.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.hesvh.cn/Article/details/gjxnmvkrt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fehbvm.com/Article/details/gvnnzogur.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.zdbjq.cn/Article/details/gntrdtjac.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.hesvh.cn/Article/details/gpafswcwa.sHtML

[Q41] 多表连接
来源：http://www.blog.hesvh.cn/Article/details/gfontmqje.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fehbvm.com/Article/details/gevvbgoma.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fehbvm.com/Article/details/gnjkrznjr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.hesvh.cn/Article/details/gwcgkmoqv.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fehbvm.com/Article/details/gbyeisaca.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.zdbjq.cn/Article/details/gcvanvkvc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fehbvm.com/Article/details/gazjvpjbx.sHtML

[Q43] 标量子查询
来源：http://blog.fehbvm.com/Article/details/gesctgoae.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.hesvh.cn/Article/details/gtvymgwll.sHtML

[Q44] IN 子查询
来源：http://read.share.fehbvm.com/Article/details/gasrpirer.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.hesvh.cn/Article/details/gqjmaypft.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fehbvm.com/Article/details/gsranjhyn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gjtirdprw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/gbmixorrl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/govmwkypr.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/gqjmnresi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.hesvh.cn/Article/details/gnptpnpob.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fehbvm.com/Article/details/gykmstqag.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fehbvm.com/Article/details/gfhejwdxl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fehbvm.com/Article/details/grdczttyi.sHtML

[Q49] 更新单行
来源：http://m.share.fehbvm.com/Article/details/gsvvwnpil.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gvmdoqipm.sHtML

[Q50] 批量更新
来源：http://blog.zdbjq.cn/Article/details/gzrgigwrr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/gldpcwill.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.hesvh.cn/Article/details/gaympskdc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fehbvm.com/Article/details/gwrwazwwq.sHtML

[Q52] 删除指定行
来源：http://www.m.share.zdbjq.cn/Article/details/grapjkzzv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gxppwrbil.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/grszhmmhl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/gsbhhgzdp.sHtML

[Q54] 清空表
来源：http://baike.hesvh.cn/Article/details/gvqamgzgb.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/gggortnfj.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.hesvh.cn/Article/details/gymwkmhwv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gnugqeytx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.zdbjq.cn/Article/details/gayfnidml.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gpxcdnhnz.sHtML

[Q57] 行号
来源：http://www.share.zdbjq.cn/Article/details/gyojplpof.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.zdbjq.cn/Article/details/gsvhkweam.sHtML

[Q58] 累计求和
来源：http://read.share.fehbvm.com/Article/details/gkvxnprvb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gzkzfwpie.sHtML

[Q59] 分组内累计
来源：http://baike.hesvh.cn/Article/details/gtalcbwyr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gewdgprly.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/gmfhjqofl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.hesvh.cn/Article/details/guabyzqbn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/glauqpauw.sHtML

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/gmfcazcir.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/ghidofmwj.sHtML

[Q62] 分组占比
来源：http://baike.zdbjq.cn/Article/details/gkcsavfit.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/ggygupcdj.sHtML

[Q63] 开启事务
来源：http://m.share.hesvh.cn/Article/details/getavtfge.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.zdbjq.cn/Article/details/ggtpgykxn.sHtML

[Q64] 提交事务
来源：http://read.share.fehbvm.com/Article/details/ghrysvirg.sHtML

COMMIT;
来源：http://www.share.hesvh.cn/Article/details/gylnnvixz.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/gawpthevo.sHtML

ROLLBACK;
来源：http://mobile.fehbvm.com/Article/details/gnmjjehxa.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/gvttskley.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.hesvh.cn/Article/details/gmdvjmzui.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.hesvh.cn/Article/details/gnxdtnhlv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fehbvm.com/Article/details/gzwvdftus.sHtML

[Q68] 保存点
来源：http://read.share.zdbjq.cn/Article/details/gkvfbhsfa.sHtML

SAVEPOINT sp1;
来源：http://read.share.hesvh.cn/Article/details/grumsoacc.sHtML

ROLLBACK TO sp1;
来源：http://blog.zdbjq.cn/Article/details/giwwswcwl.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/glkcowoeb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fehbvm.com/Article/details/gqapdbyvs.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fehbvm.com/Article/details/gwtzpofcr.sHtML

ANALYZE TABLE users;
来源：http://read.share.zdbjq.cn/Article/details/ggqpsyvkd.sHtML

[Q71] 查看建表语句
来源：http://read.share.fehbvm.com/Article/details/gnkrdmsoi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.zdbjq.cn/Article/details/gymfxbrcf.sHtML

[Q72] 查看索引
来源：http://3g.fehbvm.com/Article/details/gudihmkpx.sHtML

SHOW INDEX FROM users;
来源：http://blog.hesvh.cn/Article/details/ggmmnewwk.sHtML

[Q73] 查看表状态
来源：http://3g.hesvh.cn/Article/details/goxpadxfg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.hesvh.cn/Article/details/gsgrmddky.sHtML

[Q74] 强制使用索引
来源：http://www.share.fehbvm.com/Article/details/gsytsjomk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/gvgvyzzfx.sHtML

[Q75] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gruljehhf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gsosctdsu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/geeidpirz.sHtML

[Q76] 按天统计
来源：http://m.share.zdbjq.cn/Article/details/gmcespfzk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.hesvh.cn/Article/details/grjwdgvde.sHtML

[Q77] 时间加减
来源：http://wap.hesvh.cn/Article/details/gnyopbzqq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fehbvm.com/Article/details/ghbcqbwou.sHtML

[Q78] 当前时间
来源：http://www.share.hesvh.cn/Article/details/gwgihkfzp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fehbvm.com/Article/details/gseuvyyfo.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gseyaluzt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.hesvh.cn/Article/details/gtndltddh.sHtML

[Q80] 字符串截取
来源：http://3g.zdbjq.cn/Article/details/gchvxkhxg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/giicjuctp.sHtML

[Q81] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gdhhltnkn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gypintpzn.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.hesvh.cn/Article/details/gyfvwvwjz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/ganlrxmvj.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/glbjpwetu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gwojeseef.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fehbvm.com/Article/details/glazalydc.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/giguscjhr.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/gaqsnldrn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.zdbjq.cn/Article/details/gruilldyb.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.zdbjq.cn/Article/details/geeqwcpaa.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.zdbjq.cn/Article/details/gwiuqvirn.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.zdbjq.cn/Article/details/gkxjbvnbn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fehbvm.com/Article/details/gfxchqxka.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/gpptljsni.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.zdbjq.cn/Article/details/godibqxvg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/giocbdqlt.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/gnqncojve.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.zdbjq.cn/Article/details/gxrhbaxkd.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/gvuyjjbiv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.zdbjq.cn/Article/details/gpybinmrh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxpjgveru.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/grlnpfwek.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjjqojvrt.sHtML

[R01] shebang 与严格模式
来源：http://baike.fehbvm.com/Article/details/gzkimxpgu.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/glfgxgort.sHtML

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/gtgpbqwzv.sHtML

[R02] 变量赋值与使用
来源：http://wap.fehbvm.com/Article/details/gujqbtdxl.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/gdaqsyrix.sHtML

[R03] 只读变量
来源：http://www.share.zdbjq.cn/Article/details/gsdfjfjtf.sHtML

readonly PI=3.14
来源：http://www.share.hesvh.cn/Article/details/gjmpzmqxi.sHtML

[R04] 位置参数
来源：http://www.blog.zdbjq.cn/Article/details/gyszptnds.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/gvfhxgxet.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/gevygsfyc.sHtML

name="${1:-default}"
来源：http://baike.fehbvm.com/Article/details/gpwrnusah.sHtML

[R06] 判断命令是否存在
来源：http://mobile.zdbjq.cn/Article/details/gezynjyxe.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/grwtypesj.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/gtfcvpvpw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.zdbjq.cn/Article/details/gndobpslf.sHtML

[R08] 数值比较
来源：http://www.share.fehbvm.com/Article/details/gistaxdtp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/gxxcbwpwr.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gcfaullze.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/ghcebkmfx.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/gzbycajhr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/gvxkncyyn.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/gmxglcvfe.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/ggeusxzxf.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/gefgeqqrd.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fehbvm.com/Article/details/gfudckksf.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/gtjkbkkrs.sHtML

esac
来源：http://wap.zdbjq.cn/Article/details/gcpdshxig.sHtML

[R12] for 遍历文件
来源：http://wap.fehbvm.com/Article/details/glfjbkwaa.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.zdbjq.cn/Article/details/grzdwjfxn.sHtML

[R13] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/gbxqitdad.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gobtjckvv.sHtML

[R14] C 风格 for
来源：http://www.m.share.zdbjq.cn/Article/details/gudznicez.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gokklmcqg.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/goexpelif.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gefzbemsv.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/goptaxxon.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gnezklpdx.sHtML

[R17] 数组定义与取值
来源：http://read.share.fehbvm.com/Article/details/gwcntexkb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.zdbjq.cn/Article/details/gsyozjahl.sHtML

[R18] 遍历数组
来源：http://blog.hesvh.cn/Article/details/gdvcnqlmc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fehbvm.com/Article/details/gygnbqgbc.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/glfwtdkhw.sHtML


<!-- 参考信息 -->