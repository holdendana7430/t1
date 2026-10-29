代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.zdbjq.cn/Article/details/gdfrqfhcu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.zdbjq.cn/Article/details/gkuzzrjwe.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fehbvm.com/Article/details/gmtrbtecw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/gztqmkjgl.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/gzxcfrvdu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.hesvh.cn/Article/details/gutthphzt.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fehbvm.com/Article/details/gklxfsgsy.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gdcmuyjke.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gskcytlky.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.fehbvm.com/Article/details/gqciwfjec.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.zdbjq.cn/Article/details/gkpjtmqhn.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/guznuddru.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/gswhftrjk.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gduseyyna.sHtML

P. 常用工具函数
来源：http://www.m.share.zdbjq.cn/Article/details/gdqplhsex.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghoeizptq.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gpjqjnmak.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/gohpdpnjc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fehbvm.com/Article/details/gywgxhyiw.sHtML

JS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gecnnkvoj.sHtML

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gmauceabs.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/gmdwtrtic.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fehbvm.com/Article/details/gmphmopnh.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.zdbjq.cn/Article/details/gjywhmghe.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/getmrpwad.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.zdbjq.cn/Article/details/gjvqcdqzz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.zdbjq.cn/Article/details/gozorgtld.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/ggumisvbm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/gdrkcwott.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fehbvm.com/Article/details/gzuwcwrnn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/grpgcbaeb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/gsppjpkyq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fehbvm.com/Article/details/gxmqihugq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.zdbjq.cn/Article/details/ggjtwutoh.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/ggwwneqcq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.zdbjq.cn/Article/details/ggbaksocm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.hesvh.cn/Article/details/gxapaivla.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gxttxxzaa.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gnrvqwmwz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fehbvm.com/Article/details/gvlojuhye.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/gsmtmoqjz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gxcjkqmqy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.hesvh.cn/Article/details/ghgwhmmvz.sHtML

[P04] 求长度
来源：http://blog.fehbvm.com/Article/details/gzlarlfhg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.zdbjq.cn/Article/details/gsohcntfl.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gumkvhrwh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/ggwabpmga.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gqytheuzk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fehbvm.com/Article/details/gsknemkyk.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.zdbjq.cn/Article/details/gsauodqwp.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/gnpqozfpu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gjttjptfh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/ggogcdtla.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.zdbjq.cn/Article/details/gwvjxhpej.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.zdbjq.cn/Article/details/giylmogxu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.zdbjq.cn/Article/details/grsgxiaiy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/guhmgzgah.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/goukjldxr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gjqlxarlq.sHtML

Ruby: a == b
来源：http://baike.fehbvm.com/Article/details/gstxbonmz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.zdbjq.cn/Article/details/gfrlefghv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.zdbjq.cn/Article/details/gucdmjfjw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/gxwpqjwqf.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fehbvm.com/Article/details/gpfjstfww.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/guclzlptm.sHtML

TS:   if (x == null) {}
来源：http://read.share.fehbvm.com/Article/details/gmyuurudn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gzettgwnk.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/gvgjjckev.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.hesvh.cn/Article/details/gapvqbwaj.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gmsmhscsc.sHtML

[P07] 防抖与节流
来源：http://www.blog.fehbvm.com/Article/details/godcigqlk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fehbvm.com/Article/details/gubkdqtgg.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.hesvh.cn/Article/details/giqvoitjs.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gsdruvnar.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gozamousa.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fehbvm.com/Article/details/gsjayhzbu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/gekphvrbp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fehbvm.com/Article/details/guuphgkic.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fehbvm.com/Article/details/ggoenlmks.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/gealibavd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.zdbjq.cn/Article/details/gkbekndsq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.zdbjq.cn/Article/details/geklvordz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/ghdsblaog.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/grolqjtei.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.zdbjq.cn/Article/details/gngwnxxkx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/gbzfrsajt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/gxecjzaij.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/gkvegnpld.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/getkijueo.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/gsshxxsjx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/golezuvvi.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/gxzlrwojf.sHtML

