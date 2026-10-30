代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkzwwhso.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzagockc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxrsfizs.sHtML

[P04] 求长度
来源：http://blog.fanxiaobao.xyz/Article/details/gisrgorgx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fanxiaobao.xyz/Article/details/gljbywgwr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykaxddwi.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fanxiaobao.xyz/Article/details/gucsrnmqp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fanxiaobao.xyz/Article/details/gseyjrtgx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnnhnutm.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphbhghwy.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkbbsmcz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgejiwik.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnjuxboy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fanxiaobao.xyz/Article/details/gzolprjri.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fanxiaobao.xyz/Article/details/gwrwncrxk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fanxiaobao.xyz/Article/details/gkngupnhz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsvmamwa.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fanxiaobao.xyz/Article/details/ghhgglnza.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkdvsdqc.sHtML

Ruby: a == b
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkkikzty.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fanxiaobao.xyz/Article/details/gwysekyrb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwjyqrhw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fanxiaobao.xyz/Article/details/gadxptynx.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gualcbnal.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkebvshy.sHtML

TS:   if (x == null) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjtoeukn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvgyvbdh.sHtML

Go:   if x == nil {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqedfmmbj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fanxiaobao.xyz/Article/details/gjmhyzjzp.sHtML

C#:   if (x is null) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gliexkgvf.sHtML

[P07] 防抖与节流
来源：http://baike.fanxiaobao.xyz/Article/details/gcgkhjvbh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfymotfoo.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfutbymp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gomgleipm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gtvagempy.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxqbeooc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpixrdhll.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fanxiaobao.xyz/Article/details/giurevpry.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fanxiaobao.xyz/Article/details/gupznjjqt.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fanxiaobao.xyz/Article/details/gqequgbra.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlofbutj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gymeodacc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmvozfdk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fanxiaobao.xyz/Article/details/gnzwyqgtv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fanxiaobao.xyz/Article/details/grheogokt.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fanxiaobao.xyz/Article/details/grlilnegd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxuriqlbo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacllnytq.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gnczgmdos.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fanxiaobao.xyz/Article/details/gpybqwxfv.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gmahsjqss.sHtML

[Q01] 创建表
来源：http://wap.fanxiaobao.xyz/Article/details/gjokoroxz.sHtML

CREATE TABLE users (
来源：http://baike.fanxiaobao.xyz/Article/details/gyrhrlmmc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhjrxlwq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsflcxcym.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnbjevwy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyvuoeck.sHtML

);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpqlqdmb.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fanxiaobao.xyz/Article/details/gaucqcofe.sHtML

CREATE TABLE orders (
来源：http://baike.fanxiaobao.xyz/Article/details/gjucpolja.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fanxiaobao.xyz/Article/details/gtldyjnco.sHtML

user_id INT NOT NULL,
来源：http://mobile.fanxiaobao.xyz/Article/details/gssmwiloq.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjnqirgo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzappovz.sHtML

);
来源：http://baike.fanxiaobao.xyz/Article/details/gyhkwatdy.sHtML

[Q03] 增加列
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzugugfc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfdevfng.sHtML

[Q04] 修改列类型
来源：http://wap.fanxiaobao.xyz/Article/details/gddpcnzgs.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzzvnpry.sHtML

[Q05] 重命名列
来源：http://mobile.fanxiaobao.xyz/Article/details/gtganczsg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fanxiaobao.xyz/Article/details/gurxuflaa.sHtML

[Q06] 删除列
来源：http://3g.fanxiaobao.xyz/Article/details/gvcsneldl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fanxiaobao.xyz/Article/details/gumfkoynf.sHtML

[Q07] 删除表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggwypljk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fanxiaobao.xyz/Article/details/goodmnggu.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzpqhrad.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhxrkyvz.sHtML

[Q09] 创建唯一索引
来源：http://3g.fanxiaobao.xyz/Article/details/gugpgzlcs.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxubkmjp.sHtML

[Q10] 插入单行
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqinbgee.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/gpalwhavy.sHtML

[Q11] 一次插入多行
来源：http://m.share.fanxiaobao.xyz/Article/details/ghegvyudg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsshdsegs.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqkhsmjh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fanxiaobao.xyz/Article/details/gmorjsaka.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fanxiaobao.xyz/Article/details/gkozlrfdv.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdalvcay.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxzjpfyk.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fanxiaobao.xyz/Article/details/gounjuqhd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqzmnusb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fanxiaobao.xyz/Article/details/gknsnnowp.sHtML

[Q15] 查询全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvyekpwh.sHtML

SELECT * FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gamfimuqh.sHtML

[Q16] 查询指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gadmclocx.sHtML

SELECT id, name FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gvjxaaedo.sHtML

[Q17] 条件查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazomebuc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/ggzfnkqne.sHtML

[Q18] 模糊匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxscrivi.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgbzgrzo.sHtML

[Q19] 范围查询
来源：http://wap.fanxiaobao.xyz/Article/details/gapsjaehx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fanxiaobao.xyz/Article/details/guoavoncr.sHtML

[Q20] IN 列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwkmxqjf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gmedyomfc.sHtML

[Q21] 空值判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpybwcuf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqtpkydd.sHtML

[Q22] 排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkszjtqe.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzdbyoci.sHtML

[Q23] 分页
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwpjkybi.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnvttlcs.sHtML

[Q24] 去重
来源：http://wap.fanxiaobao.xyz/Article/details/gljeypkyt.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gjogajowq.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gsldrvllg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fanxiaobao.xyz/Article/details/gbporvygq.sHtML

[Q26] 计数
来源：http://mobile.fanxiaobao.xyz/Article/details/giutzdmav.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/guxsbqkbv.sHtML

[Q27] 条件计数
来源：http://baike.fanxiaobao.xyz/Article/details/gicvhhzzd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcrbgirv.sHtML

[Q28] 求和与平均
来源：http://read.share.fanxiaobao.xyz/Article/details/gznlrteeu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxolehlkt.sHtML

[Q29] 最大最小值
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxhtxbjc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gzokrifyr.sHtML

[Q30] 分组统计
来源：http://baike.fanxiaobao.xyz/Article/details/gshoovmaq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gewpctbfg.sHtML

[Q31] 分组后过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gjzwvnvzz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbxghtuw.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gfhgyzmds.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gppexedai.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmpkvkpj.sHtML

[Q33] 多列分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gtisdbwmg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fanxiaobao.xyz/Article/details/gyqqahyji.sHtML

[Q34] 每组取第一条
来源：http://blog.fanxiaobao.xyz/Article/details/guoiwdrkj.sHtML

SELECT * FROM (
来源：http://read.share.fanxiaobao.xyz/Article/details/glabydqiv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fanxiaobao.xyz/Article/details/gwbcmjwrd.sHtML

) t WHERE rn = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwethpyf.sHtML

[Q35] 内连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdgkkekr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gaahflekg.sHtML

[Q36] 左连接
来源：http://baike.fanxiaobao.xyz/Article/details/gownsoujc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gwrwkmjtb.sHtML

[Q37] 右连接
来源：http://blog.fanxiaobao.xyz/Article/details/gaugawrjb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gmbsghcga.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fanxiaobao.xyz/Article/details/gcmtyrnlw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkwtrzsx.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fanxiaobao.xyz/Article/details/gofpqrnkk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fanxiaobao.xyz/Article/details/gmhiwjhxm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/grcozmpuk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fanxiaobao.xyz/Article/details/glollkbkf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqdqdfpd.sHtML

[Q41] 多表连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggztecsvp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvewmhbj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyagdubl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjspcteeq.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gppnoapes.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbjgfrvc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gatvmtjng.sHtML

[Q43] 标量子查询
来源：http://baike.fanxiaobao.xyz/Article/details/guiayfisf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fanxiaobao.xyz/Article/details/gphljdyjk.sHtML

[Q44] IN 子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqokalcph.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galpvbgxi.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcibmami.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjdalzym.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnzfpshh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gfoockhhm.sHtML

[Q47] 与平均值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gouohfksn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fanxiaobao.xyz/Article/details/gzcflehpi.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtntklcyk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fanxiaobao.xyz/Article/details/gzbcycots.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gbzkckkfd.sHtML

[Q49] 更新单行
来源：http://baike.fanxiaobao.xyz/Article/details/gdhsknzvz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gshrwgckx.sHtML

[Q50] 批量更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpxbpudh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gykvaqoid.sHtML

[Q51] 用子查询更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpyglwzc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gnuuvqewe.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhnlucvh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvbmwruy.sHtML

[Q53] 按条件删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbwxeulx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gfgaydlps.sHtML

[Q54] 清空表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbilcgjwe.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyqnzjlb.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzahqcvll.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfsyacys.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fanxiaobao.xyz/Article/details/guuvapcab.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/grolwabib.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/grugjaong.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gscciitns.sHtML

[Q58] 累计求和
来源：http://3g.fanxiaobao.xyz/Article/details/gugowiqit.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxtkaywd.sHtML

[Q59] 分组内累计
来源：http://read.share.fanxiaobao.xyz/Article/details/gqioygxwf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/grbpgdkvz.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fanxiaobao.xyz/Article/details/gojppiocd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fanxiaobao.xyz/Article/details/guvxsifoe.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtheneipy.sHtML

[Q61] 移动平均
来源：http://wap.fanxiaobao.xyz/Article/details/gtcpmksim.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwzoyqzx.sHtML

[Q62] 分组占比
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfufiuhg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gfnbvildg.sHtML

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/gyiecfkho.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvphdpmj.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/guerdlmxw.sHtML

COMMIT;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkpklymb.sHtML

[Q65] 回滚事务
来源：http://wap.fanxiaobao.xyz/Article/details/gasmolcgf.sHtML

ROLLBACK;
来源：http://blog.fanxiaobao.xyz/Article/details/gqbrpodfz.sHtML

[Q66] 行锁查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyxirnfr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fanxiaobao.xyz/Article/details/gjooxmmbl.sHtML

[Q67] 设置隔离级别
来源：http://wap.fanxiaobao.xyz/Article/details/gghwswgli.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fanxiaobao.xyz/Article/details/glszkspsx.sHtML

[Q68] 保存点
来源：http://read.share.fanxiaobao.xyz/Article/details/gcuyopktq.sHtML

SAVEPOINT sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gjkscjgli.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gshqdwewy.sHtML

[Q69] 查看执行计划
来源：http://3g.fanxiaobao.xyz/Article/details/gsiynoxrs.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlaidgxj.sHtML

[Q70] 更新统计信息
来源：http://read.share.fanxiaobao.xyz/Article/details/gqesbgpoi.sHtML

ANALYZE TABLE users;
来源：http://3g.fanxiaobao.xyz/Article/details/gsjcwkmrx.sHtML

[Q71] 查看建表语句
来源：http://mobile.fanxiaobao.xyz/Article/details/gztfmkxca.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fanxiaobao.xyz/Article/details/gxuvmygml.sHtML

[Q72] 查看索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gvugjperm.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gaofhufen.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzazdckyg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gcptkrotx.sHtML

[Q74] 强制使用索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gqembvgtr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgxsgnyg.sHtML

[Q75] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gglwegcwg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxjklvww.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fanxiaobao.xyz/Article/details/gelisjgtp.sHtML

[Q76] 按天统计
来源：http://3g.fanxiaobao.xyz/Article/details/gvsybskjf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrxbjzvj.sHtML

[Q77] 时间加减
来源：http://blog.fanxiaobao.xyz/Article/details/gjozgfjzu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/gvsdpqvmd.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/guewozeag.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/glhdnitgf.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpazhigt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fanxiaobao.xyz/Article/details/gavldowai.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxcwaisq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqfgcjhh.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gqrznudme.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzifdiqjh.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fanxiaobao.xyz/Article/details/gsksfvsjj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gufzzfbuw.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevsurbnf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/glqstaawh.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gwfprscub.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyiowvzgr.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/gpskvvhtw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fanxiaobao.xyz/Article/details/gcrzuegzi.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fanxiaobao.xyz/Article/details/giubjlupw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/gmqzqgcij.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/gjurunsje.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/gimcjexez.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/ghjmvgumi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/gjykdlbht.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/ggbryirgt.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlacruij.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/guqhwihan.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/gszbhmjux.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gxtjyjobj.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gzuubhiwp.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbcnoygi.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ggicyupvz.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gabiycrbx.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/gaeripxwo.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/glxehbctp.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/gjrkhzbiu.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/gjeyfmwoc.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxmkgrgg.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtenldxpx.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnevsnzx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjyjemlcd.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gweluwfgs.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxomdwdff.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/guhymcaeh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gypvyauao.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/gwycqzrio.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhpclbxe.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmuwjrex.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gebkewbsq.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwuuhjjcd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gnsbuefke.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gblrhnlxd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gojwuhugu.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gomhbkzvv.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkyiawtw.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspnpxrjk.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakwdxuxi.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gmmzxdtfr.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gairkqohr.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/gwoyvhimg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gskqufvpl.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gxkwambkb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/ghiieacav.sHtML

[R14] C 风格 for
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrvdrrji.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/garkkgyxw.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gtcumdnio.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzanblra.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gpotxfeua.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/grnicglfo.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbqqnvfh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gzrqniely.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkqpsyef.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gbvsqbotw.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gfytfsblb.sHtML


<!-- 参考信息 -->