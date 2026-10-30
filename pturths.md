代发 wailian999

[P01] 生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gwzmjzqzc.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/gjiwjrjoj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/gqpksomwy.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/giqgnwugx.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/glaczmfmr.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fehbvm.com/Article/details/gsuamcaqr.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/glbihuvjh.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/gltgubqky.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.zdbjq.cn/Article/details/guzbwanhm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fehbvm.com/Article/details/gnthvxmfo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.fehbvm.com/Article/details/gbwyfkgth.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.zdbjq.cn/Article/details/glmvyjieb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.zdbjq.cn/Article/details/gkokcwysr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.zdbjq.cn/Article/details/gewosnpma.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/gssofruxy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/gujvxrmwn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.hesvh.cn/Article/details/ggvvsuuaa.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fehbvm.com/Article/details/gjqzbnrlp.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/gezzeqyan.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.hesvh.cn/Article/details/geghxtzln.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fehbvm.com/Article/details/gduzawypn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gpriheoyx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/goizlhqdl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fehbvm.com/Article/details/grmsboxqk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/gkgqvlzed.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.zdbjq.cn/Article/details/gfwkwgfmp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.zdbjq.cn/Article/details/gtyrkypva.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/ggwrdmjat.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fehbvm.com/Article/details/gwocbdjbs.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gocrliamd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gsrupenzq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gswpyqhsm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fehbvm.com/Article/details/gyuambxjh.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/glxmpemuw.sHtML

Ruby: x.length;  x.size
来源：http://3g.fehbvm.com/Article/details/gxwccsktq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gciauzmou.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.hesvh.cn/Article/details/gftubzdyd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.zdbjq.cn/Article/details/gsgbftoct.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.zdbjq.cn/Article/details/gyflprqkk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.zdbjq.cn/Article/details/gdlbphdjw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gbunszxxf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/gwsvzsqap.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.fehbvm.com/Article/details/gcaovmdxa.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/gqbqtbfii.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/gggbyggrv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.zdbjq.cn/Article/details/gztiqwnlz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.zdbjq.cn/Article/details/gxtqpjzbh.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.hesvh.cn/Article/details/gfhspcxze.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.hesvh.cn/Article/details/gytjkkafo.sHtML

