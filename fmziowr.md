代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/gezxhuxxe.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/gmldimcrz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.hesvh.cn/Article/details/gfxdukudv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.zdbjq.cn/Article/details/gbokkptym.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gctjioloh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.zdbjq.cn/Article/details/gjzahbmjr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gmjdynznv.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/gjrpkpqaz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.hesvh.cn/Article/details/gebemhepb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.hesvh.cn/Article/details/gtarmyqvv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.zdbjq.cn/Article/details/gixpzrghv.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fehbvm.com/Article/details/gxgivgpfq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/gpasnmpbq.sHtML

TS:   if (x == null) {}
来源：http://m.share.zdbjq.cn/Article/details/gcxerkqdk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gxxdarjbb.sHtML

Go:   if x == nil {}
来源：http://blog.fehbvm.com/Article/details/gkcbjpcsg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fehbvm.com/Article/details/gqebvuvtv.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/gfimafann.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/gxdbxrxng.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.hesvh.cn/Article/details/geussnrrc.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.hesvh.cn/Article/details/glctcchxl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/getqyqoxj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gtjawomvl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.hesvh.cn/Article/details/glzszcqmf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.zdbjq.cn/Article/details/gcetllyjt.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.zdbjq.cn/Article/details/gkfodvptb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.zdbjq.cn/Article/details/gzqffxihb.sHtML

[P08] 处理浮点精度问题
来源：http://baike.zdbjq.cn/Article/details/gnpaevxre.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/gpggcfmal.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.zdbjq.cn/Article/details/ggkyakpcm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.hesvh.cn/Article/details/gechxveme.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/grukurnjb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fehbvm.com/Article/details/grxjwlbsp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gmlpwtdsv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.hesvh.cn/Article/details/glejixtpm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fehbvm.com/Article/details/gclhccsrt.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gopfidaix.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.hesvh.cn/Article/details/gsswbhiwo.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gugkgkosz.sHtML

[Q01] 创建表
来源：http://read.share.hesvh.cn/Article/details/goiztryso.sHtML

