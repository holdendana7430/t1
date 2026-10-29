代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/gveviyugp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/gngimtrfz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gttgucltz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/gmjflzmuu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/gkqaypjbt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fehbvm.com/Article/details/gswqsejex.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fehbvm.com/Article/details/gpdflxtsg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.hesvh.cn/Article/details/gjyjytvwn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.zdbjq.cn/Article/details/gedryzrbi.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gfcpetzmd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gzrwmbhpj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fehbvm.com/Article/details/gujrquiqi.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fehbvm.com/Article/details/gbqoxskio.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.hesvh.cn/Article/details/gcdualikd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fehbvm.com/Article/details/glylnwmrf.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/gesbiscko.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.zdbjq.cn/Article/details/gtszbbzsd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gnpibtffy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gzebapwzx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gwhekthjk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fehbvm.com/Article/details/ggoqskfxn.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/gictxhkrs.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/gggdkvlnj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.zdbjq.cn/Article/details/gypxfqlfd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/gohgmpone.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.hesvh.cn/Article/details/gcmpygqry.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/gkcaxhchz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.zdbjq.cn/Article/details/gyjmukiyu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gilrkfffn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.hesvh.cn/Article/details/glvnxompq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.zdbjq.cn/Article/details/gtkzjoptj.sHtML

Ruby: a == b
来源：http://read.share.zdbjq.cn/Article/details/gcyuxrkwq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.hesvh.cn/Article/details/gysmuaddl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.zdbjq.cn/Article/details/gurfaspml.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.hesvh.cn/Article/details/gptquplcn.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.zdbjq.cn/Article/details/giijathhs.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/galncyyxi.sHtML

TS:   if (x == null) {}
来源：http://wap.zdbjq.cn/Article/details/gugadvhhv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gcvbowloh.sHtML

Go:   if x == nil {}
来源：http://mobile.hesvh.cn/Article/details/gnkdkattj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.hesvh.cn/Article/details/gnfwbldzz.sHtML

C#:   if (x is null) {}
来源：http://www.share.zdbjq.cn/Article/details/gocqsutgt.sHtML

[P07] 防抖与节流
来源：http://www.blog.zdbjq.cn/Article/details/glrgihoyo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fehbvm.com/Article/details/gwgxnkhio.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.zdbjq.cn/Article/details/gvcugifmb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gjbxvlqzn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gvdkvtsqu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.hesvh.cn/Article/details/gqhflehec.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.zdbjq.cn/Article/details/gdixnmqog.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/gwgvggeaq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.hesvh.cn/Article/details/gwpkxddrp.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fehbvm.com/Article/details/gdihdpxjb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.hesvh.cn/Article/details/gcpgfcvrf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.zdbjq.cn/Article/details/gyufnglql.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.hesvh.cn/Article/details/gdwvwfpdx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/goohxlbzz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.zdbjq.cn/Article/details/gktrqhdca.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fehbvm.com/Article/details/gjzudwmas.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fehbvm.com/Article/details/gqhvnsefa.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.hesvh.cn/Article/details/gmyhqwqvl.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gblfjycda.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.hesvh.cn/Article/details/ghcgowegs.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkcqcmxeg.sHtML

[Q01] 创建表
来源：http://m.share.hesvh.cn/Article/details/gticsbeux.sHtML

