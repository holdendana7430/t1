代发 wailian999

TS:   crypto.randomUUID()
来源：http://baike.fanxiaobao.xyz/Article/details/gcnegovoi.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fanxiaobao.xyz/Article/details/gjtzqjqnm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fanxiaobao.xyz/Article/details/ghifpahbl.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbcqdnre.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fanxiaobao.xyz/Article/details/gusewcjpi.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fanxiaobao.xyz/Article/details/ghkmwxruk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmpftgvf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxakxjfu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkoykued.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fanxiaobao.xyz/Article/details/gbrinhuvy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fanxiaobao.xyz/Article/details/gqczzzmby.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fanxiaobao.xyz/Article/details/gyamdfinn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggiwsaufj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fanxiaobao.xyz/Article/details/gbwrrjlfd.sHtML

[P03] 生成短随机字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gcgvrlmwv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fanxiaobao.xyz/Article/details/guwikhcqw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgwborcz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fanxiaobao.xyz/Article/details/gbdtjnfhw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdvquaqr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fanxiaobao.xyz/Article/details/gufubqnfk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fanxiaobao.xyz/Article/details/gxfbtlrxu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gryimxdvx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fanxiaobao.xyz/Article/details/gskwptarg.sHtML

[P04] 求长度
来源：http://blog.fanxiaobao.xyz/Article/details/gtonzedlb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fanxiaobao.xyz/Article/details/gekfpqero.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fanxiaobao.xyz/Article/details/gveyzaddc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fanxiaobao.xyz/Article/details/gqtjrxgge.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fanxiaobao.xyz/Article/details/gmofnnhnj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fanxiaobao.xyz/Article/details/gerdxowpn.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fanxiaobao.xyz/Article/details/gctzgwbhm.sHtML

Ruby: x.length;  x.size
来源：http://baike.fanxiaobao.xyz/Article/details/gkzmavxdg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwovtltvq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjlshlgd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gymffkpia.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fanxiaobao.xyz/Article/details/gakeywcsl.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fanxiaobao.xyz/Article/details/guswmcedy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzqvxpue.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fanxiaobao.xyz/Article/details/gtuqbohgi.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddgseqil.sHtML

Ruby: a == b
来源：http://wap.fanxiaobao.xyz/Article/details/gmzhlewsx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjcsmaza.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gipclhewe.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmaahixaa.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gycsavfcu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fanxiaobao.xyz/Article/details/gbumwufnz.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsacvwyq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/giadhxgze.sHtML

Go:   if x == nil {}
来源：http://3g.fanxiaobao.xyz/Article/details/gfloipuxc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffchzipo.sHtML

C#:   if (x is null) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/glggvbamf.sHtML

[P07] 防抖与节流
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsvnmvks.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fanxiaobao.xyz/Article/details/gihwoqmpv.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fanxiaobao.xyz/Article/details/gthhwmjvf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfroahulp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsjxnmbj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcttsqpk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.fanxiaobao.xyz/Article/details/gbcqthocw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fanxiaobao.xyz/Article/details/gibkanswk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdkvcgdy.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fanxiaobao.xyz/Article/details/guqacsymo.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybkugtag.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbdshivs.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpygkalh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gblnnfwoo.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fanxiaobao.xyz/Article/details/grlmymwvn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fanxiaobao.xyz/Article/details/gqquqckrv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxqnuoup.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fanxiaobao.xyz/Article/details/gklyrtsax.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gseuzoskz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fanxiaobao.xyz/Article/details/gbvtzqpck.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmugxplz.sHtML

[Q01] 创建表
来源：http://blog.fanxiaobao.xyz/Article/details/gimixafdf.sHtML

CREATE TABLE users (
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrrsykpv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fanxiaobao.xyz/Article/details/gpllomxax.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fanxiaobao.xyz/Article/details/gjzhuojyc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fanxiaobao.xyz/Article/details/gstpaacmb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fanxiaobao.xyz/Article/details/gawnaiyke.sHtML

);
来源：http://3g.fanxiaobao.xyz/Article/details/gtkwuuvra.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjiqoclu.sHtML

CREATE TABLE orders (
来源：http://www.share.fanxiaobao.xyz/Article/details/glwjdnjtg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fanxiaobao.xyz/Article/details/gfauopgms.sHtML

user_id INT NOT NULL,
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxsijgjg.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fanxiaobao.xyz/Article/details/gydowvkxr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzwlgjkb.sHtML

);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvagdrhgb.sHtML

[Q03] 增加列
来源：http://baike.fanxiaobao.xyz/Article/details/gqedwiqnv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gazeeiuhn.sHtML

[Q04] 修改列类型
来源：http://read.share.fanxiaobao.xyz/Article/details/glldhglde.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvcerlue.sHtML

[Q05] 重命名列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbhfykjx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fanxiaobao.xyz/Article/details/gzwnozytv.sHtML