CREATE TABLE users (
来源：http://baike.zdbjq.cn/Article/details/ggemezfmw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gjamhcerq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gtzptzmex.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fehbvm.com/Article/details/gkhhwjrsd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.zdbjq.cn/Article/details/gcxnecoyi.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/guvyjkaqa.sHtML

[Q02] 创建带外键的表
来源：http://blog.hesvh.cn/Article/details/gxbfcickb.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/gmcgdkhwi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gvwjhocck.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gtgtgnfdb.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fehbvm.com/Article/details/gmsxicyva.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.zdbjq.cn/Article/details/gjcioqrfb.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gdcvveota.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/gevjwzhra.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fehbvm.com/Article/details/gtzgtmggx.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/gosqjndoy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.zdbjq.cn/Article/details/gukqphphg.sHtML

[Q05] 重命名列
来源：http://wap.zdbjq.cn/Article/details/guxnaqvfw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/gedraulrk.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/grozenwta.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.hesvh.cn/Article/details/ggbonjxmn.sHtML

[Q07] 删除表
来源：http://wap.zdbjq.cn/Article/details/gnxzlvivs.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.zdbjq.cn/Article/details/gvogtsbdn.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/ggdrbygxo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/giogzbvxm.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/grvzcafqd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/ggnwszoco.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/glsdwxedm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/gtsarfmts.sHtML

[Q11] 一次插入多行
来源：http://read.share.zdbjq.cn/Article/details/ghuojsivb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gyfqefrza.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.zdbjq.cn/Article/details/gjiuaakgo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/gmxowqizu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fehbvm.com/Article/details/gfhkoddtg.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/gwtwtymjr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gfwjiwxqh.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.zdbjq.cn/Article/details/grakhragv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.hesvh.cn/Article/details/gfodfomfx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.hesvh.cn/Article/details/gecbohjmv.sHtML

[Q15] 查询全部
来源：http://read.share.zdbjq.cn/Article/details/glkyzgfnc.sHtML

SELECT * FROM users;
来源：http://baike.zdbjq.cn/Article/details/gchznbipa.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/gibfqouww.sHtML

SELECT id, name FROM users;
来源：http://read.share.zdbjq.cn/Article/details/ghlbgxoia.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/gowgptbcb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.hesvh.cn/Article/details/gjasgymkr.sHtML

[Q18] 模糊匹配
来源：http://m.share.fehbvm.com/Article/details/gwqiwuuzu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.zdbjq.cn/Article/details/golxlzxxg.sHtML

[Q19] 范围查询
来源：http://read.share.fehbvm.com/Article/details/ggxnfdhsn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fehbvm.com/Article/details/gxdbfqosa.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/gfrhtwovs.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.hesvh.cn/Article/details/gxmuehmtf.sHtML

[Q21] 空值判断
来源：http://baike.hesvh.cn/Article/details/glbpwyyph.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gatlnqefu.sHtML

[Q22] 排序
来源：http://www.m.share.zdbjq.cn/Article/details/gfgehmpkc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/gxzsxsmyb.sHtML

[Q23] 分页
来源：http://blog.fehbvm.com/Article/details/ghclklfdz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/gkvepqide.sHtML

[Q24] 去重
来源：http://3g.hesvh.cn/Article/details/gvrwwclno.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.hesvh.cn/Article/details/gpnpahflz.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fehbvm.com/Article/details/ggyxysuhn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/gufthbrdn.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/goslkkfnk.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fehbvm.com/Article/details/gkzkhomnw.sHtML

[Q27] 条件计数
来源：http://www.m.share.fehbvm.com/Article/details/geflzxlhk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.zdbjq.cn/Article/details/gcmywfmms.sHtML

[Q28] 求和与平均
来源：http://www.m.share.hesvh.cn/Article/details/gonvhkrep.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gryvziezk.sHtML

[Q29] 最大最小值
来源：http://www.share.fehbvm.com/Article/details/gkluhprrp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gpfxiyfmf.sHtML

[Q30] 分组统计
来源：http://www.share.fehbvm.com/Article/details/gancivexb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gbzhhiojf.sHtML

[Q31] 分组后过滤
来源：http://blog.zdbjq.cn/Article/details/gaymqyaya.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.zdbjq.cn/Article/details/glnkorebb.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fehbvm.com/Article/details/guqfgubgb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/ghlidtfyi.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fehbvm.com/Article/details/gfgozbyxf.sHtML

[Q33] 多列分组
来源：http://baike.hesvh.cn/Article/details/gkimgednr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.zdbjq.cn/Article/details/gvykwnqjn.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/guwqammsh.sHtML

SELECT * FROM (
来源：http://wap.zdbjq.cn/Article/details/gdlpsoyuj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.zdbjq.cn/Article/details/glaymcwnc.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/glaltmnho.sHtML

[Q35] 内连接
来源：http://www.m.share.hesvh.cn/Article/details/ggolatnwi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/ghmfpcgfs.sHtML

[Q36] 左连接
来源：http://baike.fehbvm.com/Article/details/gcetgufeo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gytucpcoa.sHtML

[Q37] 右连接
来源：http://blog.fehbvm.com/Article/details/grmazvtil.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/gidxwbwhb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/gbjlzxinn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.hesvh.cn/Article/details/gwtpalexy.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.hesvh.cn/Article/details/gccslhcol.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.zdbjq.cn/Article/details/gcefdevqk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/ghylllxnj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.zdbjq.cn/Article/details/gfgozzxed.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fehbvm.com/Article/details/gunwruoqu.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/gejtrpeze.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/gpjonnqhk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/gdfyurjnk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.zdbjq.cn/Article/details/ghqpfvrvw.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.hesvh.cn/Article/details/ghfrmrrls.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.zdbjq.cn/Article/details/gncavoutv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/gnvgltkzi.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/gldtxapqz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fehbvm.com/Article/details/gfphmfyyx.sHtML

[Q44] IN 子查询
来源：http://www.share.hesvh.cn/Article/details/gtkkaeffv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/gcwtqjufo.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/gvbuernvr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gtljgmosw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/gulyotjok.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gxggcnsax.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fehbvm.com/Article/details/gwjzygiik.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/gjemgyopg.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.zdbjq.cn/Article/details/gdbjuchcz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.hesvh.cn/Article/details/gigbmkdkm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fehbvm.com/Article/details/goqigsmtq.sHtML

[Q49] 更新单行
来源：http://blog.zdbjq.cn/Article/details/gdvdsthre.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gqulrlthl.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gqsirfnas.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.zdbjq.cn/Article/details/gtmemkdvk.sHtML

[Q51] 用子查询更新
来源：http://www.share.zdbjq.cn/Article/details/gurgfhsfr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.zdbjq.cn/Article/details/gacqxzeli.sHtML

[Q52] 删除指定行
来源：http://www.share.zdbjq.cn/Article/details/guoubzkhm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gydoqwqin.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/geiyliytx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gzfgyqqea.sHtML

[Q54] 清空表
来源：http://mobile.hesvh.cn/Article/details/gaprualsq.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/gcyigdkzj.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.hesvh.cn/Article/details/gnhxqtvmg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/gfedfcfud.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.zdbjq.cn/Article/details/gtuhlvksp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gegvnkuho.sHtML

[Q57] 行号
来源：http://www.m.share.hesvh.cn/Article/details/giahiyemf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/gholycvky.sHtML

[Q58] 累计求和
来源：http://wap.hesvh.cn/Article/details/grthqnqlx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/geynhhmxq.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/gilahcdin.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gqxearryf.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.zdbjq.cn/Article/details/goxremeur.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fehbvm.com/Article/details/gqaugwjig.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/guwzjcyfb.sHtML

[Q61] 移动平均
来源：http://read.share.zdbjq.cn/Article/details/giutooyer.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gwruufelj.sHtML

[Q62] 分组占比
来源：http://www.share.fehbvm.com/Article/details/gwiawzfga.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gsvsvozgu.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/gymcazxlb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.hesvh.cn/Article/details/gihidzmwm.sHtML

[Q64] 提交事务
来源：http://wap.zdbjq.cn/Article/details/gqmqhmkpf.sHtML

COMMIT;
来源：http://m.share.fehbvm.com/Article/details/gewwpsigr.sHtML

[Q65] 回滚事务
来源：http://www.blog.fehbvm.com/Article/details/gvgjlkvla.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/guwzzilka.sHtML

[Q66] 行锁查询
来源：http://wap.hesvh.cn/Article/details/gpabgwunl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.zdbjq.cn/Article/details/gcpnbtlpr.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.hesvh.cn/Article/details/gytlzxbwq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/gssxzshnn.sHtML

[Q68] 保存点
来源：http://blog.fehbvm.com/Article/details/gmkwzsxiu.sHtML

SAVEPOINT sp1;
来源：http://baike.hesvh.cn/Article/details/gfhedwwen.sHtML

ROLLBACK TO sp1;
来源：http://blog.zdbjq.cn/Article/details/ghefhnjex.sHtML

[Q69] 查看执行计划
来源：http://m.share.zdbjq.cn/Article/details/ggljizqtc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.zdbjq.cn/Article/details/gqqozalem.sHtML

[Q70] 更新统计信息
来源：http://read.share.fehbvm.com/Article/details/gvoicaqcg.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.hesvh.cn/Article/details/guqffpfqr.sHtML

[Q71] 查看建表语句
来源：http://www.share.fehbvm.com/Article/details/gejkpqsel.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.hesvh.cn/Article/details/gvooylgvs.sHtML

[Q72] 查看索引
来源：http://www.blog.fehbvm.com/Article/details/gfkwfvovv.sHtML

SHOW INDEX FROM users;
来源：http://baike.zdbjq.cn/Article/details/gyqpvmkxa.sHtML

[Q73] 查看表状态
来源：http://www.blog.fehbvm.com/Article/details/gfrjjtwax.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gpcmurrvh.sHtML

[Q74] 强制使用索引
来源：http://m.share.hesvh.cn/Article/details/gcqjlsohr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/ghwimmzxc.sHtML

[Q75] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gdtldhuby.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/ggghrxjck.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.hesvh.cn/Article/details/ggraggpgr.sHtML

[Q76] 按天统计
来源：http://www.m.share.fehbvm.com/Article/details/gcoljsvvo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.zdbjq.cn/Article/details/gusgcbdso.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/glejhnkok.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/gcypykakj.sHtML

[Q78] 当前时间
来源：http://blog.hesvh.cn/Article/details/gexnnrmkk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.zdbjq.cn/Article/details/gpzkkmfks.sHtML

[Q79] 字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gxzwwjzuy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fehbvm.com/Article/details/ghvuzmdtn.sHtML

[Q80] 字符串截取
来源：http://read.share.fehbvm.com/Article/details/ggszygccw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gkmdnjidh.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/ggikslgoe.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.hesvh.cn/Article/details/gfviqeddf.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fehbvm.com/Article/details/gjqiwzpxa.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gfrvlyxis.sHtML

[Q83] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gizdsncjb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gdfpwfqfp.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/guofnvglx.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gtomhwpbz.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/gxproivyu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/gegiayzjz.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.hesvh.cn/Article/details/gpdvadlbh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fehbvm.com/Article/details/gbjulfbvd.sHtML

[Q87] JSON 字段做条件
来源：http://3g.hesvh.cn/Article/details/gjcjkkevo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.hesvh.cn/Article/details/gnpdhhrkn.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.hesvh.cn/Article/details/gqmxyydaw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.hesvh.cn/Article/details/gtvhndisw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.zdbjq.cn/Article/details/gduivsgyg.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/gstqhiwez.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/gzjyxbmpj.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/guoujrfgp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.hesvh.cn/Article/details/gwixaetct.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gaksmusjp.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/geunotndt.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/goxidjbib.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fehbvm.com/Article/details/gbbiqaeia.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fehbvm.com/Article/details/gcpznltuu.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/gnhhvuplg.sHtML

[R02] 变量赋值与使用
来源：http://3g.hesvh.cn/Article/details/ggqnerguz.sHtML

name="Tom"; echo "$name"
来源：http://baike.fehbvm.com/Article/details/gooskkhoa.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/gmbupnezx.sHtML

readonly PI=3.14
来源：http://m.share.fehbvm.com/Article/details/glgjzifrs.sHtML

[R04] 位置参数
来源：http://www.m.share.hesvh.cn/Article/details/gpcpwbljn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.hesvh.cn/Article/details/gvrxhvlkj.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/gpkobkztz.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gtoxzrrnt.sHtML

[R06] 判断命令是否存在
来源：http://3g.hesvh.cn/Article/details/gpzhjwllv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gvyjfjohi.sHtML

[R07] if 判断文件
来源：http://m.share.hesvh.cn/Article/details/gzkzxydfu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gsehxtdyq.sHtML

[R08] 数值比较
来源：http://m.share.hesvh.cn/Article/details/gtdyylwyv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/gpsmuihft.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/ghtyewbfh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.zdbjq.cn/Article/details/gwdajvsui.sHtML

[R10] 正则匹配
来源：http://mobile.zdbjq.cn/Article/details/giduaopty.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.hesvh.cn/Article/details/gzoalzzth.sHtML

[R11] case 多分支
来源：http://blog.hesvh.cn/Article/details/ggbfhbkyh.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/gykysowzr.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gkptzygkt.sHtML

stop)  echo "停止" ;;
来源：http://read.share.hesvh.cn/Article/details/gstihvjpe.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gvbhyckjh.sHtML

esac
来源：http://mobile.fehbvm.com/Article/details/gdvoyfnwx.sHtML

[R12] for 遍历文件
来源：http://wap.hesvh.cn/Article/details/gjlnwdpaa.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/gbuzmbpmo.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gkrqwhltd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gqldyzulq.sHtML

[R14] C 风格 for
来源：http://www.share.zdbjq.cn/Article/details/gaofcjkby.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gnsoninxt.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/gqbeebjas.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.zdbjq.cn/Article/details/gobvrbnjk.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gciixkebb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gdbulqtpz.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/gubengrmy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/gtmknedhu.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/gmlgjussw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.zdbjq.cn/Article/details/gklrfcydu.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gqkmgllmj.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/grazpepsr.sHtML

[R20] 关联数组（字典）
来源：http://m.share.hesvh.cn/Article/details/gdxbyludk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/gpvchdvbb.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/gshheeevo.sHtML

echo "${#s}"
来源：http://wap.fehbvm.com/Article/details/gvjraccat.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gnmuaimrm.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/gvxrevtuo.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gykxkycng.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fehbvm.com/Article/details/gwidjjltg.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gypbjlviq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fehbvm.com/Article/details/giellvcgn.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.hesvh.cn/Article/details/gshgsnsdx.sHtML


<!-- 参考信息 -->