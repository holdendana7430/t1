代发 wailian999

[P01] 生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gahrftfkb.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/gtnlxfhjy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gzyezfkeo.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gwtsxdero.sHtML

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gbkmxogqd.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.hesvh.cn/Article/details/gvfbiqlnt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.hesvh.cn/Article/details/gnhkhhbub.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.zdbjq.cn/Article/details/galwspegf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.zdbjq.cn/Article/details/gqwjicttc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/gvdsfosyi.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.hesvh.cn/Article/details/gicuemjiu.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/gwkfhhiuz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gfcuzaxzd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.zdbjq.cn/Article/details/gjdkrblxr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gwxkqwgvy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/gviprsvyn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/gauqbjbft.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/grlxcyats.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gjjskvqxa.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fehbvm.com/Article/details/gzkrlojug.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fehbvm.com/Article/details/gofgnejgm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gnwbnwlor.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gxahwakmj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.zdbjq.cn/Article/details/gxomydnqh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fehbvm.com/Article/details/grxjrqfsi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fehbvm.com/Article/details/gzwyizuuk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.zdbjq.cn/Article/details/guhocviok.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/gxseggqxr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fehbvm.com/Article/details/gnjyoqxcx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gcpacpmgn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gyztbevqx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gmzamxsih.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fehbvm.com/Article/details/glvecwwtv.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fehbvm.com/Article/details/gvqsviqog.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/goeetrevo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/gwngdvmqk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fehbvm.com/Article/details/gvmzsjkrw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.zdbjq.cn/Article/details/gyaytxkwe.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.hesvh.cn/Article/details/gezemgall.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.zdbjq.cn/Article/details/gagokuuij.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gikqienea.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.fehbvm.com/Article/details/gaiwfkhij.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/gqxmvpowh.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/gquduaciz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fehbvm.com/Article/details/gnqsepyui.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/gbttexeos.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fehbvm.com/Article/details/ganhojczl.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.hesvh.cn/Article/details/glajhimjl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fehbvm.com/Article/details/gzzugdkoq.sHtML

TS:   if (x == null) {}
来源：http://m.share.zdbjq.cn/Article/details/gbfehjldn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/ggvoldnrw.sHtML

Go:   if x == nil {}
来源：http://www.share.zdbjq.cn/Article/details/gplnmpjgk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.zdbjq.cn/Article/details/gtsgalvdt.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/gewhhthdc.sHtML

[P07] 防抖与节流
来源：http://www.m.share.hesvh.cn/Article/details/gfegtwvue.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/gaveemaxl.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.fehbvm.com/Article/details/gptccdjpf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gjgtcrerg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gmptqigcy.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fehbvm.com/Article/details/gqinjoryk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.hesvh.cn/Article/details/gjkqynjhl.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.hesvh.cn/Article/details/gubsytjyy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/gjzwywovj.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/gtuqtdola.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fehbvm.com/Article/details/gqiocnrqh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fehbvm.com/Article/details/gxpfnfmbi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/gqplememn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/gzjzuivme.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.zdbjq.cn/Article/details/gqtjywpvl.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.hesvh.cn/Article/details/gjxoeosjz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fehbvm.com/Article/details/gbiflxiwc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/geppqijtu.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glwanxrop.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.hesvh.cn/Article/details/goxzxidvp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gumpajnyv.sHtML

[Q01] 创建表
来源：http://www.share.fehbvm.com/Article/details/gynxxdxvh.sHtML

