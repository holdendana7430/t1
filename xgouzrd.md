代发 wailian999

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gdbexdcjx.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gwpcmwgij.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gyfqyfrnb.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.hesvh.cn/Article/details/glyziduev.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.hesvh.cn/Article/details/gwypnyldm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.zdbjq.cn/Article/details/gshkjhswd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.zdbjq.cn/Article/details/ggcbwwegj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.zdbjq.cn/Article/details/gcgyjlckx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.hesvh.cn/Article/details/gppezpdue.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/glvppyfzd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fehbvm.com/Article/details/grqwwtdjw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.zdbjq.cn/Article/details/gcumhfqll.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/gkdqncjoa.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/gheuduhdh.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/gwynwweox.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/gqfdlitbt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.hesvh.cn/Article/details/gxzrncifo.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gueldvntw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gpbgljbpe.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.zdbjq.cn/Article/details/gkdjhqond.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fehbvm.com/Article/details/gerectpxb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.hesvh.cn/Article/details/gkysteqxl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.hesvh.cn/Article/details/gmbfwhhyd.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/gdzqoqukh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fehbvm.com/Article/details/gazawrhph.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gkogwubzw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gzpqxekfn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gvpwesmlp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/giowjfhoe.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.zdbjq.cn/Article/details/gffshlqbd.sHtML

Ruby: x.length;  x.size
来源：http://blog.hesvh.cn/Article/details/gbyclpxlu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/gwegdfred.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fehbvm.com/Article/details/gufeureyv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/geghuhqol.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.zdbjq.cn/Article/details/grsfeqjgp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.zdbjq.cn/Article/details/gdototnjc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gnmlxvqca.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/grudocbtd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gszfvrkdc.sHtML

Ruby: a == b
来源：http://wap.hesvh.cn/Article/details/gavwlgosi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.hesvh.cn/Article/details/gsusencol.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.hesvh.cn/Article/details/gusdmkbzk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/gnkvqbmle.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fehbvm.com/Article/details/geeorbpwd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.zdbjq.cn/Article/details/gsbmcnbzh.sHtML

