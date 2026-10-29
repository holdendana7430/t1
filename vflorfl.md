代发 wailian999

[O06] 使用进程池
来源：http://wap.zdbjq.cn/Article/details/guyaezaqs.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fehbvm.com/Article/details/gdswitisw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/glwdhzkyh.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/ggzhvhsgp.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/givecsjqh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.zdbjq.cn/Article/details/gyfmrdfja.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fehbvm.com/Article/details/gkpczzmbz.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/gpfyqxigq.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/gztdrcmix.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbzzbgfck.sHtML

P. 常用工具函数
来源：http://3g.zdbjq.cn/Article/details/gwnqobnox.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gsyixhusv.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gzdjbsbqv.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.zdbjq.cn/Article/details/gjfcizpds.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.hesvh.cn/Article/details/gwltvrgvp.sHtML

JS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gaiwceupc.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gvkquaazr.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gigolmcvg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.zdbjq.cn/Article/details/gyvuqtmga.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fehbvm.com/Article/details/gyhjepeud.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fehbvm.com/Article/details/gwzqahlox.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.hesvh.cn/Article/details/gbvmzaqdb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.hesvh.cn/Article/details/gauypxgzy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.zdbjq.cn/Article/details/ggomulmsv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.hesvh.cn/Article/details/gvtnzfvvu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.hesvh.cn/Article/details/gmlzutwtj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gnrfkmfsp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.zdbjq.cn/Article/details/gaqgxugex.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/gcjmahzim.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.hesvh.cn/Article/details/gnufamijy.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/gfgoncgsd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/gnezbinst.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.zdbjq.cn/Article/details/gkjzyjjbr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/guojfzuoq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gqqfhrxzx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gdddktxjq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.hesvh.cn/Article/details/gdbemulxl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/gczfbfegv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/geuapiyyj.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/gmxrstlyo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.fehbvm.com/Article/details/gwjfxbwsk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gvlnufayp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/glokgafrm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gsuickeft.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/glbapvftp.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/grggobjdm.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/gtkzqwrbp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fehbvm.com/Article/details/gpkjcsadf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/gigzvcmvc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.zdbjq.cn/Article/details/gfeoijbuv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/gzxohqwfr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fehbvm.com/Article/details/gmbfvybos.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/ghjdxhmpo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.fehbvm.com/Article/details/gewbsvzdg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gndyolaoq.sHtML

Ruby: a == b
来源：http://mobile.zdbjq.cn/Article/details/gmhelmuda.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.hesvh.cn/Article/details/gbpblzlpy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/gunnfhepl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gvfnssoeo.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gkjgchlqb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.hesvh.cn/Article/details/gbiejlwle.sHtML

TS:   if (x == null) {}
来源：http://wap.fehbvm.com/Article/details/gjxhhzesg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gsabidwat.sHtML

Go:   if x == nil {}
来源：http://3g.fehbvm.com/Article/details/gpuydmzpi.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fehbvm.com/Article/details/gteyveodm.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/gluapjhxf.sHtML

[P07] 防抖与节流
来源：http://www.m.share.hesvh.cn/Article/details/gpwduistt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fehbvm.com/Article/details/getojutch.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fehbvm.com/Article/details/ggijarqxw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/ghkncqwhl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gvagtyiah.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.hesvh.cn/Article/details/gblftuagb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/gjxkyxkas.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/geyobhfqu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/gpwgxuspp.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.hesvh.cn/Article/details/gmncwenlj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/gkdvgktme.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.zdbjq.cn/Article/details/gmbffszgd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.zdbjq.cn/Article/details/grozpaqrf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gtjznkfhv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.zdbjq.cn/Article/details/glumdklab.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/glcefursl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.zdbjq.cn/Article/details/guvinzhsg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/gbzogyhyp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvxgxazcg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.zdbjq.cn/Article/details/gyrrkyhmh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwzyutbkx.sHtML

[Q01] 创建表
来源：http://read.share.zdbjq.cn/Article/details/gevczkplg.sHtML

