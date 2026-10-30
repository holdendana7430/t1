代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fehbvm.com/Article/details/gshcfxryb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/ghxcbjsbf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fehbvm.com/Article/details/gxcnaeufo.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.zdbjq.cn/Article/details/gogmxihmh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fehbvm.com/Article/details/gwjbacwkr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.zdbjq.cn/Article/details/gntbquuvc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.zdbjq.cn/Article/details/gpqkqmezd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.hesvh.cn/Article/details/gyygibpal.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fehbvm.com/Article/details/gxqgqwhcr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fehbvm.com/Article/details/ggdxlqaxn.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/gsnrjreeh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.zdbjq.cn/Article/details/gkfsmaswp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.zdbjq.cn/Article/details/gjilkwfqa.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/guzubcjzh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gfnzyyxsb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/gmebgnkzi.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.hesvh.cn/Article/details/glfplwrao.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/gnfwdrabc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fehbvm.com/Article/details/gwuuixxxb.sHtML

[P04] 求长度
来源：http://3g.fehbvm.com/Article/details/gwhrslmne.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/gdvzggtqm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/grtyqkyty.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gnkmzjvkl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/ggymjlvwv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/grbvnlktl.sHtML

Go:   len(arr);  len(m)
来源：http://wap.hesvh.cn/Article/details/gslqohkvr.sHtML

Ruby: x.length;  x.size
来源：http://m.share.zdbjq.cn/Article/details/gqpekekuc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fehbvm.com/Article/details/gelpuohlc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.hesvh.cn/Article/details/gxcnvjtpp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.zdbjq.cn/Article/details/gtgrguoln.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.hesvh.cn/Article/details/gzguurzwm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fehbvm.com/Article/details/gzerffdwk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gyazcdwwu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.zdbjq.cn/Article/details/gyhmcvdqs.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.hesvh.cn/Article/details/gfijkkftu.sHtML

Ruby: a == b
来源：http://baike.zdbjq.cn/Article/details/gmlxjmsrf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.zdbjq.cn/Article/details/gcjwpdxnj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.zdbjq.cn/Article/details/gnvgsqjme.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.zdbjq.cn/Article/details/gllbeqzdw.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gknbzorhe.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.zdbjq.cn/Article/details/geetpwbbz.sHtML

TS:   if (x == null) {}
来源：http://mobile.zdbjq.cn/Article/details/gvzjicaux.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gzolaigfe.sHtML

Go:   if x == nil {}
来源：http://blog.zdbjq.cn/Article/details/gxfoxeksz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/gknoharyh.sHtML

C#:   if (x is null) {}
来源：http://blog.hesvh.cn/Article/details/gexbcywhn.sHtML

[P07] 防抖与节流
来源：http://www.blog.zdbjq.cn/Article/details/gffyzfvid.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.hesvh.cn/Article/details/ghuqpwchq.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.zdbjq.cn/Article/details/ghmfiysuw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gnxxzrsqz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gvxjgkznx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.zdbjq.cn/Article/details/gropxyigw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.zdbjq.cn/Article/details/gwoyjjmvc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/gresdbqxp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fehbvm.com/Article/details/gwfnwozpk.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fehbvm.com/Article/details/gugsvgawz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.zdbjq.cn/Article/details/gbalpmsdt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fehbvm.com/Article/details/gfhejttvc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.zdbjq.cn/Article/details/grfinytfl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/gthaxtikw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.zdbjq.cn/Article/details/guaceysuz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fehbvm.com/Article/details/ggfkpvlgy.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fehbvm.com/Article/details/gmqlaaiwo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.hesvh.cn/Article/details/gmxvmhluj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkffmngdj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.hesvh.cn/Article/details/gxroznble.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyjekjwte.sHtML

[Q01] 创建表
来源：http://baike.hesvh.cn/Article/details/gnsdwekuc.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gvuozcrem.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/glvgxfjej.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gaeuzhuad.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fehbvm.com/Article/details/gorudpkug.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.hesvh.cn/Article/details/gkrrzczir.sHtML

);
来源：http://3g.fehbvm.com/Article/details/geudmrzqp.sHtML

[Q02] 创建带外键的表
来源：http://m.share.zdbjq.cn/Article/details/gwbbxgxgc.sHtML