CREATE TABLE users (
来源：http://m.share.zdbjq.cn/Article/details/gixdscnpr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gjlmelaca.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gtrwruiqf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/gzrsusent.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.zdbjq.cn/Article/details/gnbarqtle.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gxdeubjll.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/glxlrmkms.sHtML

CREATE TABLE orders (
来源：http://m.share.zdbjq.cn/Article/details/golloskmb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gjwsifemf.sHtML

user_id INT NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gmhosquiw.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.hesvh.cn/Article/details/gujxcubok.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.zdbjq.cn/Article/details/gbmcmqbok.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gqxoxshyi.sHtML

[Q03] 增加列
来源：http://read.share.hesvh.cn/Article/details/gjaedrhyj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fehbvm.com/Article/details/gjicdshde.sHtML

[Q04] 修改列类型
来源：http://www.m.share.zdbjq.cn/Article/details/gghlaxwwa.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.hesvh.cn/Article/details/gjqtlbglm.sHtML

[Q05] 重命名列
来源：http://baike.fehbvm.com/Article/details/gwavymheq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fehbvm.com/Article/details/gglaqflrx.sHtML

[Q06] 删除列
来源：http://www.share.fehbvm.com/Article/details/ghnjloknu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/gjgqacobr.sHtML

[Q07] 删除表
来源：http://baike.zdbjq.cn/Article/details/gzlvoehmo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.hesvh.cn/Article/details/gvmhunxvr.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/glwciceed.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/ginwregkz.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/ghhvkvsyb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gzojiusqo.sHtML

[Q10] 插入单行
来源：http://www.blog.fehbvm.com/Article/details/ginnfltvq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fehbvm.com/Article/details/ggrsalvwf.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fehbvm.com/Article/details/glbevzvdx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.zdbjq.cn/Article/details/gowrxcyzk.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.zdbjq.cn/Article/details/gmaritghm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/gduapbgrk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/gylitncov.sHtML

[Q13] 忽略重复插入
来源：http://blog.zdbjq.cn/Article/details/gnmrpuhuv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gthirdcry.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fehbvm.com/Article/details/gbfuexdpa.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/gxhjzeagm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/gbengngro.sHtML

[Q15] 查询全部
来源：http://read.share.hesvh.cn/Article/details/gciotgpjf.sHtML

SELECT * FROM users;
来源：http://read.share.hesvh.cn/Article/details/gxwrsktxx.sHtML

[Q16] 查询指定列
来源：http://read.share.fehbvm.com/Article/details/gqmsqxfym.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gfcwpbyez.sHtML

[Q17] 条件查询
来源：http://mobile.fehbvm.com/Article/details/gtlpatvks.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.zdbjq.cn/Article/details/glthorzmp.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gfwkpfjnf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/gjyduggjn.sHtML

[Q19] 范围查询
来源：http://read.share.fehbvm.com/Article/details/gdtesqcsc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/gfbnamhgx.sHtML

[Q20] IN 列表
来源：http://blog.fehbvm.com/Article/details/gheypzhfd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.hesvh.cn/Article/details/gtghbqvfk.sHtML

[Q21] 空值判断
来源：http://m.share.fehbvm.com/Article/details/gilboheyx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.hesvh.cn/Article/details/gfbkjvvsp.sHtML

[Q22] 排序
来源：http://3g.zdbjq.cn/Article/details/ghtsrzcba.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.hesvh.cn/Article/details/gqwjtlwny.sHtML

[Q23] 分页
来源：http://wap.fehbvm.com/Article/details/gvkncbhhg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fehbvm.com/Article/details/gyxuymnsx.sHtML

[Q24] 去重
来源：http://wap.fehbvm.com/Article/details/gfdkyurax.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fehbvm.com/Article/details/gpdngcbnq.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/gzxdmwhxv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/gnxkmmice.sHtML

[Q26] 计数
来源：http://blog.hesvh.cn/Article/details/gilfdzffm.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gytnrimmc.sHtML

[Q27] 条件计数
来源：http://wap.fehbvm.com/Article/details/gwjjrawkt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.hesvh.cn/Article/details/ggwdyclwn.sHtML

[Q28] 求和与平均
来源：http://blog.hesvh.cn/Article/details/gwxlgnzhj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gkvwnqoqk.sHtML

[Q29] 最大最小值
来源：http://www.share.fehbvm.com/Article/details/gokkxoqii.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/glhbuxgfu.sHtML

[Q30] 分组统计
来源：http://wap.zdbjq.cn/Article/details/gxbvutmvh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gpcuapbsu.sHtML

[Q31] 分组后过滤
来源：http://baike.zdbjq.cn/Article/details/gqnwbxxjk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.hesvh.cn/Article/details/gegfpdhrb.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gggtcjktx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gpzpbzhyr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/gpenwlpdc.sHtML

[Q33] 多列分组
来源：http://3g.zdbjq.cn/Article/details/guhvtbufk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/golurgzcx.sHtML

[Q34] 每组取第一条
来源：http://3g.fehbvm.com/Article/details/gszkmmlxd.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/gclsojcrh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.zdbjq.cn/Article/details/gamvqvgna.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/gucszrdnq.sHtML

[Q35] 内连接
来源：http://m.share.fehbvm.com/Article/details/goejpmynd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gktcppwsi.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/gkgsmxfpw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gtvicpgub.sHtML

[Q37] 右连接
来源：http://www.m.share.hesvh.cn/Article/details/gldthowpr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gvhrreekl.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fehbvm.com/Article/details/gfrldtkba.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gnwesdndo.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.zdbjq.cn/Article/details/gvdyexxkl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fehbvm.com/Article/details/gpgpsjomy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fehbvm.com/Article/details/gbzjhjdrj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/gyfugekbk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.zdbjq.cn/Article/details/gksctzorh.sHtML

[Q41] 多表连接
来源：http://read.share.hesvh.cn/Article/details/gnyfjavru.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/geqojnucs.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fehbvm.com/Article/details/gwqbtmoqx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fehbvm.com/Article/details/gndwgojew.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fehbvm.com/Article/details/goyqjrbjm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.hesvh.cn/Article/details/gxxiyfgid.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.zdbjq.cn/Article/details/gfkbbwumf.sHtML

[Q43] 标量子查询
来源：http://m.share.zdbjq.cn/Article/details/grkadjclc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fehbvm.com/Article/details/gknhaxhqw.sHtML

[Q44] IN 子查询
来源：http://m.share.hesvh.cn/Article/details/giizfuiyx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.zdbjq.cn/Article/details/gzvdhiart.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fehbvm.com/Article/details/gyhdirqsq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gxxrdnzsa.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.hesvh.cn/Article/details/gmvgjoktu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/grkuvkwzy.sHtML

[Q47] 与平均值比较
来源：http://read.share.zdbjq.cn/Article/details/gfoedvdog.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.hesvh.cn/Article/details/gcjbhohvg.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fehbvm.com/Article/details/geotfeyxs.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fehbvm.com/Article/details/gjiumjqnk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.hesvh.cn/Article/details/gtmcbbvup.sHtML

[Q49] 更新单行
来源：http://3g.hesvh.cn/Article/details/guctyvqxm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/ggjhiadlr.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/gasalvjka.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fehbvm.com/Article/details/gtvqvyajc.sHtML

[Q51] 用子查询更新
来源：http://3g.hesvh.cn/Article/details/gzqvlbpfq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fehbvm.com/Article/details/gntrkpywr.sHtML

[Q52] 删除指定行
来源：http://www.blog.hesvh.cn/Article/details/grxkzayzk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gsofozbah.sHtML

[Q53] 按条件删除
来源：http://www.blog.fehbvm.com/Article/details/gfkbljkfy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/gimtkfppl.sHtML

[Q54] 清空表
来源：http://blog.zdbjq.cn/Article/details/gldavujwe.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.hesvh.cn/Article/details/gxkerbvku.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/gwhvdwjme.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gjnbzwqgc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.hesvh.cn/Article/details/gefbliejw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gnrxgwdpa.sHtML

[Q57] 行号
来源：http://blog.hesvh.cn/Article/details/gzdkhqvyz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gouhtdkdm.sHtML

[Q58] 累计求和
来源：http://www.share.fehbvm.com/Article/details/gjfoxnhib.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gfplcowkh.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/gayakcukm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.hesvh.cn/Article/details/grjqxptab.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fehbvm.com/Article/details/grrgcxqbe.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.hesvh.cn/Article/details/gcxcibfwl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/goxwraccm.sHtML

[Q61] 移动平均
来源：http://3g.zdbjq.cn/Article/details/gfdfejtvn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gtwzuyqsc.sHtML

[Q62] 分组占比
来源：http://baike.fehbvm.com/Article/details/gcnkbyavp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gcmgdvhka.sHtML

[Q63] 开启事务
来源：http://3g.hesvh.cn/Article/details/grnhbxnga.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fehbvm.com/Article/details/girjeiqhr.sHtML

[Q64] 提交事务
来源：http://3g.hesvh.cn/Article/details/gigozosah.sHtML

COMMIT;
来源：http://www.share.zdbjq.cn/Article/details/gdxrohioi.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gvzcxpcnx.sHtML

ROLLBACK;
来源：http://3g.zdbjq.cn/Article/details/gbhdlnbit.sHtML

[Q66] 行锁查询
来源：http://3g.zdbjq.cn/Article/details/gssvddxkc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.hesvh.cn/Article/details/gbjorrmwm.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/gtmiyhsqq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/gmxivgtwi.sHtML

[Q68] 保存点
来源：http://wap.fehbvm.com/Article/details/gyqsoksqv.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/ghxfqewve.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/gwipshbsd.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fehbvm.com/Article/details/gapdlmzbz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fehbvm.com/Article/details/gjunhplhj.sHtML

[Q70] 更新统计信息
来源：http://baike.zdbjq.cn/Article/details/ggqayircb.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/gctsxzieh.sHtML

[Q71] 查看建表语句
来源：http://blog.hesvh.cn/Article/details/gzbneoksc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fehbvm.com/Article/details/gpxaprbzb.sHtML

[Q72] 查看索引
来源：http://3g.zdbjq.cn/Article/details/gcwcvjvrt.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/gclzizyqt.sHtML

[Q73] 查看表状态
来源：http://www.m.share.zdbjq.cn/Article/details/gearxplvb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gjtkdvzwy.sHtML

[Q74] 强制使用索引
来源：http://www.share.zdbjq.cn/Article/details/gwkvmiycc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.zdbjq.cn/Article/details/ginpfydai.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gdwhmnmtm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fehbvm.com/Article/details/gifnicsfu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/gcmdemjrv.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/gicschiuo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.hesvh.cn/Article/details/govkgcgly.sHtML

[Q77] 时间加减
来源：http://3g.zdbjq.cn/Article/details/gxjujemwp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/gjrvvihlq.sHtML

[Q78] 当前时间
来源：http://baike.zdbjq.cn/Article/details/gqcyslxmd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.hesvh.cn/Article/details/gvkfulopa.sHtML

[Q79] 字符串拼接
来源：http://wap.fehbvm.com/Article/details/gcnsxjdfy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.zdbjq.cn/Article/details/gagjqzzet.sHtML

[Q80] 字符串截取
来源：http://www.share.fehbvm.com/Article/details/gyydsbcmb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.hesvh.cn/Article/details/grtddaawi.sHtML

[Q81] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gxwyfwpft.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/gceaibetl.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fehbvm.com/Article/details/gecjbsamb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gsgztayup.sHtML

[Q83] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gubexzbwa.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/guubwjfbt.sHtML

[Q84] 去除首尾空格
来源：http://wap.zdbjq.cn/Article/details/gyfbobisf.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gnayjsvoj.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/gpzzhvxiw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/gxyyazwni.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/gvhtmibfg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fehbvm.com/Article/details/gnuyjbaej.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fehbvm.com/Article/details/gbqohkjhv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/ghmavzbwr.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.zdbjq.cn/Article/details/gbkpsouzl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/gbilwmzbz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gfziwkrrw.sHtML

[Q89] 判断表是否存在
来源：http://baike.hesvh.cn/Article/details/gxwfhwnql.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.hesvh.cn/Article/details/gwgowgrxy.sHtML

[Q90] 生成序号列
来源：http://www.share.hesvh.cn/Article/details/gmeyyuxlt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.zdbjq.cn/Article/details/gxjwfahlb.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ganufifkc.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/gxiccfqbv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gccgohfgy.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/ghfzqaafi.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/gyfxnpcjz.sHtML


<!-- 参考信息 -->