[Q06] 删除列
来源：http://baike.fanxiaobao.xyz/Article/details/gscbpwsdz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fanxiaobao.xyz/Article/details/gaihkjobx.sHtML

[Q07] 删除表
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzyvziak.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkfdtfcp.sHtML

[Q08] 创建普通索引
来源：http://baike.fanxiaobao.xyz/Article/details/gszoxlrcn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtszvbunj.sHtML

[Q09] 创建唯一索引
来源：http://blog.fanxiaobao.xyz/Article/details/gazjcqdqu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxasqiwj.sHtML

[Q10] 插入单行
来源：http://3g.fanxiaobao.xyz/Article/details/gdyusyccq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gzkhljfwn.sHtML

[Q11] 一次插入多行
来源：http://www.share.fanxiaobao.xyz/Article/details/gyisxlvah.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/ggiyewwwz.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fanxiaobao.xyz/Article/details/gwokwxlnz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fanxiaobao.xyz/Article/details/gunyyyykt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fanxiaobao.xyz/Article/details/grxjsquci.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqomfbgp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/gtatkyose.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsjtmvwa.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fanxiaobao.xyz/Article/details/gefyyvubv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjntrsup.sHtML

[Q15] 查询全部
来源：http://baike.fanxiaobao.xyz/Article/details/gskkkpvaw.sHtML

SELECT * FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guigbhyoh.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlyaddqh.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmcucxbb.sHtML

[Q17] 条件查询
来源：http://wap.fanxiaobao.xyz/Article/details/gwvaptieb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpdsnppo.sHtML

[Q18] 模糊匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gekfgqjbk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fanxiaobao.xyz/Article/details/gynkwzefr.sHtML

[Q19] 范围查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtpiqvfc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdollxqez.sHtML

[Q20] IN 列表
来源：http://blog.fanxiaobao.xyz/Article/details/guuxkwhys.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fanxiaobao.xyz/Article/details/giflufejq.sHtML

[Q21] 空值判断
来源：http://blog.fanxiaobao.xyz/Article/details/gkcvzpcwz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fanxiaobao.xyz/Article/details/gejurnkfd.sHtML

[Q22] 排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gefhaplcs.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdtjtmuh.sHtML

[Q23] 分页
来源：http://baike.fanxiaobao.xyz/Article/details/gdxewbyvc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgpfpxpp.sHtML

[Q24] 去重
来源：http://wap.fanxiaobao.xyz/Article/details/gzqnxtkbr.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gagegaclu.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmfwikhx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fanxiaobao.xyz/Article/details/grxbdbqos.sHtML

[Q26] 计数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcerlwvcp.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gaynmxnzx.sHtML

[Q27] 条件计数
来源：http://wap.fanxiaobao.xyz/Article/details/gimtxanus.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gxsnybtfs.sHtML

[Q28] 求和与平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvymlfvh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxiuwreku.sHtML

[Q29] 最大最小值
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzvkehzm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gwyzxtvyf.sHtML

[Q30] 分组统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqelktutr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuuwalwq.sHtML

[Q31] 分组后过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gmzjcdwtl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllxneytz.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gjzhnkdgl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gqhtscdbz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fanxiaobao.xyz/Article/details/gcweynfuu.sHtML

[Q33] 多列分组
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjkfkixm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagmgunfc.sHtML

[Q34] 每组取第一条
来源：http://wap.fanxiaobao.xyz/Article/details/gbcewiczg.sHtML

SELECT * FROM (
来源：http://blog.fanxiaobao.xyz/Article/details/gxgjkrfig.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzrwluvk.sHtML

) t WHERE rn = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgddbpys.sHtML

[Q35] 内连接
来源：http://baike.fanxiaobao.xyz/Article/details/gsykcrkrp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gwblbhsjo.sHtML

[Q36] 左连接
来源：http://baike.fanxiaobao.xyz/Article/details/gxfwrepzx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwyzvijv.sHtML

[Q37] 右连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrjkigbb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsqogqrl.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fanxiaobao.xyz/Article/details/gmoptzsak.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqhicmhj.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fanxiaobao.xyz/Article/details/guisettvq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnncolwvk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbfdqceu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsqhmdts.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fanxiaobao.xyz/Article/details/gntdbviki.sHtML

[Q41] 多表连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwyfcohmv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fanxiaobao.xyz/Article/details/gfjrgqtkp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fanxiaobao.xyz/Article/details/gnumdqmgo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gaqswnvex.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gnsyjbjkk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwcmegod.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgtwmlbc.sHtML

[Q43] 标量子查询
来源：http://baike.fanxiaobao.xyz/Article/details/gxmyduate.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fanxiaobao.xyz/Article/details/gcitmmlby.sHtML

