代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fanxiaobao.xyz/Article/details/gohvbnrzm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fanxiaobao.xyz/Article/details/gvmjlbjmj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fanxiaobao.xyz/Article/details/glvizupxa.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fanxiaobao.xyz/Article/details/gdwgkwwad.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fanxiaobao.xyz/Article/details/gidzytbwe.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fanxiaobao.xyz/Article/details/gokrolflr.sHtML

Ruby: x.length;  x.size
来源：http://3g.fanxiaobao.xyz/Article/details/gufbynyis.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fanxiaobao.xyz/Article/details/gwmgpsgkh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdzxcttn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gstgaujun.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fanxiaobao.xyz/Article/details/gszlgwcvb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcvnfosf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gqgmegafs.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.fanxiaobao.xyz/Article/details/gjtqtcubo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnlvlrha.sHtML

Ruby: a == b
来源：http://baike.fanxiaobao.xyz/Article/details/gqloubvvs.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzaihyue.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fanxiaobao.xyz/Article/details/griedhnob.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fanxiaobao.xyz/Article/details/gibvdvnmr.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gzdgxzlrl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fanxiaobao.xyz/Article/details/guxxelsbo.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnteltxhk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gfgeuczge.sHtML

Go:   if x == nil {}
来源：http://baike.fanxiaobao.xyz/Article/details/gozyljrfq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmlasgve.sHtML

C#:   if (x is null) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gxwygifsc.sHtML

[P07] 防抖与节流
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtmwoaih.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fanxiaobao.xyz/Article/details/glidusujd.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.fanxiaobao.xyz/Article/details/ggtacnlwb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/galuvdvig.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkldumtv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gatmwmsos.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.fanxiaobao.xyz/Article/details/genejfvhj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdamkdow.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fanxiaobao.xyz/Article/details/gdvxrkwil.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fanxiaobao.xyz/Article/details/givdastuk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fanxiaobao.xyz/Article/details/gtdmqeaeg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdrowupq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlfakipn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumscjzot.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fanxiaobao.xyz/Article/details/ginpublvn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnwyyafi.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fanxiaobao.xyz/Article/details/gooxmkjyf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fanxiaobao.xyz/Article/details/gagutuiwc.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxzloker.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fanxiaobao.xyz/Article/details/gwnghnnwn.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gqhhxkwhn.sHtML

[Q01] 创建表
来源：http://read.share.fanxiaobao.xyz/Article/details/gqaawyhab.sHtML

CREATE TABLE users (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdktvnyle.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fanxiaobao.xyz/Article/details/gaekdkhcd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fanxiaobao.xyz/Article/details/gqxnsytlv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtphovic.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fanxiaobao.xyz/Article/details/ghamvcvsf.sHtML

);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvneinall.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fanxiaobao.xyz/Article/details/gqyriwahy.sHtML

CREATE TABLE orders (
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhujmnbm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqjfwlwy.sHtML

user_id INT NOT NULL,
来源：http://m.share.fanxiaobao.xyz/Article/details/gsiqgxamz.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fanxiaobao.xyz/Article/details/gzyggdbpr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfphpdyj.sHtML

);
来源：http://3g.fanxiaobao.xyz/Article/details/gyoxqdjov.sHtML

[Q03] 增加列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqagtfapq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gtszhepea.sHtML

[Q04] 修改列类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gulqvffpa.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fanxiaobao.xyz/Article/details/gghiyzvuu.sHtML

[Q05] 重命名列
来源：http://blog.fanxiaobao.xyz/Article/details/grkafhqpn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqaznhluf.sHtML

[Q06] 删除列
来源：http://baike.fanxiaobao.xyz/Article/details/gyhjfzcky.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fanxiaobao.xyz/Article/details/gscovhttd.sHtML

[Q07] 删除表
来源：http://baike.fanxiaobao.xyz/Article/details/gocwdzsae.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fanxiaobao.xyz/Article/details/glcjszcgf.sHtML

[Q08] 创建普通索引
来源：http://wap.fanxiaobao.xyz/Article/details/giopawufq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fanxiaobao.xyz/Article/details/gxnmjttqg.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzoivemys.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmmtwoqm.sHtML

[Q10] 插入单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshmnuoar.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdavljfkz.sHtML

[Q11] 一次插入多行
来源：http://3g.fanxiaobao.xyz/Article/details/gbidaiwgg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gerhbowvi.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fanxiaobao.xyz/Article/details/gbgblduoc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fanxiaobao.xyz/Article/details/gbchiipqg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gooufsjhx.sHtML

[Q13] 忽略重复插入
来源：http://blog.fanxiaobao.xyz/Article/details/gqcwhxylo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgpebbyy.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fanxiaobao.xyz/Article/details/gapsenshu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fanxiaobao.xyz/Article/details/gtvfhbyzj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fanxiaobao.xyz/Article/details/gygkqapas.sHtML

[Q15] 查询全部
来源：http://blog.fanxiaobao.xyz/Article/details/gkagwgnxe.sHtML

