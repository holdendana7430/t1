代发 wailian999

TS:   crypto.randomUUID()
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzztkgrb.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjcfotnr.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fanxiaobao.xyz/Article/details/ghkzrjxsg.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvoxxfwd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxgvmfjn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgcxbztf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyywtslq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohbzbdjm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fanxiaobao.xyz/Article/details/gazcjyoqz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvynvopmu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fanxiaobao.xyz/Article/details/govbxitlj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fanxiaobao.xyz/Article/details/gwcnopglu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gcpawxxzq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fanxiaobao.xyz/Article/details/gbenysdys.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gbarjatcx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fanxiaobao.xyz/Article/details/guwpbzkjt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fanxiaobao.xyz/Article/details/gasciwkce.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fanxiaobao.xyz/Article/details/goiwbhnfq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fanxiaobao.xyz/Article/details/gywvwihzi.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fanxiaobao.xyz/Article/details/geyndjhki.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fanxiaobao.xyz/Article/details/gklrxrhlv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrwxljtw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fanxiaobao.xyz/Article/details/gacaajuxd.sHtML

[P04] 求长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgwtbvzi.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmetuckfb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fanxiaobao.xyz/Article/details/gtgonaseb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwpcaqwo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fanxiaobao.xyz/Article/details/gklpftqtk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fanxiaobao.xyz/Article/details/gvmnominm.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fanxiaobao.xyz/Article/details/gunxqokyo.sHtML

Ruby: x.length;  x.size
来源：http://3g.fanxiaobao.xyz/Article/details/gcmgoqytd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fanxiaobao.xyz/Article/details/gdakonvsz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fanxiaobao.xyz/Article/details/gqeuxyqsd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fanxiaobao.xyz/Article/details/gbpsdyspa.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfhwwmvh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhhfvdyc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gzcjslikc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnkowepp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzapegmjo.sHtML

Ruby: a == b
来源：http://baike.fanxiaobao.xyz/Article/details/gtefhmqqn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzptwmbi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrawsies.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fanxiaobao.xyz/Article/details/gugvyucue.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycellyww.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fanxiaobao.xyz/Article/details/gldfvpdjv.sHtML

TS:   if (x == null) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gdbracsfe.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gomwolsrc.sHtML