[Q44] IN 子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkkatsmc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fanxiaobao.xyz/Article/details/gybdanrzi.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtfxpeew.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzlxxmky.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzkejcff.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/gklexqcws.sHtML

[Q47] 与平均值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gvuonkasb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnudxufu.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/glketlwcy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnuetzjad.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjffysidi.sHtML

[Q49] 更新单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhvlnrlu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gujdsmtxk.sHtML

[Q50] 批量更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrmsiygh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxepmsyo.sHtML

[Q51] 用子查询更新
来源：http://baike.fanxiaobao.xyz/Article/details/grhvibguy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/ggdlovxpm.sHtML

[Q52] 删除指定行
来源：http://3g.fanxiaobao.xyz/Article/details/gjcmakkej.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehkuslqa.sHtML

[Q53] 按条件删除
来源：http://3g.fanxiaobao.xyz/Article/details/gjawnybdb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzotpuwr.sHtML

[Q54] 清空表
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqhunupl.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fanxiaobao.xyz/Article/details/gachmrpfu.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gyojcdurp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxuddtod.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gdjxgiqjk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gotratkov.sHtML

[Q57] 行号
来源：http://www.share.fanxiaobao.xyz/Article/details/ggksoufjy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gxhimfwdh.sHtML

[Q58] 累计求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giuanqdws.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/ghojapwsk.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/gyunikqii.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxykaebso.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fanxiaobao.xyz/Article/details/gesglncze.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fanxiaobao.xyz/Article/details/githseqfw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggyqlsion.sHtML

[Q61] 移动平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfcjzuch.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvemdllff.sHtML

[Q62] 分组占比
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmccnbzpn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/givraawib.sHtML

[Q63] 开启事务
来源：http://blog.fanxiaobao.xyz/Article/details/gqoyloyad.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fanxiaobao.xyz/Article/details/gozsycwlq.sHtML

[Q64] 提交事务
来源：http://wap.fanxiaobao.xyz/Article/details/ghitcvytd.sHtML

COMMIT;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpifcfgq.sHtML

[Q65] 回滚事务
来源：http://read.share.fanxiaobao.xyz/Article/details/grzdjgrsi.sHtML

ROLLBACK;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbuzfasl.sHtML

[Q66] 行锁查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gqldpnpxe.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrkcjhlq.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxeqogub.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fanxiaobao.xyz/Article/details/gqcvymmdg.sHtML

[Q68] 保存点
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxselxzd.sHtML

SAVEPOINT sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gacoiwber.sHtML

ROLLBACK TO sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gujpgdslc.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzwuyhtn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fanxiaobao.xyz/Article/details/gssxywimd.sHtML

[Q70] 更新统计信息
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjakhpnq.sHtML

ANALYZE TABLE users;
来源：http://mobile.fanxiaobao.xyz/Article/details/giqudaopv.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbtupmqk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fanxiaobao.xyz/Article/details/gehwoagfd.sHtML

[Q72] 查看索引
来源：http://wap.fanxiaobao.xyz/Article/details/gpdpzvkwu.sHtML

SHOW INDEX FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gjpipmaqv.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzyyjkxnr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/grlxlnged.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/gipfzsvut.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/gmshmnoii.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwhylrpb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gzdqqlcco.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgwkceoo.sHtML

[Q76] 按天统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrwsjzci.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fanxiaobao.xyz/Article/details/grcwkrxjj.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/gmggcwasr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvlhqdlp.sHtML

[Q78] 当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/gdnhwgepk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fanxiaobao.xyz/Article/details/grsealspv.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/glvmatqlv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljmxxcaf.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/gvkrwbksj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/getidjcts.sHtML

[Q81] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzpuqpwd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/girkmabog.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/gfxsyneuf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvguqoxy.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gvpuqihia.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gvolkghgm.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdltnkmw.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsiomwwz.sHtML

[Q85] 数值取整
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpumqzmz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbylcsueg.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/ggucoevei.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fanxiaobao.xyz/Article/details/gnodnbimr.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/gforqxnxy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/gclgjcjzd.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gwztjcfqh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgxueyla.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzfsygfx.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/golwkoenj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gcvpdxpfh.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gvqnwzjgi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhmcvlrh.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbuxgkhx.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gcxcidrqs.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifrdxbhu.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqxnzrot.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwiqcoazt.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqhwdfua.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxqitlta.sHtML

name="Tom"; echo "$name"
来源：http://wap.fanxiaobao.xyz/Article/details/ggujhphyb.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfxdyxeo.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gytggdavj.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gzvjzvlua.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkpjgmft.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gneqctgfi.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/grlsoyxuw.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gxcxtreyq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/giefxygrm.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjzueomu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/geuqyerxe.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpdnmvyq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gbhqeomjh.sHtML

[R09] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzqlypvp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/guxuwwqcg.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkbayoyo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gapodcits.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqwpwujx.sHtML


<!-- 参考信息 -->