CREATE TABLE users (
来源：http://read.share.fehbvm.com/Article/details/gxsfwsnht.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gwxzeawnr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/guuqdpevf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.zdbjq.cn/Article/details/gzcgejzph.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.hesvh.cn/Article/details/gafnuofav.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gusecxhbr.sHtML

[Q02] 创建带外键的表
来源：http://baike.hesvh.cn/Article/details/gczigsiiz.sHtML

CREATE TABLE orders (
来源：http://m.share.fehbvm.com/Article/details/gbaqbihao.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gywxlztkx.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gazxctxkl.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fehbvm.com/Article/details/gdpogbcsb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fehbvm.com/Article/details/gmokfyvxg.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gyqhycmxz.sHtML

[Q03] 增加列
来源：http://wap.zdbjq.cn/Article/details/gcnqcxami.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fehbvm.com/Article/details/gsmqwgswh.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/gckarabhs.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gulcfzvoe.sHtML

[Q05] 重命名列
来源：http://www.blog.fehbvm.com/Article/details/guvgsyavl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fehbvm.com/Article/details/gtpmfjjdm.sHtML

[Q06] 删除列
来源：http://wap.fehbvm.com/Article/details/gwklizbqa.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.hesvh.cn/Article/details/gmufkvool.sHtML

[Q07] 删除表
来源：http://blog.hesvh.cn/Article/details/gecntpqhn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.zdbjq.cn/Article/details/grmvkvwqd.sHtML

[Q08] 创建普通索引
来源：http://m.share.hesvh.cn/Article/details/gjzmzuwmw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gxjszyvfl.sHtML

[Q09] 创建唯一索引
来源：http://3g.zdbjq.cn/Article/details/gsxowbgqu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/giovffgcp.sHtML

[Q10] 插入单行
来源：http://3g.fehbvm.com/Article/details/godtasdrj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.hesvh.cn/Article/details/gnbqapabp.sHtML

[Q11] 一次插入多行
来源：http://www.share.fehbvm.com/Article/details/gaqbdecdd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fehbvm.com/Article/details/gjnuqwycp.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/grchdvnis.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fehbvm.com/Article/details/gstkkdnyi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.zdbjq.cn/Article/details/gotmjijrj.sHtML

[Q13] 忽略重复插入
来源：http://mobile.zdbjq.cn/Article/details/gbtnrikmd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gwxxgrofp.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.hesvh.cn/Article/details/gzxuanzgr.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fehbvm.com/Article/details/guackdfrt.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.zdbjq.cn/Article/details/gphnjttni.sHtML

[Q15] 查询全部
来源：http://www.m.share.fehbvm.com/Article/details/glvnijsyb.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/gcyqkxvhx.sHtML

[Q16] 查询指定列
来源：http://m.share.fehbvm.com/Article/details/gaqzpdrqk.sHtML

SELECT id, name FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ghcqxdbed.sHtML

[Q17] 条件查询
来源：http://3g.zdbjq.cn/Article/details/grfgflhuo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gheknmymb.sHtML

[Q18] 模糊匹配
来源：http://baike.hesvh.cn/Article/details/gijonocaf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.hesvh.cn/Article/details/gqtfwafra.sHtML

[Q19] 范围查询
来源：http://www.blog.fehbvm.com/Article/details/gjkrtvceq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fehbvm.com/Article/details/gmwhitqcc.sHtML

[Q20] IN 列表
来源：http://read.share.zdbjq.cn/Article/details/gbheuwggg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.zdbjq.cn/Article/details/grrhnjmxm.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/gwdltznsz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.hesvh.cn/Article/details/ggsspaukk.sHtML

[Q22] 排序
来源：http://read.share.fehbvm.com/Article/details/gjeibgiuo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/gsepevknp.sHtML

[Q23] 分页
来源：http://baike.fehbvm.com/Article/details/ggpoixupr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fehbvm.com/Article/details/giwgrhmgh.sHtML

[Q24] 去重
来源：http://www.blog.fehbvm.com/Article/details/gxclsbxfd.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gjmbodcta.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/gtlaanmih.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.zdbjq.cn/Article/details/gvmzvjsvc.sHtML

[Q26] 计数
来源：http://mobile.fehbvm.com/Article/details/gdijvqfrj.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gdvkravll.sHtML

[Q27] 条件计数
来源：http://m.share.hesvh.cn/Article/details/gmkmhelau.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.zdbjq.cn/Article/details/ggpesezwr.sHtML

[Q28] 求和与平均
来源：http://blog.hesvh.cn/Article/details/gplnqjvbh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/glwmvglzj.sHtML

[Q29] 最大最小值
来源：http://baike.hesvh.cn/Article/details/grilmuyev.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.hesvh.cn/Article/details/glmswyweg.sHtML

[Q30] 分组统计
来源：http://baike.hesvh.cn/Article/details/gttlpdjlj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gavgrpwwd.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/gdasfpkaq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fehbvm.com/Article/details/gwihsldee.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gvtyspxtt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gwcsbdwoi.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.zdbjq.cn/Article/details/gpfymkqdz.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/grvbkwpnp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/gqigfunwf.sHtML

[Q34] 每组取第一条
来源：http://www.share.fehbvm.com/Article/details/gbxujjdoe.sHtML

SELECT * FROM (
来源：http://mobile.hesvh.cn/Article/details/gplyoogqx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.zdbjq.cn/Article/details/ggfvakbea.sHtML

) t WHERE rn = 1;
来源：http://baike.hesvh.cn/Article/details/gdpwmxofd.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/ghxmqebxw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/ghaigdftf.sHtML

[Q36] 左连接
来源：http://www.m.share.fehbvm.com/Article/details/grdxjmdek.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gontjnyzo.sHtML

[Q37] 右连接
来源：http://read.share.hesvh.cn/Article/details/gobljxuor.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.zdbjq.cn/Article/details/gxgibdsxg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.zdbjq.cn/Article/details/gscjxjqot.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fehbvm.com/Article/details/gzugnamrl.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fehbvm.com/Article/details/gccomcnpm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fehbvm.com/Article/details/gdynpjhyi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.hesvh.cn/Article/details/grwfkfdsv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fehbvm.com/Article/details/gbytuqezb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.zdbjq.cn/Article/details/gwppvoxvr.sHtML

[Q41] 多表连接
来源：http://www.blog.fehbvm.com/Article/details/gvwbwlyuv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fehbvm.com/Article/details/gemluftfw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/gyiuoxvcx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/gmaroazvz.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.hesvh.cn/Article/details/gtrghzhdn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.zdbjq.cn/Article/details/gmocnsynw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.zdbjq.cn/Article/details/gxbxzznku.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/gfegjxjmn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gvmzjxjay.sHtML

[Q44] IN 子查询
来源：http://www.blog.hesvh.cn/Article/details/gecqxwwtk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fehbvm.com/Article/details/gcvqnokoz.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.hesvh.cn/Article/details/gknedwggs.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gzsxzjbww.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fehbvm.com/Article/details/geazryozu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gbqzkctpk.sHtML

[Q47] 与平均值比较
来源：http://3g.hesvh.cn/Article/details/gzxrjbhcq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gjvwwdpcp.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.zdbjq.cn/Article/details/gmlntgtss.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fehbvm.com/Article/details/gooexzefr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/gqjwxyvne.sHtML

[Q49] 更新单行
来源：http://blog.hesvh.cn/Article/details/gfkqfgnik.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gjjkdtmnx.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/gflupqzlv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gcomeppxv.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/gjflltknb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.zdbjq.cn/Article/details/grmufbqew.sHtML

[Q52] 删除指定行
来源：http://read.share.fehbvm.com/Article/details/gdmsirmyf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gstysyqds.sHtML

[Q53] 按条件删除
来源：http://3g.fehbvm.com/Article/details/gcegztnak.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/glniuaiyo.sHtML

[Q54] 清空表
来源：http://m.share.hesvh.cn/Article/details/grmwbxffi.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/gkozzuyim.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.hesvh.cn/Article/details/gcmlhedvc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gjxnkwyeh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.zdbjq.cn/Article/details/gazhqubjk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fehbvm.com/Article/details/gjsgfoxfz.sHtML

[Q57] 行号
来源：http://baike.zdbjq.cn/Article/details/gsgueothk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fehbvm.com/Article/details/gjrmppahz.sHtML

[Q58] 累计求和
来源：http://blog.fehbvm.com/Article/details/giseaobxa.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/gwmltgjno.sHtML

[Q59] 分组内累计
来源：http://blog.zdbjq.cn/Article/details/grnholdcr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gnzvkxoot.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gyusbbwtk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fehbvm.com/Article/details/gyhddpbiz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gzczmaita.sHtML

[Q61] 移动平均
来源：http://blog.fehbvm.com/Article/details/gngtxzfdi.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/glhrjzhnx.sHtML

[Q62] 分组占比
来源：http://www.share.hesvh.cn/Article/details/gtfnaqvfw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gyfoqnoyi.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/gmugzjumr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fehbvm.com/Article/details/giwaomyfx.sHtML

[Q64] 提交事务
来源：http://mobile.zdbjq.cn/Article/details/geuwmssmd.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/goeqnheod.sHtML

[Q65] 回滚事务
来源：http://read.share.hesvh.cn/Article/details/gksjmrzjq.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/gfabzjoaw.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/gofbrxtrx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fehbvm.com/Article/details/gntfbbrfv.sHtML

[Q67] 设置隔离级别
来源：http://wap.zdbjq.cn/Article/details/ghdhwrijj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.hesvh.cn/Article/details/grkaesmil.sHtML

[Q68] 保存点
来源：http://www.blog.fehbvm.com/Article/details/gcfapmmfg.sHtML

SAVEPOINT sp1;
来源：http://wap.zdbjq.cn/Article/details/gouxaoaqq.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fehbvm.com/Article/details/givssbikr.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/gwrjqhcrg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fehbvm.com/Article/details/gopfbgfxi.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/gtzdvtflr.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fehbvm.com/Article/details/gyeuegrqe.sHtML

[Q71] 查看建表语句
来源：http://mobile.zdbjq.cn/Article/details/gdpsjsmbq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/grvyftzpk.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/gcmvvobcj.sHtML

SHOW INDEX FROM users;
来源：http://m.share.hesvh.cn/Article/details/grgkqbkyn.sHtML

[Q73] 查看表状态
来源：http://3g.zdbjq.cn/Article/details/ggielxegr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fehbvm.com/Article/details/gubdlgmrd.sHtML

[Q74] 强制使用索引
来源：http://www.share.hesvh.cn/Article/details/gxnwlsffh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/gkwldodnq.sHtML

[Q75] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gfkuydrlz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gqmepprht.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.hesvh.cn/Article/details/gzgbfatab.sHtML

[Q76] 按天统计
来源：http://www.m.share.fehbvm.com/Article/details/gkbfretee.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.hesvh.cn/Article/details/gchuhogjd.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/gdzwnepjw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/gbwzpebyr.sHtML

[Q78] 当前时间
来源：http://mobile.zdbjq.cn/Article/details/gyxxleabc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fehbvm.com/Article/details/gnzbbsnbc.sHtML

[Q79] 字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gbnbbkfpz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.hesvh.cn/Article/details/geeefhkgw.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/gfofmfcbt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gfpavugzw.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gxhptaegn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fehbvm.com/Article/details/gkmlqewci.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gipqxcemp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/guhkdcjgz.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gtmgegplo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/glunedqzz.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fehbvm.com/Article/details/gwrkyxecd.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gjqgnsyuw.sHtML

[Q85] 数值取整
来源：http://read.share.fehbvm.com/Article/details/gijmmespf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.hesvh.cn/Article/details/gqsrcfvbk.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fehbvm.com/Article/details/gdxpagqcd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fehbvm.com/Article/details/gsplmerku.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/gwvjgpmjq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/givrhveib.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fehbvm.com/Article/details/gbgpixwid.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/gedmdzkkk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/gojbmavrk.sHtML

[Q89] 判断表是否存在
来源：http://baike.hesvh.cn/Article/details/grpqnqxas.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.zdbjq.cn/Article/details/glgdraqex.sHtML

[Q90] 生成序号列
来源：http://wap.zdbjq.cn/Article/details/gsgfktxgu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fehbvm.com/Article/details/ggiaskbaa.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpczouzcp.sHtML

R. Bash 专题
来源：http://blog.fehbvm.com/Article/details/gnvjkctnt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grxiutqli.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/gzzaxljoj.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/gemsfpclp.sHtML

set -euo pipefail
来源：http://read.share.hesvh.cn/Article/details/grgscsgpg.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/gwtrvlwbl.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/gxkeqsouw.sHtML

[R03] 只读变量
来源：http://m.share.zdbjq.cn/Article/details/gkqmcotzx.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/gfxlpddgn.sHtML

[R04] 位置参数
来源：http://baike.fehbvm.com/Article/details/gpndhrrtc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/gsiurklil.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/gfcotqjwp.sHtML

name="${1:-default}"
来源：http://wap.hesvh.cn/Article/details/gnlhchcha.sHtML

[R06] 判断命令是否存在
来源：http://m.share.zdbjq.cn/Article/details/gdbftodfo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gsuytrved.sHtML

[R07] if 判断文件
来源：http://mobile.hesvh.cn/Article/details/grqlzozbi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fehbvm.com/Article/details/gttcewzov.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gtdqvzzth.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.zdbjq.cn/Article/details/goxtukxto.sHtML

[R09] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gtqbhcnbx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/gxwtmiwzr.sHtML

[R10] 正则匹配
来源：http://blog.hesvh.cn/Article/details/gxtllbafv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.zdbjq.cn/Article/details/gnducphdx.sHtML

[R11] case 多分支
来源：http://blog.hesvh.cn/Article/details/gtuebqllt.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/gwcuicbho.sHtML

start) echo "启动" ;;
来源：http://read.share.zdbjq.cn/Article/details/gwrhqvsrx.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/goleygfyy.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fehbvm.com/Article/details/ggkwgvgpb.sHtML

esac
来源：http://read.share.fehbvm.com/Article/details/gmjoqkxho.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/gnocqocem.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.hesvh.cn/Article/details/gabqglnyz.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gisvdljvv.sHtML


<!-- 参考信息 -->