CREATE TABLE users (
来源：http://mobile.zdbjq.cn/Article/details/gnrkymvnw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gqpbvfhhd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gpncdgawv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.zdbjq.cn/Article/details/giukjmqqi.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.hesvh.cn/Article/details/gzewaamcc.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gjzpzfhjb.sHtML

[Q02] 创建带外键的表
来源：http://baike.hesvh.cn/Article/details/gdviblzcm.sHtML

CREATE TABLE orders (
来源：http://m.share.fehbvm.com/Article/details/giibsiekc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/giwotdrxi.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gdhkczpbd.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.hesvh.cn/Article/details/gnsovglrs.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.hesvh.cn/Article/details/gvbtkvoyh.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gnwufzcip.sHtML

[Q03] 增加列
来源：http://www.share.hesvh.cn/Article/details/gzaamorjc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.zdbjq.cn/Article/details/gmibeayig.sHtML

[Q04] 修改列类型
来源：http://www.blog.fehbvm.com/Article/details/gryyovjfo.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.hesvh.cn/Article/details/gceeqgsxa.sHtML

[Q05] 重命名列
来源：http://www.blog.fehbvm.com/Article/details/gddzvshnq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.zdbjq.cn/Article/details/gfjwmlsaw.sHtML

[Q06] 删除列
来源：http://www.blog.fehbvm.com/Article/details/gwnsovhlb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fehbvm.com/Article/details/gmxydrueb.sHtML

[Q07] 删除表
来源：http://www.blog.zdbjq.cn/Article/details/gtevlrrsi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.hesvh.cn/Article/details/gmuikojep.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/gbiwxaatg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gyeprmkxz.sHtML

[Q09] 创建唯一索引
来源：http://m.share.zdbjq.cn/Article/details/guklaqewk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gutautosk.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/gqxlmmdut.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fehbvm.com/Article/details/gwrxfovmj.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/giidcrlus.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gvynkyvwa.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.zdbjq.cn/Article/details/gjdkyzolj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.hesvh.cn/Article/details/gyfbgwkry.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/gysfvjqil.sHtML

[Q13] 忽略重复插入
来源：http://m.share.zdbjq.cn/Article/details/gsdbqzyou.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fehbvm.com/Article/details/grvgioilo.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.zdbjq.cn/Article/details/gpvagavio.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.hesvh.cn/Article/details/gyolwcjid.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.zdbjq.cn/Article/details/gxdttrguo.sHtML

[Q15] 查询全部
来源：http://www.m.share.zdbjq.cn/Article/details/gmkmgndzo.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gfzcuyhru.sHtML

[Q16] 查询指定列
来源：http://blog.zdbjq.cn/Article/details/gbxiefvem.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gcbeikznb.sHtML

[Q17] 条件查询
来源：http://m.share.fehbvm.com/Article/details/gcynzgggm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fehbvm.com/Article/details/guifqmvfh.sHtML

[Q18] 模糊匹配
来源：http://wap.zdbjq.cn/Article/details/gqtttczco.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/gtolrvuub.sHtML

[Q19] 范围查询
来源：http://www.m.share.fehbvm.com/Article/details/gldrrehft.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/gwxmgqwcf.sHtML

[Q20] IN 列表
来源：http://read.share.hesvh.cn/Article/details/gxrdimdpt.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fehbvm.com/Article/details/gwjlbobac.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/gqkkyvoad.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.hesvh.cn/Article/details/gwtnytckk.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/ggzyriepa.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.zdbjq.cn/Article/details/gmnaupxfs.sHtML

[Q23] 分页
来源：http://blog.hesvh.cn/Article/details/gxaplibih.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/gubfzhxac.sHtML

[Q24] 去重
来源：http://www.blog.hesvh.cn/Article/details/gynbedljo.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.hesvh.cn/Article/details/gaipsnrrn.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fehbvm.com/Article/details/gmnxfpajd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.zdbjq.cn/Article/details/gfuktviyc.sHtML

[Q26] 计数
来源：http://mobile.fehbvm.com/Article/details/gicbbiyxh.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gudmpjosd.sHtML

[Q27] 条件计数
来源：http://blog.hesvh.cn/Article/details/guesxdrnp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gkrarwrqy.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/gbxvzwnzh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gjgrezjei.sHtML

[Q29] 最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/gorbgkiwd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/glrvjyoah.sHtML

[Q30] 分组统计
来源：http://3g.fehbvm.com/Article/details/gaggripnl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gyfjpzuys.sHtML

[Q31] 分组后过滤
来源：http://m.share.zdbjq.cn/Article/details/ghypxligp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.zdbjq.cn/Article/details/gwmbdoscb.sHtML

[Q32] 分组拼接字符串
来源：http://wap.zdbjq.cn/Article/details/ggtmfzmcm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gqftfxgfc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/gqlosoqon.sHtML

[Q33] 多列分组
来源：http://wap.hesvh.cn/Article/details/gjlnvvgyd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/gvddfvals.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/gdipmmgzj.sHtML

SELECT * FROM (
来源：http://www.share.zdbjq.cn/Article/details/gknjpqzvd.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fehbvm.com/Article/details/gqafeqyex.sHtML

) t WHERE rn = 1;
来源：http://mobile.fehbvm.com/Article/details/glpgzzjcn.sHtML

[Q35] 内连接
来源：http://read.share.hesvh.cn/Article/details/grwpxfase.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gvbivbonj.sHtML

[Q36] 左连接
来源：http://m.share.hesvh.cn/Article/details/gltxuenzp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gmwwgglpw.sHtML

[Q37] 右连接
来源：http://3g.fehbvm.com/Article/details/gxuzkbjqu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/goztwngpy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.zdbjq.cn/Article/details/gcqrpqlqm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fehbvm.com/Article/details/gablwahge.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fehbvm.com/Article/details/gwldgixfn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/gaqqowvpp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fehbvm.com/Article/details/gyrylclvp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/gzbsdizby.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.zdbjq.cn/Article/details/gfiseaduy.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/gebviuuud.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.hesvh.cn/Article/details/gyuzxsgor.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/ggbfxhwkx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fehbvm.com/Article/details/gtdrjeyzc.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.zdbjq.cn/Article/details/gksenkggb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/gkwuxfjem.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fehbvm.com/Article/details/gpziaobyd.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/gizseuimr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/gazxahehk.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/ggzddcpbo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/gavhozsrl.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fehbvm.com/Article/details/gcwpldfao.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gxtpnoggu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.zdbjq.cn/Article/details/gittteaiz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gbvvygigc.sHtML

[Q47] 与平均值比较
来源：http://mobile.hesvh.cn/Article/details/grgorfbbu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.zdbjq.cn/Article/details/gtjdpcvqc.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.hesvh.cn/Article/details/ghniwtfkr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fehbvm.com/Article/details/gjijmnaae.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gxbagioeu.sHtML

[Q49] 更新单行
来源：http://wap.fehbvm.com/Article/details/gmytkyjyx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/ghtcavgoh.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/gpiwasugi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.hesvh.cn/Article/details/gfzuccxlu.sHtML

[Q51] 用子查询更新
来源：http://wap.hesvh.cn/Article/details/gaegohscy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fehbvm.com/Article/details/gikkaeqwq.sHtML

[Q52] 删除指定行
来源：http://read.share.hesvh.cn/Article/details/gkbppxxcr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gyfsybkiy.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/gdwwpunhk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fehbvm.com/Article/details/gieyrwxxk.sHtML

[Q54] 清空表
来源：http://mobile.hesvh.cn/Article/details/gpnsnzqhj.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fehbvm.com/Article/details/grfqvweto.sHtML

[Q55] 排名（并列占位）
来源：http://wap.zdbjq.cn/Article/details/gpjipugvz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gbcphfhnk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.zdbjq.cn/Article/details/gtpnkukrg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gxxmtqxpa.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/gwfectyqv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gindkhuvm.sHtML

[Q58] 累计求和
来源：http://read.share.zdbjq.cn/Article/details/gowoonogb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gpfbjylrp.sHtML

[Q59] 分组内累计
来源：http://baike.hesvh.cn/Article/details/giqzefwkw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gtwggrnkq.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.zdbjq.cn/Article/details/gegjnnyii.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fehbvm.com/Article/details/gszxqpjbu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/gwkizxflb.sHtML

[Q61] 移动平均
来源：http://m.share.hesvh.cn/Article/details/ghqdsdgne.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gmjetfjvx.sHtML

[Q62] 分组占比
来源：http://blog.zdbjq.cn/Article/details/ggfiwryzy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gctidnmru.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/gxamjwskq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fehbvm.com/Article/details/gniunphcb.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/gghtlnsiw.sHtML

COMMIT;
来源：http://wap.fehbvm.com/Article/details/grkgzegpp.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/ghmlkwvby.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/gcmtjyxyi.sHtML

[Q66] 行锁查询
来源：http://3g.fehbvm.com/Article/details/gddbgrfyo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.zdbjq.cn/Article/details/gwyxvraht.sHtML

[Q67] 设置隔离级别
来源：http://www.share.hesvh.cn/Article/details/gcnksjwrv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fehbvm.com/Article/details/gezlioofr.sHtML

[Q68] 保存点
来源：http://wap.fehbvm.com/Article/details/gpkpuncup.sHtML

SAVEPOINT sp1;
来源：http://www.share.hesvh.cn/Article/details/gpyszrizx.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/gkwigewgh.sHtML

[Q69] 查看执行计划
来源：http://3g.fehbvm.com/Article/details/ganregzwq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.zdbjq.cn/Article/details/ghkzsavog.sHtML

[Q70] 更新统计信息
来源：http://wap.fehbvm.com/Article/details/gsznzmjii.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/gxutrzkfk.sHtML

[Q71] 查看建表语句
来源：http://mobile.hesvh.cn/Article/details/gfmmmbgua.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/gujqgbkts.sHtML

[Q72] 查看索引
来源：http://3g.hesvh.cn/Article/details/gnxpupxlj.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gywzttmcr.sHtML

[Q73] 查看表状态
来源：http://m.share.zdbjq.cn/Article/details/gzjkwgvai.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.zdbjq.cn/Article/details/ghrxrwzbh.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/gftghsfke.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/gvplqhpan.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gvizfpxwc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gmdkykmzk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fehbvm.com/Article/details/gsysuztzw.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/gkhbpuprs.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.zdbjq.cn/Article/details/gmfpzwzbc.sHtML

[Q77] 时间加减
来源：http://3g.zdbjq.cn/Article/details/gdxzjmsdq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/gahpefknw.sHtML

[Q78] 当前时间
来源：http://m.share.zdbjq.cn/Article/details/gbyozkkxg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fehbvm.com/Article/details/gauzirprv.sHtML

[Q79] 字符串拼接
来源：http://wap.hesvh.cn/Article/details/gxbllrjtd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fehbvm.com/Article/details/gqtdujmxt.sHtML

[Q80] 字符串截取
来源：http://mobile.fehbvm.com/Article/details/gdmfpexxb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gohmxjryt.sHtML

[Q81] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gczljkcfs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.hesvh.cn/Article/details/gjuaknxek.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gjrjwbzrf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/goaihpcgl.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gcqcjrsdx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gjdbhxxlm.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gkvvnnbto.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/ghcshadwf.sHtML

[Q85] 数值取整
来源：http://mobile.fehbvm.com/Article/details/ghvrlkqqn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.hesvh.cn/Article/details/gznzrzgtq.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.zdbjq.cn/Article/details/gabnfnsit.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.zdbjq.cn/Article/details/gcllmoaya.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.hesvh.cn/Article/details/gyhxokned.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/gyrvoxsfl.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fehbvm.com/Article/details/gxlkbncke.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.zdbjq.cn/Article/details/gpqstpsyq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gvhzeghxi.sHtML

[Q89] 判断表是否存在
来源：http://blog.fehbvm.com/Article/details/gyxlxikit.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fehbvm.com/Article/details/gosaeaxpx.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gacuiqpft.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/glhbztzds.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/getffetcu.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/gkxlgrsba.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gojwqzvvb.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/gomgkpcgh.sHtML

#!/usr/bin/env bash
来源：http://3g.zdbjq.cn/Article/details/gpmfuosur.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gzqwrbsdd.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/gkcvwkiym.sHtML

name="Tom"; echo "$name"
来源：http://baike.hesvh.cn/Article/details/gggqncubh.sHtML

[R03] 只读变量
来源：http://www.blog.fehbvm.com/Article/details/gkkafahtw.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/gtqzbzyua.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/gogdztslc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/gicupbllw.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gnapsuoxo.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/gparvture.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gkpjhsphe.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gwpjllptr.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/grttccdbm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/gudlqcofm.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/gyvqmfqcg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.hesvh.cn/Article/details/gvhqobksj.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/gkgxluctp.sHtML


<!-- 参考信息 -->