TS:   if (x == null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gbuyzynoi.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gdcftglsg.sHtML

Go:   if x == nil {}
来源：http://blog.hesvh.cn/Article/details/gqczuoqnq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.hesvh.cn/Article/details/gzuyiqupz.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gsvoxjtmd.sHtML

[P07] 防抖与节流
来源：http://www.m.share.zdbjq.cn/Article/details/gnemfrwzs.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fehbvm.com/Article/details/gukqeszva.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fehbvm.com/Article/details/gfxrekjar.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/grspcfjdt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gefakyknl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.hesvh.cn/Article/details/gfbdgtjjo.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/gwgdhazvx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fehbvm.com/Article/details/gqkpppllu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/gxxobvwcs.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fehbvm.com/Article/details/galgjkecq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fehbvm.com/Article/details/grjykjrzo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.zdbjq.cn/Article/details/geaeskynf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fehbvm.com/Article/details/gqjqtnftk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gwuornsen.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.zdbjq.cn/Article/details/gihyufdka.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.hesvh.cn/Article/details/galeffbxp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/gqslyibep.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fehbvm.com/Article/details/gzxgshfht.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gkqcqrjmn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.hesvh.cn/Article/details/gorqeyabs.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gyebpflqk.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/guascmjzq.sHtML

CREATE TABLE users (
来源：http://www.share.fehbvm.com/Article/details/gfnrdncag.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/ggpbzthsr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gwhmcollk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.zdbjq.cn/Article/details/gbltwhvca.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.hesvh.cn/Article/details/glkxuzrgi.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gggqpiurm.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fehbvm.com/Article/details/gqiayrrkd.sHtML

CREATE TABLE orders (
来源：http://wap.fehbvm.com/Article/details/gbvzjxxre.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gtzrbksgy.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gbzsjekca.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.hesvh.cn/Article/details/gbfnrzlxg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.zdbjq.cn/Article/details/gasmddagi.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/geugfghtq.sHtML

[Q03] 增加列
来源：http://3g.zdbjq.cn/Article/details/gvnqoqvfj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fehbvm.com/Article/details/gcrwnelgm.sHtML

[Q04] 修改列类型
来源：http://www.blog.zdbjq.cn/Article/details/gvybnksyq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.zdbjq.cn/Article/details/gcqjqvdln.sHtML

[Q05] 重命名列
来源：http://blog.hesvh.cn/Article/details/gmkpfyrvn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.hesvh.cn/Article/details/ggoygkyod.sHtML

[Q06] 删除列
来源：http://www.share.fehbvm.com/Article/details/gjeemgict.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.zdbjq.cn/Article/details/gdycbzvwu.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/gnuyrmttf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fehbvm.com/Article/details/ghrckpxvg.sHtML

[Q08] 创建普通索引
来源：http://3g.fehbvm.com/Article/details/gofhwkuzr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/guwbjpwss.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/gbvugrhxs.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gjpxmzfjy.sHtML

[Q10] 插入单行
来源：http://mobile.hesvh.cn/Article/details/gqknbjgnj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gulfggswm.sHtML

[Q11] 一次插入多行
来源：http://m.share.fehbvm.com/Article/details/gjnnontbe.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gyglguwiu.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.zdbjq.cn/Article/details/geiycdcoo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.hesvh.cn/Article/details/gifsdndrn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/gqkatspbk.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fehbvm.com/Article/details/gafxvjgvs.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gjffmwrqf.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/gylajbzul.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/gqnsjionl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.hesvh.cn/Article/details/gjohckvos.sHtML

[Q15] 查询全部
来源：http://www.share.zdbjq.cn/Article/details/gddigylhe.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/gufjpxwcz.sHtML

[Q16] 查询指定列
来源：http://mobile.hesvh.cn/Article/details/gnnntgqct.sHtML

SELECT id, name FROM users;
来源：http://blog.zdbjq.cn/Article/details/geskizhmx.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gvopckotf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.hesvh.cn/Article/details/gfromqcru.sHtML

[Q18] 模糊匹配
来源：http://baike.fehbvm.com/Article/details/gvirbaies.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.hesvh.cn/Article/details/gvtxhcxcj.sHtML

[Q19] 范围查询
来源：http://baike.hesvh.cn/Article/details/gyceiaslr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fehbvm.com/Article/details/gbgjhprqv.sHtML

[Q20] IN 列表
来源：http://wap.hesvh.cn/Article/details/gptwcmfye.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fehbvm.com/Article/details/gyujgoreu.sHtML

[Q21] 空值判断
来源：http://www.share.hesvh.cn/Article/details/gwtoipsms.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/geggfzlat.sHtML

[Q22] 排序
来源：http://m.share.hesvh.cn/Article/details/gtfuwnerk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fehbvm.com/Article/details/glkmrwegj.sHtML

[Q23] 分页
来源：http://www.share.hesvh.cn/Article/details/gyfysymiy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.hesvh.cn/Article/details/gskwtzhnd.sHtML

[Q24] 去重
来源：http://wap.hesvh.cn/Article/details/ghpcuidca.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gfjmvbsui.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/gkcgqfvbd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.hesvh.cn/Article/details/gdlehvumi.sHtML

[Q26] 计数
来源：http://mobile.hesvh.cn/Article/details/gxpiwtwiy.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fehbvm.com/Article/details/gzbxxsxet.sHtML

[Q27] 条件计数
来源：http://m.share.fehbvm.com/Article/details/gqujzfekn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.hesvh.cn/Article/details/gkbbciacl.sHtML

[Q28] 求和与平均
来源：http://baike.fehbvm.com/Article/details/gxkmgepsn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gvdwrawep.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fehbvm.com/Article/details/gjguefzhk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fehbvm.com/Article/details/gdslssgqo.sHtML

[Q30] 分组统计
来源：http://www.share.zdbjq.cn/Article/details/guisbrrjz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gsfdmwscq.sHtML

[Q31] 分组后过滤
来源：http://baike.fehbvm.com/Article/details/glvmushws.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fehbvm.com/Article/details/greojdkwo.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gcnonuhth.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gdbjqatow.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.zdbjq.cn/Article/details/gakqgczra.sHtML

[Q33] 多列分组
来源：http://3g.hesvh.cn/Article/details/gxiwihvcg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/glckswmfy.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fehbvm.com/Article/details/gehvzjved.sHtML

SELECT * FROM (
来源：http://3g.fehbvm.com/Article/details/goapnmtxf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/giqnascgn.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gxfcwfgep.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/gmfxmdgfx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gmkdxdsed.sHtML

[Q36] 左连接
来源：http://wap.fehbvm.com/Article/details/gupjmcngm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gdgsxeqnn.sHtML

[Q37] 右连接
来源：http://blog.zdbjq.cn/Article/details/ghlgsmrij.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.hesvh.cn/Article/details/ggaagvdoi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.hesvh.cn/Article/details/gluyzfqgq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/grxotczyu.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/gkmquaxgo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/gnzrgdqiu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/ghfdwnyap.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.hesvh.cn/Article/details/gbrjhqeuz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.zdbjq.cn/Article/details/gdyamrhly.sHtML

[Q41] 多表连接
来源：http://www.blog.fehbvm.com/Article/details/gtojnobdf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/gjpkegred.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/geahzufmv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gmnoiriax.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fehbvm.com/Article/details/gcaxiolnx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fehbvm.com/Article/details/gjijejbwb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fehbvm.com/Article/details/ggicnoaem.sHtML

[Q43] 标量子查询
来源：http://blog.zdbjq.cn/Article/details/gybuglcxm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.hesvh.cn/Article/details/gerohmitl.sHtML

[Q44] IN 子查询
来源：http://www.share.hesvh.cn/Article/details/gigkxduvi.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fehbvm.com/Article/details/ghigyjvrk.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fehbvm.com/Article/details/gouycacma.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gxokxrgfx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fehbvm.com/Article/details/gygmtkdwl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/giiryjqey.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/goqwczrdp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fehbvm.com/Article/details/gstvbwgrr.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.zdbjq.cn/Article/details/gwriorknx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/gfaclasjl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.zdbjq.cn/Article/details/gdznectcg.sHtML

[Q49] 更新单行
来源：http://www.m.share.zdbjq.cn/Article/details/gdpnlbtpz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gmsppkqjm.sHtML

[Q50] 批量更新
来源：http://wap.hesvh.cn/Article/details/gyurenzlq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gfuxkbxvv.sHtML

[Q51] 用子查询更新
来源：http://3g.fehbvm.com/Article/details/gqxwezorb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.hesvh.cn/Article/details/gfyariybm.sHtML

[Q52] 删除指定行
来源：http://read.share.fehbvm.com/Article/details/gibaavgqi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gaeavonyb.sHtML

[Q53] 按条件删除
来源：http://www.blog.hesvh.cn/Article/details/gieknfbto.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/ghfmbtrak.sHtML

[Q54] 清空表
来源：http://www.m.share.hesvh.cn/Article/details/gvttxvkby.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.zdbjq.cn/Article/details/gnwdwvned.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gytfhbnbq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gojnnwofk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.hesvh.cn/Article/details/gtbeexszn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.hesvh.cn/Article/details/goeyfcjbc.sHtML

[Q57] 行号
来源：http://www.m.share.fehbvm.com/Article/details/gyjwbzltg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gyuvdmkee.sHtML

[Q58] 累计求和
来源：http://www.share.hesvh.cn/Article/details/gpebjhapw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gffdfusez.sHtML

[Q59] 分组内累计
来源：http://baike.hesvh.cn/Article/details/grbgiesyo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gthqybhej.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.hesvh.cn/Article/details/gibbtsqxl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fehbvm.com/Article/details/gnrrflkch.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gxmwmiuha.sHtML

[Q61] 移动平均
来源：http://blog.fehbvm.com/Article/details/gotxgjjgy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gmyhcuziy.sHtML

[Q62] 分组占比
来源：http://read.share.fehbvm.com/Article/details/gvdulveyf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gsyjfnpwt.sHtML

[Q63] 开启事务
来源：http://wap.zdbjq.cn/Article/details/goldaybcx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.zdbjq.cn/Article/details/gegvyugvf.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/gjogfdhoe.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/gisuhwmjf.sHtML

[Q65] 回滚事务
来源：http://www.share.zdbjq.cn/Article/details/gitqsnswo.sHtML

ROLLBACK;
来源：http://www.share.hesvh.cn/Article/details/gdeeieimg.sHtML

[Q66] 行锁查询
来源：http://read.share.fehbvm.com/Article/details/grcsznxeb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.hesvh.cn/Article/details/ggujsjlvk.sHtML

[Q67] 设置隔离级别
来源：http://wap.fehbvm.com/Article/details/guzbpwbwm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/giwcsqgby.sHtML

[Q68] 保存点
来源：http://blog.zdbjq.cn/Article/details/gjagbsyfo.sHtML

SAVEPOINT sp1;
来源：http://wap.hesvh.cn/Article/details/gdpekvjti.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fehbvm.com/Article/details/gjgetupva.sHtML

[Q69] 查看执行计划
来源：http://wap.zdbjq.cn/Article/details/getekpzti.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fehbvm.com/Article/details/gzpvqnehw.sHtML

[Q70] 更新统计信息
来源：http://baike.fehbvm.com/Article/details/gwhxcyogk.sHtML

ANALYZE TABLE users;
来源：http://baike.fehbvm.com/Article/details/gjajufdyw.sHtML

[Q71] 查看建表语句
来源：http://wap.zdbjq.cn/Article/details/grwqpvtep.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/gemqgrwkq.sHtML

[Q72] 查看索引
来源：http://read.share.hesvh.cn/Article/details/glpsseglq.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/gvofiymub.sHtML

[Q73] 查看表状态
来源：http://read.share.zdbjq.cn/Article/details/gqlfihact.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fehbvm.com/Article/details/goavyjvjb.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/gsaxaibqe.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fehbvm.com/Article/details/gkyozjwnf.sHtML

[Q75] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gnkihghgj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fehbvm.com/Article/details/gkwdzdzzg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fehbvm.com/Article/details/gpmibnyca.sHtML

[Q76] 按天统计
来源：http://www.share.fehbvm.com/Article/details/grlgpmltg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/gdofhfjkg.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/gxvxpjpki.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/ggnzqwvqz.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gksallwqy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.hesvh.cn/Article/details/gvqrndwyi.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gdwifgrpj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.hesvh.cn/Article/details/grswzmaje.sHtML

[Q80] 字符串截取
来源：http://www.blog.zdbjq.cn/Article/details/gyvznfeia.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/glhpgxqqv.sHtML

[Q81] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gkdxxnejf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ggnpupetc.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gvcmghhgb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gcqstvine.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/geuohvdji.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gsebtuyse.sHtML

[Q84] 去除首尾空格
来源：http://wap.hesvh.cn/Article/details/gtlcpjoed.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gsuwjplty.sHtML

[Q85] 数值取整
来源：http://www.m.share.fehbvm.com/Article/details/gzffbuequ.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/gkoexqbfo.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.zdbjq.cn/Article/details/gzoanuiey.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/gxmbcnjee.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/ghheqawki.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/guoxwlayq.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/gkvkxiwcz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.zdbjq.cn/Article/details/grozgqujh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/gvctwnufq.sHtML

[Q89] 判断表是否存在
来源：http://3g.hesvh.cn/Article/details/gwrlomkyh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/gftwhbaew.sHtML

[Q90] 生成序号列
来源：http://wap.zdbjq.cn/Article/details/gidzriwmp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fehbvm.com/Article/details/goiiacolg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbecwodkj.sHtML

R. Bash 专题
来源：http://www.m.share.fehbvm.com/Article/details/gynfobmjn.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glbzblznj.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/gtypsbvcn.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/gxpequjmj.sHtML

set -euo pipefail
来源：http://3g.fehbvm.com/Article/details/gholcwxjf.sHtML

[R02] 变量赋值与使用
来源：http://m.share.zdbjq.cn/Article/details/gfojvymou.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/gqwcjrskq.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/gkuarjsjv.sHtML

readonly PI=3.14
来源：http://wap.hesvh.cn/Article/details/grsjnlwlg.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/gxqapwmju.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.hesvh.cn/Article/details/gmpvzbtiv.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/guxreoikf.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gmujqbzyi.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/guvvofrrc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gihqeefhg.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/guatedtuq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/gixyjusdb.sHtML

[R08] 数值比较
来源：http://m.share.hesvh.cn/Article/details/gdarmfahi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.zdbjq.cn/Article/details/gltjuniht.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gbptchpla.sHtML


<!-- 参考信息 -->