CREATE TABLE orders (
来源：http://www.share.zdbjq.cn/Article/details/gvahirtwv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gygtaxcxr.sHtML

user_id INT NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/grjotkxav.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.zdbjq.cn/Article/details/gacxgwrdb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.zdbjq.cn/Article/details/gpmftzhus.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/geawbazws.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/gjvnnuqxp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.hesvh.cn/Article/details/gylmfgqzd.sHtML

[Q04] 修改列类型
来源：http://mobile.fehbvm.com/Article/details/gdaicymna.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fehbvm.com/Article/details/geurucglx.sHtML

[Q05] 重命名列
来源：http://www.m.share.zdbjq.cn/Article/details/ggvugmvsc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.zdbjq.cn/Article/details/ggnfspkpx.sHtML

[Q06] 删除列
来源：http://www.blog.zdbjq.cn/Article/details/gwxtydukh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/gxksbchui.sHtML

[Q07] 删除表
来源：http://www.m.share.hesvh.cn/Article/details/gwiywqeiz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.hesvh.cn/Article/details/gshvmrvhy.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/gdwrdmfzh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gbjonkmpk.sHtML

[Q09] 创建唯一索引
来源：http://wap.fehbvm.com/Article/details/gonkirhxi.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gizijmsil.sHtML

[Q10] 插入单行
来源：http://www.blog.hesvh.cn/Article/details/gejnxerhe.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fehbvm.com/Article/details/gnvbjsdia.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/gpjeqsxfk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gbbqnglmr.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/gobxfoyut.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fehbvm.com/Article/details/gxjakomwo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.hesvh.cn/Article/details/ghlayodsu.sHtML

[Q13] 忽略重复插入
来源：http://wap.zdbjq.cn/Article/details/gmzltzudo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gvnaawapt.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/gsppxhtqm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/gduwmxzdq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fehbvm.com/Article/details/gbqrkzrys.sHtML

[Q15] 查询全部
来源：http://www.share.fehbvm.com/Article/details/gxiefzqvo.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gkelchdbe.sHtML

[Q16] 查询指定列
来源：http://blog.fehbvm.com/Article/details/gqlyeukro.sHtML

SELECT id, name FROM users;
来源：http://blog.zdbjq.cn/Article/details/gmumlqdnc.sHtML

[Q17] 条件查询
来源：http://mobile.fehbvm.com/Article/details/gazsktvfb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fehbvm.com/Article/details/gqznxjjey.sHtML

[Q18] 模糊匹配
来源：http://wap.zdbjq.cn/Article/details/gxwuajitu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.zdbjq.cn/Article/details/gvgagexcl.sHtML

[Q19] 范围查询
来源：http://3g.hesvh.cn/Article/details/glewmcbwf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.hesvh.cn/Article/details/gdtzgchbg.sHtML

[Q20] IN 列表
来源：http://3g.fehbvm.com/Article/details/gqzynlxfq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.zdbjq.cn/Article/details/gauiewtbj.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/goaofjbxr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gcmescpyg.sHtML

[Q22] 排序
来源：http://m.share.hesvh.cn/Article/details/ggvzvgikl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/gvtosdjut.sHtML

[Q23] 分页
来源：http://3g.hesvh.cn/Article/details/gtdcpirjp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/ghauwgxqa.sHtML

[Q24] 去重
来源：http://3g.zdbjq.cn/Article/details/grkiiemwz.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.hesvh.cn/Article/details/gxfebosjd.sHtML

[Q25] 只取前 N 条
来源：http://mobile.zdbjq.cn/Article/details/ghmgheduq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.zdbjq.cn/Article/details/gnayjviic.sHtML

[Q26] 计数
来源：http://mobile.zdbjq.cn/Article/details/gelmqoqqe.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/ghdoqjwwh.sHtML

[Q27] 条件计数
来源：http://blog.hesvh.cn/Article/details/gucmqivvk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fehbvm.com/Article/details/gwcudtzeh.sHtML

[Q28] 求和与平均
来源：http://www.blog.hesvh.cn/Article/details/gppycxfjc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gdotreykg.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/grffagfaj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.hesvh.cn/Article/details/grycqyyql.sHtML

[Q30] 分组统计
来源：http://3g.zdbjq.cn/Article/details/gtzjnbaso.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gcgtgesgu.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/gzpoakfax.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.zdbjq.cn/Article/details/gzrwfnpxo.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fehbvm.com/Article/details/gmbsciexv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gmqgbhaln.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/gpzdbokse.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/gcbmwbjvl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.hesvh.cn/Article/details/gvzaywafw.sHtML

[Q34] 每组取第一条
来源：http://www.share.zdbjq.cn/Article/details/gggqsebrw.sHtML

SELECT * FROM (
来源：http://read.share.fehbvm.com/Article/details/gxmncxhkt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.zdbjq.cn/Article/details/gyrdjxrox.sHtML

) t WHERE rn = 1;
来源：http://read.share.fehbvm.com/Article/details/gdkmknppl.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/gsfktidwt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gobudtrnm.sHtML

[Q36] 左连接
来源：http://www.blog.fehbvm.com/Article/details/gfzpififs.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gbrdydawl.sHtML

[Q37] 右连接
来源：http://www.m.share.hesvh.cn/Article/details/gaivlfrvd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/gmpoluiny.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/gbhlabzyi.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.zdbjq.cn/Article/details/gzymwuwxo.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.hesvh.cn/Article/details/gylejhcuc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fehbvm.com/Article/details/gregftito.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.hesvh.cn/Article/details/gyuaolbqj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/gkrenvjrs.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.zdbjq.cn/Article/details/ghwqxxsvl.sHtML

[Q41] 多表连接
来源：http://read.share.hesvh.cn/Article/details/gjwmycpep.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fehbvm.com/Article/details/gswlqlnas.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.hesvh.cn/Article/details/gkbnmbreb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.zdbjq.cn/Article/details/gjmtumqam.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.hesvh.cn/Article/details/gboffujbv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.hesvh.cn/Article/details/grscqtttm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/gvqrditgg.sHtML

[Q43] 标量子查询
来源：http://baike.zdbjq.cn/Article/details/ggdfsfrmx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/gfahljldt.sHtML

[Q44] IN 子查询
来源：http://www.m.share.hesvh.cn/Article/details/gdkwrtspl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fehbvm.com/Article/details/gyzwfnzgf.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.hesvh.cn/Article/details/gvqdydshi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gzhzjyekx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.hesvh.cn/Article/details/gihoodyuc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gaqoensub.sHtML

[Q47] 与平均值比较
来源：http://blog.zdbjq.cn/Article/details/gpmpblplr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.hesvh.cn/Article/details/gyghowgzy.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.hesvh.cn/Article/details/gofwvaich.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.hesvh.cn/Article/details/gsqijyuzp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fehbvm.com/Article/details/gkqryrrzb.sHtML

[Q49] 更新单行
来源：http://mobile.hesvh.cn/Article/details/ggngtgjam.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gbsdxbaqc.sHtML

[Q50] 批量更新
来源：http://www.share.hesvh.cn/Article/details/gehogrlry.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.hesvh.cn/Article/details/gunlhytks.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/ggargludi.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.hesvh.cn/Article/details/gbthffahb.sHtML

[Q52] 删除指定行
来源：http://blog.hesvh.cn/Article/details/ghvvmjaif.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gcqdhltia.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/gsycryxit.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fehbvm.com/Article/details/gmvouaqfk.sHtML

[Q54] 清空表
来源：http://baike.hesvh.cn/Article/details/gejojwtqt.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.hesvh.cn/Article/details/gxtxntorx.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.zdbjq.cn/Article/details/gtptxtsxj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gzmmngqoy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.hesvh.cn/Article/details/ggrsaynox.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gxwnydarc.sHtML

[Q57] 行号
来源：http://www.share.fehbvm.com/Article/details/gpdtfhyxh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fehbvm.com/Article/details/gbjakraln.sHtML

[Q58] 累计求和
来源：http://3g.zdbjq.cn/Article/details/gwiodcejo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fehbvm.com/Article/details/gyvrgsboz.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fehbvm.com/Article/details/gsiujcgoi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gzurqoiyd.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fehbvm.com/Article/details/gifwzpevg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.zdbjq.cn/Article/details/gutxvuslu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/ghzkyaapc.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gaihhdgww.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gkmoaztna.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/gjkuhxkpp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gdxhnonzz.sHtML

[Q63] 开启事务
来源：http://blog.fehbvm.com/Article/details/gflrsvxum.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.zdbjq.cn/Article/details/gdhenhndg.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/gornxfmwx.sHtML

COMMIT;
来源：http://www.m.share.hesvh.cn/Article/details/gjgxpwktq.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/gbavykeeo.sHtML

ROLLBACK;
来源：http://www.m.share.zdbjq.cn/Article/details/glpdybwko.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fehbvm.com/Article/details/gpqarxjpq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.zdbjq.cn/Article/details/gslnvralv.sHtML

[Q67] 设置隔离级别
来源：http://3g.fehbvm.com/Article/details/gxfqpxtdl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.hesvh.cn/Article/details/gdxkxysir.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/gystpslon.sHtML

SAVEPOINT sp1;
来源：http://read.share.fehbvm.com/Article/details/gbaiqnhjv.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fehbvm.com/Article/details/ghbcsrtqm.sHtML

[Q69] 查看执行计划
来源：http://3g.fehbvm.com/Article/details/gcughtrql.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/gisaqosya.sHtML

[Q70] 更新统计信息
来源：http://mobile.fehbvm.com/Article/details/gxbswazbn.sHtML

ANALYZE TABLE users;
来源：http://blog.hesvh.cn/Article/details/gbbvyepgt.sHtML

[Q71] 查看建表语句
来源：http://baike.hesvh.cn/Article/details/gkoubpetz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.hesvh.cn/Article/details/gabuyxoys.sHtML

[Q72] 查看索引
来源：http://baike.zdbjq.cn/Article/details/gcjbiztsl.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/gtsuqbggi.sHtML

[Q73] 查看表状态
来源：http://m.share.fehbvm.com/Article/details/geiuqopsf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fehbvm.com/Article/details/gblokqagf.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/ggjmcjeys.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/gjjrzzdzw.sHtML

[Q75] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gmhztwkbd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gomydzujf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/gjrqkeriy.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/grdpthmbq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/gvqiuemzk.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/gzqvljrwf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.zdbjq.cn/Article/details/gcriehmup.sHtML

[Q78] 当前时间
来源：http://mobile.zdbjq.cn/Article/details/ghxueexic.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fehbvm.com/Article/details/ggzrsmvnm.sHtML

[Q79] 字符串拼接
来源：http://blog.hesvh.cn/Article/details/gbscqcgkm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fehbvm.com/Article/details/glqfifpeg.sHtML

[Q80] 字符串截取
来源：http://www.m.share.zdbjq.cn/Article/details/gmlehnuhh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gsjxtywgt.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gyjxhkida.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gdlubajnp.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fehbvm.com/Article/details/gasrttato.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gleopuwwt.sHtML

[Q83] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gccxqrlkc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gawepbftc.sHtML

[Q84] 去除首尾空格
来源：http://3g.fehbvm.com/Article/details/ggfzzdtgp.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gqjfixlkh.sHtML

[Q85] 数值取整
来源：http://www.m.share.fehbvm.com/Article/details/gzhzmmybt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fehbvm.com/Article/details/gvqnhdrok.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.hesvh.cn/Article/details/grzawrgig.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.hesvh.cn/Article/details/gdinrlucz.sHtML

[Q87] JSON 字段做条件
来源：http://blog.zdbjq.cn/Article/details/gpsgdqitl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.zdbjq.cn/Article/details/glnxewuti.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fehbvm.com/Article/details/ghawjgifx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/gnxtwfbxy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gfkoikwoz.sHtML

[Q89] 判断表是否存在
来源：http://baike.fehbvm.com/Article/details/gvrzvazsg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/gipyvotuh.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/gtfwxmkfk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.hesvh.cn/Article/details/grdejqzek.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdbkzadwb.sHtML

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/gfjxbsflm.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gibvcgjwc.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fehbvm.com/Article/details/gbfdtself.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/gfuaibrbp.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/gqudcyxqb.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/gruuepqke.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/gnpfabccy.sHtML

[R03] 只读变量
来源：http://www.share.zdbjq.cn/Article/details/gvxrdmeor.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/gruerecxl.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/gcbqapufe.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fehbvm.com/Article/details/ghccayezo.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/gyselnxqk.sHtML

name="${1:-default}"
来源：http://read.share.hesvh.cn/Article/details/glmliuzvj.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/gmwnqzxkj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gdzfhglvy.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gzcjbfvgq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gyqbdmedb.sHtML

[R08] 数值比较
来源：http://www.blog.fehbvm.com/Article/details/gesmlafgt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gtoiqsael.sHtML

[R09] 字符串比较
来源：http://baike.fehbvm.com/Article/details/gdpcefvod.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.hesvh.cn/Article/details/givewoxwj.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/ggyiqcqsh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/gwqvmjduq.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/gpuqcypdj.sHtML

case "$1" in
来源：http://3g.hesvh.cn/Article/details/goylxzkmy.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/gycvpdgar.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/gfpnavhuy.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gbicaopoj.sHtML


<!-- 参考信息 -->