SELECT * FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqucnydlw.sHtML

[Q16] 查询指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gddzmklfz.sHtML

SELECT id, name FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gronmrkbh.sHtML

[Q17] 条件查询
来源：http://3g.fanxiaobao.xyz/Article/details/gwpbnlsiu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkikjnwn.sHtML

[Q18] 模糊匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gcbgbymfn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fanxiaobao.xyz/Article/details/gqpdwkook.sHtML

[Q19] 范围查询
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwvejjha.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fanxiaobao.xyz/Article/details/gzmczxvxx.sHtML

[Q20] IN 列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gjelddakb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gomhgscyx.sHtML

[Q21] 空值判断
来源：http://wap.fanxiaobao.xyz/Article/details/gojzvdssw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fanxiaobao.xyz/Article/details/ggqjmmohd.sHtML

[Q22] 排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gykznccsz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fanxiaobao.xyz/Article/details/gnnayoinu.sHtML

[Q23] 分页
来源：http://wap.fanxiaobao.xyz/Article/details/gaygghwxd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fanxiaobao.xyz/Article/details/gwalrpkeo.sHtML

[Q24] 去重
来源：http://3g.fanxiaobao.xyz/Article/details/gesiakqnk.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gsphafssz.sHtML

[Q25] 只取前 N 条
来源：http://3g.fanxiaobao.xyz/Article/details/ggtmjixar.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fanxiaobao.xyz/Article/details/gntmtqvil.sHtML

[Q26] 计数
来源：http://read.share.fanxiaobao.xyz/Article/details/gqoshrirq.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glophapgu.sHtML

[Q27] 条件计数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnoskqlw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznbfwmju.sHtML

[Q28] 求和与平均
来源：http://baike.fanxiaobao.xyz/Article/details/glputjyam.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvsmymqe.sHtML

[Q29] 最大最小值
来源：http://blog.fanxiaobao.xyz/Article/details/ghmsplyme.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gojwxioln.sHtML

[Q30] 分组统计
来源：http://baike.fanxiaobao.xyz/Article/details/gpsiljyzr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gcvleulhz.sHtML

[Q31] 分组后过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvqatvuu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gqxylkpxw.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbnvccxt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gxuwqbslv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fanxiaobao.xyz/Article/details/gbaqvqnxp.sHtML

[Q33] 多列分组
来源：http://3g.fanxiaobao.xyz/Article/details/ghkrdyvls.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fanxiaobao.xyz/Article/details/grugregnv.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzdfphng.sHtML

SELECT * FROM (
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvvkbqug.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fanxiaobao.xyz/Article/details/gtryhhzzo.sHtML

) t WHERE rn = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsxbdotg.sHtML

[Q35] 内连接
来源：http://blog.fanxiaobao.xyz/Article/details/gmfsleybl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhwnamrq.sHtML

[Q36] 左连接
来源：http://blog.fanxiaobao.xyz/Article/details/gwxrkwptw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gyaapxqdc.sHtML

[Q37] 右连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gptpyvjmq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gqiejxxgr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fanxiaobao.xyz/Article/details/gnysrocmh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjzwbrre.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdsmwnnb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fanxiaobao.xyz/Article/details/gnrjlqsvz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gplmrodtz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fanxiaobao.xyz/Article/details/glhgnilpt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fanxiaobao.xyz/Article/details/gutxfpyhd.sHtML

[Q41] 多表连接
来源：http://baike.fanxiaobao.xyz/Article/details/gloitlonm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwgcdpsp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fanxiaobao.xyz/Article/details/giawokndt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwjuvykk.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gzboqfikw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fanxiaobao.xyz/Article/details/glqidzxql.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gkdqathhz.sHtML

[Q43] 标量子查询
来源：http://wap.fanxiaobao.xyz/Article/details/gmckyxvei.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fanxiaobao.xyz/Article/details/gthjjjtso.sHtML

[Q44] IN 子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gzeswkmpw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcffexvzx.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fanxiaobao.xyz/Article/details/gpxvwepoc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvykticx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fanxiaobao.xyz/Article/details/gdxdtlqss.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gagmkwpnv.sHtML

[Q47] 与平均值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gobvgukao.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fanxiaobao.xyz/Article/details/gerccmbui.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggybhfbfn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fanxiaobao.xyz/Article/details/gyyczqrve.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/grrolfaex.sHtML

[Q49] 更新单行
来源：http://wap.fanxiaobao.xyz/Article/details/gyxuuwncg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbljoljf.sHtML

[Q50] 批量更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpgpahlg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gxnzdxypv.sHtML

[Q51] 用子查询更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gbholjaco.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdparisxw.sHtML

[Q52] 删除指定行
来源：http://3g.fanxiaobao.xyz/Article/details/gprbpbzsm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gwkcjttor.sHtML

[Q53] 按条件删除
来源：http://baike.fanxiaobao.xyz/Article/details/gmphilttb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjwqjhrj.sHtML