TS:   if (x == null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gcrcqgoew.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gkepvduqj.sHtML

Go:   if x == nil {}
来源：http://www.blog.fehbvm.com/Article/details/gahexkgza.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.zdbjq.cn/Article/details/ghshggwrf.sHtML

C#:   if (x is null) {}
来源：http://baike.fehbvm.com/Article/details/gydzqokgo.sHtML

[P07] 防抖与节流
来源：http://mobile.hesvh.cn/Article/details/guhltwtmc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/goqomjkob.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.zdbjq.cn/Article/details/gtldmzwan.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/glnepeiya.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/glvdytzxw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fehbvm.com/Article/details/gaetmahij.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fehbvm.com/Article/details/gncgsoikj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fehbvm.com/Article/details/gbvcyrgyn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/gqrfqzqau.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/gjdijqktq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.zdbjq.cn/Article/details/gdmkytcil.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/gpsqvimcz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fehbvm.com/Article/details/gvhvjpbvx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/gwbeltqov.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.hesvh.cn/Article/details/gfzxohyaa.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.hesvh.cn/Article/details/gmgenneec.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fehbvm.com/Article/details/girpwtngc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/grofitogn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/giywyluvq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/gqhkyvbuj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gpflbqblz.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/gigwlpwtw.sHtML

CREATE TABLE users (
来源：http://baike.hesvh.cn/Article/details/gntnwidbt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gjbdovqna.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gpgamqzie.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/gqmprtnrq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/gfhtdbqkp.sHtML

);
来源：http://wap.hesvh.cn/Article/details/goxjbiulu.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fehbvm.com/Article/details/gnqifjmsw.sHtML

CREATE TABLE orders (
来源：http://www.blog.fehbvm.com/Article/details/gduasfnag.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gtxrynamd.sHtML

user_id INT NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gwbzdhbvc.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.zdbjq.cn/Article/details/gdvtflkfu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.hesvh.cn/Article/details/gopnegdgz.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gpywvedwx.sHtML

[Q03] 增加列
来源：http://3g.zdbjq.cn/Article/details/gmpanrbeg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.hesvh.cn/Article/details/gtjwkuusa.sHtML

[Q04] 修改列类型
来源：http://www.blog.fehbvm.com/Article/details/gadfvurai.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.hesvh.cn/Article/details/gehfsrike.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/grxwdklmp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fehbvm.com/Article/details/goeazhyti.sHtML

[Q06] 删除列
来源：http://blog.fehbvm.com/Article/details/gtbudxymt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.hesvh.cn/Article/details/gsovbtemw.sHtML

[Q07] 删除表
来源：http://www.blog.zdbjq.cn/Article/details/gjzqlfczp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.zdbjq.cn/Article/details/guoxqoaya.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/gpejuqruk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gejbkccql.sHtML

[Q09] 创建唯一索引
来源：http://wap.fehbvm.com/Article/details/ghuefxgcs.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gaeknugjo.sHtML

[Q10] 插入单行
来源：http://m.share.fehbvm.com/Article/details/gtxtkfpzi.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.hesvh.cn/Article/details/ggchkvxiy.sHtML

[Q11] 一次插入多行
来源：http://www.share.fehbvm.com/Article/details/gbdbuaqrd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gmstfwbyn.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fehbvm.com/Article/details/gqvnvzfyc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fehbvm.com/Article/details/gtformkpx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fehbvm.com/Article/details/gwvpzugcx.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.zdbjq.cn/Article/details/glvllrtzs.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.hesvh.cn/Article/details/ggnekemnw.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/gftxxfpkq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.zdbjq.cn/Article/details/gggwvuuxi.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.hesvh.cn/Article/details/gdicfwytl.sHtML

[Q15] 查询全部
来源：http://blog.hesvh.cn/Article/details/gwpwirxbh.sHtML

SELECT * FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gurqinsla.sHtML

[Q16] 查询指定列
来源：http://wap.fehbvm.com/Article/details/gscgtbzgc.sHtML

SELECT id, name FROM users;
来源：http://www.blog.hesvh.cn/Article/details/goocrnjdo.sHtML

[Q17] 条件查询
来源：http://www.blog.hesvh.cn/Article/details/gqbpzaxqw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.hesvh.cn/Article/details/gerrsjzej.sHtML

[Q18] 模糊匹配
来源：http://blog.fehbvm.com/Article/details/gwcuvxumn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/gbxjhdnyy.sHtML

[Q19] 范围查询
来源：http://m.share.hesvh.cn/Article/details/gywrqbxaa.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.hesvh.cn/Article/details/gciojksay.sHtML

[Q20] IN 列表
来源：http://www.m.share.fehbvm.com/Article/details/gogzxrlvn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fehbvm.com/Article/details/gabnbvxqt.sHtML

[Q21] 空值判断
来源：http://www.share.fehbvm.com/Article/details/gdyfacibg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/gfxwnkzrx.sHtML

[Q22] 排序
来源：http://www.blog.zdbjq.cn/Article/details/gzzfcamle.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fehbvm.com/Article/details/grttwrvlx.sHtML

[Q23] 分页
来源：http://www.share.hesvh.cn/Article/details/gyfivtlmc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/gulgrjbfx.sHtML

[Q24] 去重
来源：http://m.share.hesvh.cn/Article/details/gcgsbjjnw.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gxmnejoxl.sHtML

[Q25] 只取前 N 条
来源：http://baike.zdbjq.cn/Article/details/gfubbuxxm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fehbvm.com/Article/details/gqfvnieza.sHtML

[Q26] 计数
来源：http://www.blog.hesvh.cn/Article/details/gnrdfixws.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.zdbjq.cn/Article/details/guutrbqma.sHtML

[Q27] 条件计数
来源：http://3g.hesvh.cn/Article/details/gxidmrvfc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.hesvh.cn/Article/details/gscbbvklc.sHtML

[Q28] 求和与平均
来源：http://wap.fehbvm.com/Article/details/gabydlzdh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fehbvm.com/Article/details/guxtvdtld.sHtML

[Q29] 最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gtckjldgx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gbwaokmwn.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/gokaivlch.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gedisbbzp.sHtML

[Q31] 分组后过滤
来源：http://m.share.hesvh.cn/Article/details/grpdutyof.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/gaqvlzufs.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gmgxoesdh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gacfvcifh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.zdbjq.cn/Article/details/grohfblst.sHtML

[Q33] 多列分组
来源：http://www.m.share.hesvh.cn/Article/details/gwwmqxrcj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.hesvh.cn/Article/details/gdhvlazor.sHtML

[Q34] 每组取第一条
来源：http://mobile.fehbvm.com/Article/details/gcxbfamul.sHtML

SELECT * FROM (
来源：http://blog.hesvh.cn/Article/details/grerzoqch.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.hesvh.cn/Article/details/gtvqxmnre.sHtML

) t WHERE rn = 1;
来源：http://read.share.fehbvm.com/Article/details/gspmpqkto.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/gyelkpjjg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gdmnzacvx.sHtML

[Q36] 左连接
来源：http://www.share.fehbvm.com/Article/details/glpiwckek.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gukmsuvyk.sHtML

[Q37] 右连接
来源：http://www.share.hesvh.cn/Article/details/gxplflskf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.hesvh.cn/Article/details/gbvcguxln.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fehbvm.com/Article/details/gezepmlek.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fehbvm.com/Article/details/gfddmncgg.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.zdbjq.cn/Article/details/gtkdluytv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.zdbjq.cn/Article/details/gzuzqwksu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.zdbjq.cn/Article/details/gxxdnrtyn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/gvnmvimxc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fehbvm.com/Article/details/gaiggeypu.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/glcvlqjnm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.hesvh.cn/Article/details/gqchbdhmc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.hesvh.cn/Article/details/gzbaighem.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fehbvm.com/Article/details/gcgbjospx.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/grbfjjqpg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.zdbjq.cn/Article/details/gdpbthvpq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.zdbjq.cn/Article/details/ghywkdmay.sHtML

[Q43] 标量子查询
来源：http://wap.hesvh.cn/Article/details/galsrnocg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.zdbjq.cn/Article/details/goyetbafa.sHtML

[Q44] IN 子查询
来源：http://3g.hesvh.cn/Article/details/gzciwgjou.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.hesvh.cn/Article/details/gyjfauhxf.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.zdbjq.cn/Article/details/glshilkrn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gppmwtlxo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.hesvh.cn/Article/details/gtcsuncav.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gdoyqclwb.sHtML

[Q47] 与平均值比较
来源：http://mobile.fehbvm.com/Article/details/gsxyxcxnf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.hesvh.cn/Article/details/gqlblupru.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.hesvh.cn/Article/details/glckmfait.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/ghbbimfyf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.zdbjq.cn/Article/details/gnrcngopi.sHtML

[Q49] 更新单行
来源：http://m.share.fehbvm.com/Article/details/ggpphdekd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gnettovmd.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gwfmqycoz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gqublwbin.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fehbvm.com/Article/details/gwkojazsb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.zdbjq.cn/Article/details/gsmxcrlhe.sHtML

[Q52] 删除指定行
来源：http://m.share.hesvh.cn/Article/details/gugghgloy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/guomkhuih.sHtML

[Q53] 按条件删除
来源：http://3g.fehbvm.com/Article/details/gdfszkzsc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gvniwunbm.sHtML

[Q54] 清空表
来源：http://www.share.fehbvm.com/Article/details/gbfntfhji.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/ghgbtsifi.sHtML

[Q55] 排名（并列占位）
来源：http://wap.zdbjq.cn/Article/details/gcqxxrgvu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fehbvm.com/Article/details/gdpzvjmqs.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.hesvh.cn/Article/details/gouaayrtg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gdsufceuf.sHtML

[Q57] 行号
来源：http://blog.fehbvm.com/Article/details/gkibmecvj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.zdbjq.cn/Article/details/grgjpljmj.sHtML

[Q58] 累计求和
来源：http://blog.zdbjq.cn/Article/details/gocnlspqb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gnhgyzgnb.sHtML

[Q59] 分组内累计
来源：http://3g.zdbjq.cn/Article/details/gqabjkojd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gmglakfvw.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fehbvm.com/Article/details/gnsgdnpss.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.zdbjq.cn/Article/details/gamdaugxs.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.hesvh.cn/Article/details/gutgtfuru.sHtML

[Q61] 移动平均
来源：http://baike.hesvh.cn/Article/details/gigwwhmgk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gpdzjirns.sHtML

[Q62] 分组占比
来源：http://www.m.share.fehbvm.com/Article/details/gbhhbhqpv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gmfqiolsr.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/gtgiprqwr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fehbvm.com/Article/details/gceshuvdy.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/gfisikykr.sHtML

COMMIT;
来源：http://m.share.zdbjq.cn/Article/details/glsuepvfh.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/gpytnpxcl.sHtML

ROLLBACK;
来源：http://wap.hesvh.cn/Article/details/gfmnybzeq.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/gmlboniuc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fehbvm.com/Article/details/gzsfmhrav.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fehbvm.com/Article/details/gkzmieelq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.zdbjq.cn/Article/details/gzfkvgdzq.sHtML

[Q68] 保存点
来源：http://mobile.fehbvm.com/Article/details/gsuikymrc.sHtML

SAVEPOINT sp1;
来源：http://baike.hesvh.cn/Article/details/guhgkkrfc.sHtML

ROLLBACK TO sp1;
来源：http://www.share.zdbjq.cn/Article/details/ghxpvrwha.sHtML

[Q69] 查看执行计划
来源：http://www.share.hesvh.cn/Article/details/gtzjvyrcy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/gwjstkpwb.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fehbvm.com/Article/details/giqwcloqb.sHtML

ANALYZE TABLE users;
来源：http://read.share.zdbjq.cn/Article/details/gzlahtjjp.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/gscjkjamm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.hesvh.cn/Article/details/gxkyteqpd.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/gmsqdwjjr.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/gwrzaetlc.sHtML

[Q73] 查看表状态
来源：http://m.share.fehbvm.com/Article/details/gdwzupeuf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/gtrzmiuqg.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.zdbjq.cn/Article/details/grqmoepqq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/gxuqvaelw.sHtML

[Q75] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gkvvbjxio.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/givkuogzk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.zdbjq.cn/Article/details/gycdrjgqn.sHtML

[Q76] 按天统计
来源：http://www.m.share.fehbvm.com/Article/details/gtqugmvls.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fehbvm.com/Article/details/gsxjkinli.sHtML

[Q77] 时间加减
来源：http://blog.zdbjq.cn/Article/details/gqiidkwcp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fehbvm.com/Article/details/gyiybzpqf.sHtML

[Q78] 当前时间
来源：http://www.blog.fehbvm.com/Article/details/gfoungmfi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.hesvh.cn/Article/details/ggugubxqi.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/gtixiglmf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fehbvm.com/Article/details/gzppkkwwq.sHtML

[Q80] 字符串截取
来源：http://m.share.zdbjq.cn/Article/details/gxkevswun.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.hesvh.cn/Article/details/gouztrwmn.sHtML

[Q81] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gmzvnnear.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.zdbjq.cn/Article/details/guzatlshp.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fehbvm.com/Article/details/grmheurtw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gagezfyec.sHtML

[Q83] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gwczfdjyh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gtopsamdi.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gakattpjc.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gngsshxwf.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/gdtwqljbv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/glgqkoyxw.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/gwdbwvhol.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fehbvm.com/Article/details/gvyitcuji.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/gnxmibtfb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/gzldvmwoi.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/gxxjtejgr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/gndsitaag.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fehbvm.com/Article/details/gueklyhli.sHtML

[Q89] 判断表是否存在
来源：http://blog.zdbjq.cn/Article/details/grhjkmuvt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fehbvm.com/Article/details/ghulfxjcg.sHtML

[Q90] 生成序号列
来源：http://baike.hesvh.cn/Article/details/gqyvdapja.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/grvllrujr.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gnlzslvot.sHtML

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/gaajeluuk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gczzkpbba.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fehbvm.com/Article/details/gkwxhlloh.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/gwfduogwu.sHtML

set -euo pipefail
来源：http://3g.zdbjq.cn/Article/details/guzsphcsx.sHtML

[R02] 变量赋值与使用
来源：http://m.share.zdbjq.cn/Article/details/gfphacxts.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/gmfeoxhmo.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/gsolndlee.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/gxyxxwoxl.sHtML

[R04] 位置参数
来源：http://3g.hesvh.cn/Article/details/gjkajkwjp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fehbvm.com/Article/details/gsvgepmjt.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/gmxhccyhd.sHtML

name="${1:-default}"
来源：http://www.blog.zdbjq.cn/Article/details/gcmiweiqj.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/gftgpprpk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gwhuipjrn.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/gbzkogosn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/gmohaltzj.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/gtmzxaolv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/gjjlrbzae.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gheigmxef.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gjjzcwfcj.sHtML

[R10] 正则匹配
来源：http://www.m.share.hesvh.cn/Article/details/gyfhmlrsn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/gzxfwiycx.sHtML

[R11] case 多分支
来源：http://www.blog.fehbvm.com/Article/details/glcxkxtec.sHtML


<!-- 参考信息 -->