Go:   if x == nil {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfhhgzer.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fanxiaobao.xyz/Article/details/ggwobdcfb.sHtML

C#:   if (x is null) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/glxxbffrj.sHtML

[P07] 防抖与节流
来源：http://3g.fanxiaobao.xyz/Article/details/gtofwdfnq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fanxiaobao.xyz/Article/details/gfofhwksz.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.fanxiaobao.xyz/Article/details/guiskvhoz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gliollrqk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmwclhnk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glznbgapr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqvclbyi.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gfltkxnwr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fanxiaobao.xyz/Article/details/gmminidvk.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqaccymm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjvymkow.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gprwzofqx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fanxiaobao.xyz/Article/details/grjicavgd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fanxiaobao.xyz/Article/details/gyjyoeoiy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fanxiaobao.xyz/Article/details/gykgyimiy.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fanxiaobao.xyz/Article/details/gugbkaqcv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcwgjyet.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fanxiaobao.xyz/Article/details/gqtkfqfwp.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmlktzoh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fanxiaobao.xyz/Article/details/gyumdbotm.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gfamqbbii.sHtML

[Q01] 创建表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlfwunmq.sHtML

CREATE TABLE users (
来源：http://wap.fanxiaobao.xyz/Article/details/guhrowbcr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fanxiaobao.xyz/Article/details/gkxtgabio.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvewlizt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fanxiaobao.xyz/Article/details/grhgxjnrs.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhrhkfau.sHtML

);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgfeunuq.sHtML

[Q02] 创建带外键的表
来源：http://baike.fanxiaobao.xyz/Article/details/gsqjnyuto.sHtML

CREATE TABLE orders (
来源：http://www.blog.fanxiaobao.xyz/Article/details/gquujpvce.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfzszvcz.sHtML

user_id INT NOT NULL,
来源：http://mobile.fanxiaobao.xyz/Article/details/gopcdgbyl.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fanxiaobao.xyz/Article/details/gnaanekio.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlnyuahh.sHtML

);
来源：http://wap.fanxiaobao.xyz/Article/details/gscgztrrq.sHtML

[Q03] 增加列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggpuxwsf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gfquehdbv.sHtML

[Q04] 修改列类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbdbfeyb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fanxiaobao.xyz/Article/details/gxbnsgqwq.sHtML

[Q05] 重命名列
来源：http://blog.fanxiaobao.xyz/Article/details/gddphqhvh.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqyfjqva.sHtML

[Q06] 删除列
来源：http://baike.fanxiaobao.xyz/Article/details/ghwkhsjqv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fanxiaobao.xyz/Article/details/ghovzpeqs.sHtML

[Q07] 删除表
来源：http://wap.fanxiaobao.xyz/Article/details/gisuhyftx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gokbwklch.sHtML

[Q08] 创建普通索引
来源：http://wap.fanxiaobao.xyz/Article/details/gqydofvke.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyoweehsh.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhvuplqi.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmqdwcge.sHtML

[Q10] 插入单行
来源：http://baike.fanxiaobao.xyz/Article/details/gjtakephd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxilqkud.sHtML

[Q11] 一次插入多行
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpwyybfz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsugqgjw.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fanxiaobao.xyz/Article/details/guucrnxyx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fanxiaobao.xyz/Article/details/glwcqkiqf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsupdtos.sHtML

[Q13] 忽略重复插入
来源：http://baike.fanxiaobao.xyz/Article/details/gqdwvdfrt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fanxiaobao.xyz/Article/details/ghoypadep.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyfohczp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfmoeeyi.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fanxiaobao.xyz/Article/details/gpmrobhoz.sHtML

[Q15] 查询全部
来源：http://wap.fanxiaobao.xyz/Article/details/gfmqtrtlz.sHtML

SELECT * FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnqkugxz.sHtML

[Q16] 查询指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gswgubaec.sHtML

SELECT id, name FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/goumrhzua.sHtML

[Q17] 条件查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdrcgztl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyetycevd.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmekyarr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fanxiaobao.xyz/Article/details/gclodkmjn.sHtML

[Q19] 范围查询
来源：http://baike.fanxiaobao.xyz/Article/details/gdkowkohf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fanxiaobao.xyz/Article/details/gwswrwzen.sHtML

[Q20] IN 列表
来源：http://wap.fanxiaobao.xyz/Article/details/gaslbayjv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fanxiaobao.xyz/Article/details/givaadupq.sHtML

[Q21] 空值判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdkmsbvy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjyapsip.sHtML

[Q22] 排序
来源：http://3g.fanxiaobao.xyz/Article/details/gwtbuaktg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkisoylv.sHtML

[Q23] 分页
来源：http://wap.fanxiaobao.xyz/Article/details/gdmcsdtxn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfekijwji.sHtML

[Q24] 去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpebfczbu.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gwvcyuwpk.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gufuywqto.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdfmxwqk.sHtML

[Q26] 计数
来源：http://mobile.fanxiaobao.xyz/Article/details/guvxvioik.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgrrutik.sHtML

[Q27] 条件计数
来源：http://mobile.fanxiaobao.xyz/Article/details/gttxeadjp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyppnripz.sHtML

[Q28] 求和与平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmuugbmpq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gsaxdttuf.sHtML

[Q29] 最大最小值
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvisihom.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gniasoabu.sHtML

[Q30] 分组统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfdrddle.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggszziwpn.sHtML

[Q31] 分组后过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gzfalsrms.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxpkyjde.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gpocqaalt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gscrvkukv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdiesuzxd.sHtML

[Q33] 多列分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbfjoemh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdunworx.sHtML

[Q34] 每组取第一条
来源：http://read.share.fanxiaobao.xyz/Article/details/gocrkgctm.sHtML

SELECT * FROM (
来源：http://m.share.fanxiaobao.xyz/Article/details/gxymfryqz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzjanwyy.sHtML

) t WHERE rn = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gcqvroppn.sHtML

[Q35] 内连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgrjsndt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gsbkopptn.sHtML

[Q36] 左连接
来源：http://blog.fanxiaobao.xyz/Article/details/gzkrueozi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gxijvnfdl.sHtML

[Q37] 右连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmhruqit.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmepkazjk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fanxiaobao.xyz/Article/details/gfbzsqsto.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsavjajm.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqveyefb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fanxiaobao.xyz/Article/details/ggrptctmv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gmiwmmnsp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fanxiaobao.xyz/Article/details/gcvmxjcjp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqiblfnj.sHtML

[Q41] 多表连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gvclcqdep.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fanxiaobao.xyz/Article/details/gqtlteqiy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbbkoxnc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjysdjipg.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqbsxwqh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqrptdrj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjaihrto.sHtML

[Q43] 标量子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycmkrxak.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywehjeug.sHtML

[Q44] IN 子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbmwkgyl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnezaczd.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grodnwlkt.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwotzmvfs.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fanxiaobao.xyz/Article/details/gqewdowbs.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gopzicfoj.sHtML

[Q47] 与平均值比较
来源：http://3g.fanxiaobao.xyz/Article/details/giuizehtw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fanxiaobao.xyz/Article/details/grfwsfumb.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gdcmrqxcl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fanxiaobao.xyz/Article/details/gbuzyfbop.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gscoqezxd.sHtML

[Q49] 更新单行
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrdgxkhj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gnspbwgff.sHtML

[Q50] 批量更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmojfgue.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdktelpf.sHtML

[Q51] 用子查询更新
来源：http://blog.fanxiaobao.xyz/Article/details/gokatktbn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gtvaamzwe.sHtML

[Q52] 删除指定行
来源：http://mobile.fanxiaobao.xyz/Article/details/gjiefmfzx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzclacvkw.sHtML

[Q53] 按条件删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjurxbhcm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdshifin.sHtML

[Q54] 清空表
来源：http://blog.fanxiaobao.xyz/Article/details/gurlfxmje.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fanxiaobao.xyz/Article/details/gumozrpgl.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fanxiaobao.xyz/Article/details/ggcdccfch.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gxxlcssuy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/glpmcwnzv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gvfwexxap.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnavhggr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/getufhkel.sHtML

[Q58] 累计求和
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrckbliv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gfyzwjhyk.sHtML

[Q59] 分组内累计
来源：http://baike.fanxiaobao.xyz/Article/details/gnhtjbwse.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/grnsdrrxp.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxjgjnjb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fanxiaobao.xyz/Article/details/gnahatenh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gszppeyxm.sHtML

[Q61] 移动平均
来源：http://wap.fanxiaobao.xyz/Article/details/gzrrbivgw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzlorekm.sHtML

[Q62] 分组占比
来源：http://blog.fanxiaobao.xyz/Article/details/gjtkicetx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gmoutrcff.sHtML

[Q63] 开启事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqpthswg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyywmnxu.sHtML

[Q64] 提交事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofsyvzxp.sHtML

COMMIT;
来源：http://blog.fanxiaobao.xyz/Article/details/gddtmhrks.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guryufije.sHtML

ROLLBACK;
来源：http://3g.fanxiaobao.xyz/Article/details/gtdoexymb.sHtML

[Q66] 行锁查询
来源：http://baike.fanxiaobao.xyz/Article/details/grmzhorly.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjwhbemx.sHtML

[Q67] 设置隔离级别
来源：http://baike.fanxiaobao.xyz/Article/details/gucqlvfvv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fanxiaobao.xyz/Article/details/gitvwxrii.sHtML

[Q68] 保存点
来源：http://baike.fanxiaobao.xyz/Article/details/gddvanfnv.sHtML

SAVEPOINT sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/goizwbicv.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gehlsjyzi.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/gnasvrqbd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtptrvmeq.sHtML

[Q70] 更新统计信息
来源：http://blog.fanxiaobao.xyz/Article/details/gxctrvuxw.sHtML

ANALYZE TABLE users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfitlcypm.sHtML

[Q71] 查看建表语句
来源：http://read.share.fanxiaobao.xyz/Article/details/gghlrjisi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fanxiaobao.xyz/Article/details/gbgbiotqi.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbtwdyjg.sHtML

SHOW INDEX FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gxonpokjc.sHtML

[Q73] 查看表状态
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyldvwya.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gdylohzer.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmrqtevy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/geiftplfz.sHtML

[Q75] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gzifpfjju.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgwapano.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvefkljk.sHtML

[Q76] 按天统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjwiqlhc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fanxiaobao.xyz/Article/details/gdcpgsugk.sHtML

[Q77] 时间加减
来源：http://m.share.fanxiaobao.xyz/Article/details/gpriwdqvx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfqxcvjc.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/guiuzycma.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwzhzqul.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/germhxagu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fanxiaobao.xyz/Article/details/gwrmwphid.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyedqwzqc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqulqltw.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhrlozyr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gezqfqtky.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxcwdndf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gynqkiogy.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbitrqalq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/glymvpiky.sHtML

[Q84] 去除首尾空格
来源：http://blog.fanxiaobao.xyz/Article/details/gfyfpqcrz.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gnpcmtjgb.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/gbuzhhmlp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlvvitfd.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gbpbjzroe.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbzkakdv.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/gsboijoxl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyrfuczh.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/glgtgvzco.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/gcmgwzsyo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcveheok.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfovquph.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/ghblawirr.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/ghvcguaju.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/gfmfxwttr.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/grfukbgvo.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gomjkhduq.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gastqvyko.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyojjmto.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwnueuut.sHtML

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/gzjlnzazk.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqolmtht.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwofodcgl.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/glftsdwox.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/gawrxyhxt.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gbumyohpv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfebvsdg.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfiauduf.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/gbjluknck.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gblyicrnv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gysdukiof.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnjkfxja.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gllkzwsxw.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrjvssma.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gekfagxtw.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojyidpiz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjozfbxyp.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gactrwkeo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gxsogxoww.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnaimksl.sHtML


<!-- 参考信息 -->