[Q54] 清空表
来源：http://baike.fanxiaobao.xyz/Article/details/gkmfpkmjt.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnjgqneh.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fanxiaobao.xyz/Article/details/giiauukvz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/glnxuqzre.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfssffpb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmhatcot.sHtML

[Q57] 行号
来源：http://blog.fanxiaobao.xyz/Article/details/gabfrtujf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwyzdgdr.sHtML

[Q58] 累计求和
来源：http://blog.fanxiaobao.xyz/Article/details/gbajmjreo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gbmlyphvg.sHtML

[Q59] 分组内累计
来源：http://www.share.fanxiaobao.xyz/Article/details/gpuwubtmk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxqeoloc.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fanxiaobao.xyz/Article/details/goydkthnh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fanxiaobao.xyz/Article/details/guembvamf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxluncupl.sHtML

[Q61] 移动平均
来源：http://3g.fanxiaobao.xyz/Article/details/grhoyridf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gjgnichdm.sHtML

[Q62] 分组占比
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmpyduor.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/glglirrde.sHtML

[Q63] 开启事务
来源：http://3g.fanxiaobao.xyz/Article/details/gascszqwc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxfhnzqp.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgglybcd.sHtML

COMMIT;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzarmpnmr.sHtML

[Q65] 回滚事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzdxzvjr.sHtML

ROLLBACK;
来源：http://3g.fanxiaobao.xyz/Article/details/gaenlwglg.sHtML

[Q66] 行锁查询
来源：http://blog.fanxiaobao.xyz/Article/details/ggqzaxukt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fanxiaobao.xyz/Article/details/gqjaxwuso.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyefhzia.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fanxiaobao.xyz/Article/details/gycwsdcwm.sHtML

[Q68] 保存点
来源：http://mobile.fanxiaobao.xyz/Article/details/glrnvrlle.sHtML

SAVEPOINT sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gsgbieyxg.sHtML

ROLLBACK TO sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gmxwpcowk.sHtML

[Q69] 查看执行计划
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhbhrnlk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fanxiaobao.xyz/Article/details/gkxrkkqab.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/gngtbzkac.sHtML

ANALYZE TABLE users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzqhsvyq.sHtML

[Q71] 查看建表语句
来源：http://wap.fanxiaobao.xyz/Article/details/gkxbytuqz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbgvqhmr.sHtML

[Q72] 查看索引
来源：http://wap.fanxiaobao.xyz/Article/details/gwclxfywo.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwppgddyy.sHtML

[Q73] 查看表状态
来源：http://read.share.fanxiaobao.xyz/Article/details/gieiftxvq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gztfsiapx.sHtML

[Q74] 强制使用索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gieoixpzb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqruqgjh.sHtML

[Q75] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gzqjmcriw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqibbdkf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocvnoyjp.sHtML

[Q76] 按天统计
来源：http://wap.fanxiaobao.xyz/Article/details/gmaeirxzq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/gnuvoseon.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/gjkpigesl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fanxiaobao.xyz/Article/details/gmrjbenoq.sHtML

[Q78] 当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gwnquzoob.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihxrhfca.sHtML

[Q79] 字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gkhxpoyfm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/gdaphvkpm.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtgqhhhh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvclmnonz.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtmxbymg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtotfzwpj.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fanxiaobao.xyz/Article/details/gwegldjvh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjbcsrhj.sHtML

[Q83] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gghblktcd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfhjzdsh.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/ggqpvseyc.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdblwqggz.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/gssenyteq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbnqdpux.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/gnhghpfqq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/gfxjreclw.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/gtpvrcuqn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgarltkx.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcdbhsgt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fanxiaobao.xyz/Article/details/glryxkuco.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gytaiooyw.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwsmcojd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gyrdcpysv.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/gjamszcgq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giahtgwbu.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgevmywe.sHtML

R. Bash 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbnjrgwm.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gimxsdbjb.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/glvgcznea.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/ggszqukfo.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonpkwcmz.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjcbptvb.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcxfxima.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqymqage.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/grisbyggl.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfhokruv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/ggirurxzd.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/guwfcwhsg.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtjjnjbe.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gttcnopsk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfrsjxeui.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/gyiggtcrg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpwvrwqz.sHtML

[R08] 数值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzydygdgq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwbsomhg.sHtML

[R09] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gipslkmez.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gyscmkscl.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxrrvoyy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gsweprkwb.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/glxxoance.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/gnykmlbii.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplcmkveo.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcayutzma.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/giszvabbq.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gcjsmqerg.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfyzgyvh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gzfxspgrb.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gpblzpoxr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/ghtetvdca.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/grohridjn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gkovgbaee.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/giqvharkq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gvqpyahft.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/genpfzwrg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gvnvupups.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/glcuogfmt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gikboulyy.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmdhffbj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gswcsojhk.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfchnsnmr.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gegztvmnq.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzhlihqd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjucfvmr.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdscyvefq.sHtML


<!-- 参考信息 -->