CREATE TABLE users (
来源：http://www.blog.hesvh.cn/Article/details/gcbzuheyu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gqgdkmand.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/gmnlgcxer.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.zdbjq.cn/Article/details/gkyworckd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fehbvm.com/Article/details/guhlofndo.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gghzdnfqt.sHtML

[Q02] 创建带外键的表
来源：http://read.share.hesvh.cn/Article/details/gerlmuoxx.sHtML

CREATE TABLE orders (
来源：http://wap.hesvh.cn/Article/details/gcmlsuitf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gbpvfmxac.sHtML

user_id INT NOT NULL,
来源：http://wap.fehbvm.com/Article/details/galcnycnt.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.zdbjq.cn/Article/details/gqpbbsmet.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.hesvh.cn/Article/details/gcgffhnyo.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gsjerkjub.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/gtmkapxnv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.hesvh.cn/Article/details/ghxoppocb.sHtML

[Q04] 修改列类型
来源：http://m.share.fehbvm.com/Article/details/gxuwgsgga.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.hesvh.cn/Article/details/gcujqbtkp.sHtML

[Q05] 重命名列
来源：http://blog.fehbvm.com/Article/details/gfmcdofjn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.hesvh.cn/Article/details/gltjsjgvp.sHtML

[Q06] 删除列
来源：http://baike.zdbjq.cn/Article/details/gvormyeex.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fehbvm.com/Article/details/geuojvxdv.sHtML

[Q07] 删除表
来源：http://www.m.share.hesvh.cn/Article/details/gnlvwuvbl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/gcgatwqto.sHtML

[Q08] 创建普通索引
来源：http://www.blog.hesvh.cn/Article/details/gxzojdjfw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gwodnsjwp.sHtML

[Q09] 创建唯一索引
来源：http://www.share.zdbjq.cn/Article/details/gbvfwzdok.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/golovsgvr.sHtML

[Q10] 插入单行
来源：http://www.blog.hesvh.cn/Article/details/gmcpnmniu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.hesvh.cn/Article/details/gawrmnlxq.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.hesvh.cn/Article/details/guebyshdw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gfydjuhvd.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.hesvh.cn/Article/details/gpnkvjlua.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.hesvh.cn/Article/details/gttgqgxbq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/gxxybzpcz.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fehbvm.com/Article/details/gtghqpnfa.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.zdbjq.cn/Article/details/gctoeruyl.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.zdbjq.cn/Article/details/glebcqlye.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/gtbkmmheq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/gihyedxrh.sHtML

[Q15] 查询全部
来源：http://read.share.hesvh.cn/Article/details/gwxuzeccy.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/ggsjqicoo.sHtML

[Q16] 查询指定列
来源：http://blog.hesvh.cn/Article/details/gdtgvixly.sHtML

SELECT id, name FROM users;
来源：http://wap.fehbvm.com/Article/details/gkgbrylzx.sHtML

[Q17] 条件查询
来源：http://baike.zdbjq.cn/Article/details/gsgohykie.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fehbvm.com/Article/details/glfviuxut.sHtML

[Q18] 模糊匹配
来源：http://www.share.zdbjq.cn/Article/details/gzvzjxzzc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.hesvh.cn/Article/details/gutyfanfo.sHtML

[Q19] 范围查询
来源：http://3g.fehbvm.com/Article/details/grlmzuixh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/guprjbqya.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/gtjbtbkgg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.hesvh.cn/Article/details/ghgjqvzxb.sHtML

[Q21] 空值判断
来源：http://read.share.zdbjq.cn/Article/details/gbknhusjy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fehbvm.com/Article/details/gnfqnesrx.sHtML

[Q22] 排序
来源：http://wap.hesvh.cn/Article/details/gonexwygl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.hesvh.cn/Article/details/gzseuokuy.sHtML

[Q23] 分页
来源：http://baike.zdbjq.cn/Article/details/gohaoldha.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fehbvm.com/Article/details/gujutgswz.sHtML

[Q24] 去重
来源：http://m.share.hesvh.cn/Article/details/gqelburyh.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gdrvggmkp.sHtML

[Q25] 只取前 N 条
来源：http://mobile.zdbjq.cn/Article/details/gpbbkimeu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gzsmydazo.sHtML

[Q26] 计数
来源：http://www.share.hesvh.cn/Article/details/ggcjfcsst.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gwyrhwgmj.sHtML

[Q27] 条件计数
来源：http://mobile.zdbjq.cn/Article/details/gaxtwvcgj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fehbvm.com/Article/details/gekiufvwt.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/gtdmdylph.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/glhsaqunl.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/gdgrtztwn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gindeepxp.sHtML

[Q30] 分组统计
来源：http://www.m.share.fehbvm.com/Article/details/gxgzgrlew.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gfazlgdkd.sHtML

[Q31] 分组后过滤
来源：http://baike.fehbvm.com/Article/details/gsmyvswgk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fehbvm.com/Article/details/gapinzvaa.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gdseglzzh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/ghpxuufnc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.hesvh.cn/Article/details/gafbqvwia.sHtML

[Q33] 多列分组
来源：http://wap.hesvh.cn/Article/details/guqipiuzp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.hesvh.cn/Article/details/gysfmjayu.sHtML

[Q34] 每组取第一条
来源：http://3g.hesvh.cn/Article/details/ghwfdxemj.sHtML

SELECT * FROM (
来源：http://www.blog.zdbjq.cn/Article/details/gzrmbnbgh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.hesvh.cn/Article/details/giukswyzl.sHtML

) t WHERE rn = 1;
来源：http://read.share.zdbjq.cn/Article/details/gixyixwfp.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/giskrgzki.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gqrhmnjou.sHtML

[Q36] 左连接
来源：http://baike.fehbvm.com/Article/details/gvxlqpglf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gaqbgazwl.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/geffdmrgn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gsagyjqeo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fehbvm.com/Article/details/gbotlpzxq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/gywjbxdjl.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fehbvm.com/Article/details/goqyuxkzh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.zdbjq.cn/Article/details/gwqynmpfn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.hesvh.cn/Article/details/gbinxfqoy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.zdbjq.cn/Article/details/grwfbgyuv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.zdbjq.cn/Article/details/grljvuyli.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/gkxdqvuae.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fehbvm.com/Article/details/gawnuuasv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fehbvm.com/Article/details/gigmbmdno.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fehbvm.com/Article/details/gykogxcgw.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.hesvh.cn/Article/details/gzdvybhnf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fehbvm.com/Article/details/gwgqyzndn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.zdbjq.cn/Article/details/gvvwmeqic.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/ghvtedgic.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.zdbjq.cn/Article/details/geunioisf.sHtML

[Q44] IN 子查询
来源：http://read.share.fehbvm.com/Article/details/gnbhkulzk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.zdbjq.cn/Article/details/guyeylwdw.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fehbvm.com/Article/details/gsrueuxof.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gxtcpexxl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.hesvh.cn/Article/details/gjveapqfr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/ghjhlawpr.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/gocggehkz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fehbvm.com/Article/details/gbolrrfps.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/gilbmujan.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/gpuuhitkm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.zdbjq.cn/Article/details/ghhvxojhf.sHtML

[Q49] 更新单行
来源：http://mobile.fehbvm.com/Article/details/gnrpigxoy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gmjfrgjiw.sHtML

[Q50] 批量更新
来源：http://wap.zdbjq.cn/Article/details/gpsjpcxse.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fehbvm.com/Article/details/gqssdwpgt.sHtML

[Q51] 用子查询更新
来源：http://wap.fehbvm.com/Article/details/gfsmrghxr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/gkjhrlhni.sHtML

[Q52] 删除指定行
来源：http://m.share.fehbvm.com/Article/details/gsfnrmsit.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gwrohhrpv.sHtML

[Q53] 按条件删除
来源：http://read.share.hesvh.cn/Article/details/gcnocxgwx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/geucjosjr.sHtML

[Q54] 清空表
来源：http://blog.fehbvm.com/Article/details/gpzjvsebf.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.hesvh.cn/Article/details/gjrujsrja.sHtML

[Q55] 排名（并列占位）
来源：http://baike.zdbjq.cn/Article/details/ghinypgii.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gtzhkgggh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.zdbjq.cn/Article/details/gyudapfre.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gmrsxaxrn.sHtML

[Q57] 行号
来源：http://baike.zdbjq.cn/Article/details/gcrdyjwxr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fehbvm.com/Article/details/gxuhxhcmf.sHtML

[Q58] 累计求和
来源：http://m.share.fehbvm.com/Article/details/gvsvmpevf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gpmmoyrpa.sHtML

[Q59] 分组内累计
来源：http://blog.fehbvm.com/Article/details/gcymqycpx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gvrbldfwq.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fehbvm.com/Article/details/gojooxjzv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.zdbjq.cn/Article/details/gmzmifltp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/ghogppyiq.sHtML

[Q61] 移动平均
来源：http://3g.fehbvm.com/Article/details/gphklqtds.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gtqtnjogk.sHtML

[Q62] 分组占比
来源：http://mobile.fehbvm.com/Article/details/ggvebssis.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gwejtvzsa.sHtML

[Q63] 开启事务
来源：http://blog.hesvh.cn/Article/details/grccjnzqg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.zdbjq.cn/Article/details/getfktskg.sHtML

[Q64] 提交事务
来源：http://www.m.share.fehbvm.com/Article/details/gwvxtmlwg.sHtML

COMMIT;
来源：http://wap.hesvh.cn/Article/details/gijcwkbnj.sHtML

[Q65] 回滚事务
来源：http://wap.zdbjq.cn/Article/details/gqjtqynmz.sHtML

ROLLBACK;
来源：http://m.share.hesvh.cn/Article/details/glsxjxyys.sHtML

[Q66] 行锁查询
来源：http://baike.zdbjq.cn/Article/details/gnphjfzhn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.zdbjq.cn/Article/details/ghqyhcmpx.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/gpllzdjoj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.hesvh.cn/Article/details/gowfkmmsp.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/gjzpyabhs.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/gvzqprjqs.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gcnldqrtt.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/gxkpgxzwz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.hesvh.cn/Article/details/gonjejrdj.sHtML

[Q70] 更新统计信息
来源：http://baike.zdbjq.cn/Article/details/ghkxkvxpy.sHtML

ANALYZE TABLE users;
来源：http://blog.hesvh.cn/Article/details/gzqjvlvly.sHtML

[Q71] 查看建表语句
来源：http://www.blog.hesvh.cn/Article/details/gfnqwvbus.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/gffqwyuyi.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/grcukmjjm.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fehbvm.com/Article/details/gaqfseggr.sHtML

[Q73] 查看表状态
来源：http://www.share.fehbvm.com/Article/details/gnhuzndzt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.hesvh.cn/Article/details/gtrutfzck.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/gpdcgzbje.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fehbvm.com/Article/details/gshldjwby.sHtML

[Q75] 日期格式化
来源：http://3g.fehbvm.com/Article/details/geekpolhe.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/guqjbuxew.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/gtkipphwb.sHtML

[Q76] 按天统计
来源：http://www.blog.fehbvm.com/Article/details/gnkeacqai.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/gjhyigtkc.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/gutakgqlo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.zdbjq.cn/Article/details/grotrgkms.sHtML

[Q78] 当前时间
来源：http://blog.fehbvm.com/Article/details/gtnefpuxn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fehbvm.com/Article/details/gkapzsnle.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gxvciuqoz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/gyntzmoqm.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/ggwsjubxq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gszaethuw.sHtML

[Q81] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gquprchem.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gytqyctga.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.zdbjq.cn/Article/details/gjytofxdz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gubmosqmz.sHtML

[Q83] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gifyvdxjv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ghtnxtdsh.sHtML

[Q84] 去除首尾空格
来源：http://baike.zdbjq.cn/Article/details/gsegimrre.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gsgucozyh.sHtML

[Q85] 数值取整
来源：http://blog.fehbvm.com/Article/details/gqsemqgej.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.hesvh.cn/Article/details/ggepsntfh.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fehbvm.com/Article/details/gmfclyaei.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/gialdiaxz.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/gfvuhyjdi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/gvcjlorot.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/gmcotxpzr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/gmzghjagl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/gnogxmncq.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gnggoqxwc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fehbvm.com/Article/details/gbbxhzogr.sHtML

[Q90] 生成序号列
来源：http://www.share.zdbjq.cn/Article/details/grbwvqtfe.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.zdbjq.cn/Article/details/gwqnzgjgd.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gsindrkpz.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/grqkmofti.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggsarlmxm.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fehbvm.com/Article/details/gmarpneho.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/goutjexpu.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/gaopiifft.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fehbvm.com/Article/details/glcmdredt.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/gawplrysp.sHtML

[R03] 只读变量
来源：http://www.blog.fehbvm.com/Article/details/gvffskhds.sHtML


<!-- 参考信息 -->