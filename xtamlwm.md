代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gsaqfswfk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.zdbjq.cn/Article/details/gctbmdlra.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gzwwnupho.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gwfgkpdcj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/gvwrptfgm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.zdbjq.cn/Article/details/ghcevrgmf.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/gfjodjzdj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.zdbjq.cn/Article/details/gvwweucwa.sHtML

[O06] 使用进程池
来源：http://read.share.zdbjq.cn/Article/details/grkmzakpm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/gvtqqatwr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.hesvh.cn/Article/details/gcdogwirz.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gvmwngysl.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gbewujkgm.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fehbvm.com/Article/details/gxaifueeu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.hesvh.cn/Article/details/gwltatvye.sHtML

Ruby: // fork 块
来源：http://m.share.hesvh.cn/Article/details/gcbeedizo.sHtML

C#:   Parallel.For
来源：http://m.share.hesvh.cn/Article/details/glxcoptod.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gsktoogfv.sHtML

P. 常用工具函数
来源：http://m.share.hesvh.cn/Article/details/gxkpgenfl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gusclnmaa.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gxhhaktlz.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/gtvnqbpxp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.zdbjq.cn/Article/details/gxngkjbpj.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gxmmisuzu.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/graqxbzwi.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.zdbjq.cn/Article/details/gzbtzwyff.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fehbvm.com/Article/details/gosxqvrvo.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/gluvsqkrt.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.hesvh.cn/Article/details/gzfyhxylk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/guuvqqyqu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/glhoaqddl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.hesvh.cn/Article/details/gwskgbcqt.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/gecsimjwa.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.zdbjq.cn/Article/details/guhdponbe.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.hesvh.cn/Article/details/glmucuxmn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.zdbjq.cn/Article/details/gzhvjboqz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/gihiigdgk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/gyoygwloc.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/gxjptrryh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.hesvh.cn/Article/details/gikvzdhbq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/gtodzzcdl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/ggdssdiac.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gtiennhek.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/ghajyrdme.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.hesvh.cn/Article/details/gzdbsunou.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fehbvm.com/Article/details/gxgnbmzdz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.hesvh.cn/Article/details/gpkbildud.sHtML

[P04] 求长度
来源：http://www.m.share.hesvh.cn/Article/details/gddwmynhi.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/ghuvenwai.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gqrxmxffc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gqphjycyd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/guzpzcflg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.hesvh.cn/Article/details/goyzxptyj.sHtML

Go:   len(arr);  len(m)
来源：http://3g.hesvh.cn/Article/details/gpkmlklfl.sHtML

Ruby: x.length;  x.size
来源：http://read.share.zdbjq.cn/Article/details/gcikfnbmw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/glizhutjj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/grvmxjemn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.zdbjq.cn/Article/details/gumskatlc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.hesvh.cn/Article/details/getppjxvj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fehbvm.com/Article/details/gqedvfges.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gqqmdybnt.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.hesvh.cn/Article/details/gzrvmufbc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gcrbqjayq.sHtML

Ruby: a == b
来源：http://blog.fehbvm.com/Article/details/gsvkpnfxf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/grbwixggm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.zdbjq.cn/Article/details/golsnziic.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.zdbjq.cn/Article/details/gblqmeenx.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/gljrmoaua.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gycajhmqb.sHtML

TS:   if (x == null) {}
来源：http://read.share.zdbjq.cn/Article/details/gfgknajbq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gjmgekqrh.sHtML

Go:   if x == nil {}
来源：http://blog.zdbjq.cn/Article/details/gkcmebhka.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.zdbjq.cn/Article/details/gfijxxwja.sHtML

C#:   if (x is null) {}
来源：http://blog.zdbjq.cn/Article/details/gytjwqrrw.sHtML

[P07] 防抖与节流
来源：http://3g.hesvh.cn/Article/details/gzjjlxyui.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/gmvflleil.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.hesvh.cn/Article/details/gegwxeeqf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gsymmupzh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gmshexqab.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.hesvh.cn/Article/details/gfpgciywk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/gudhsokse.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.fehbvm.com/Article/details/gsruxtdnl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.zdbjq.cn/Article/details/gfupjzsdv.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/glzuxcyya.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fehbvm.com/Article/details/gokpqfduj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gcucrncuf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.zdbjq.cn/Article/details/gvagufhag.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/ggknkdtxm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.zdbjq.cn/Article/details/gzastrdif.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.hesvh.cn/Article/details/guybciuct.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.hesvh.cn/Article/details/gqnykdzab.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.hesvh.cn/Article/details/gusicfyld.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gapiansbd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.hesvh.cn/Article/details/gajrthovk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/giicngjzy.sHtML

[Q01] 创建表
来源：http://baike.fehbvm.com/Article/details/gfqhwbumh.sHtML

CREATE TABLE users (
来源：http://www.blog.hesvh.cn/Article/details/gbnpcazhq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gffgusnob.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gligfwvgf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/gceazwgvd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/gogmijovd.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gbqijcbbt.sHtML

[Q02] 创建带外键的表
来源：http://m.share.hesvh.cn/Article/details/gylfckgut.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fehbvm.com/Article/details/ggmymzuiq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/ghoombpcg.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gvxevwgvf.sHtML

amount DECIMAL(10, 2),
来源：http://blog.zdbjq.cn/Article/details/gjpygysdq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fehbvm.com/Article/details/grihmahbo.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gidfhysxm.sHtML

[Q03] 增加列
来源：http://www.blog.fehbvm.com/Article/details/gyohppbjt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fehbvm.com/Article/details/gqblfmowc.sHtML

[Q04] 修改列类型
来源：http://baike.hesvh.cn/Article/details/gtfrpzvud.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fehbvm.com/Article/details/gapdsvrlj.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/gueiavuaq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fehbvm.com/Article/details/gubpisxdy.sHtML

[Q06] 删除列
来源：http://wap.fehbvm.com/Article/details/gxtcdbklt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.hesvh.cn/Article/details/gdkfmipcy.sHtML

[Q07] 删除表
来源：http://wap.zdbjq.cn/Article/details/gidlqnsrt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.hesvh.cn/Article/details/gshcrxcsg.sHtML

[Q08] 创建普通索引
来源：http://blog.fehbvm.com/Article/details/gainmamza.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/ggjqphety.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/gjgbhyeoj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gubpxedaq.sHtML

[Q10] 插入单行
来源：http://blog.fehbvm.com/Article/details/ggrqsoana.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gbyogwlea.sHtML

[Q11] 一次插入多行
来源：http://blog.fehbvm.com/Article/details/gsopljdpy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fehbvm.com/Article/details/gsswvjmlz.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/gtzwyrxic.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.zdbjq.cn/Article/details/gfyyhgvrc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.hesvh.cn/Article/details/gncixlrnh.sHtML

[Q13] 忽略重复插入
来源：http://www.share.hesvh.cn/Article/details/gxzebjbnj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gpwwuiiuw.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.zdbjq.cn/Article/details/giucufdop.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/gnvwxjtni.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/gndakktgl.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/gpggruyjb.sHtML

SELECT * FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gcyvrbqbe.sHtML

[Q16] 查询指定列
来源：http://www.blog.zdbjq.cn/Article/details/gejlorfnv.sHtML

SELECT id, name FROM users;
来源：http://www.share.hesvh.cn/Article/details/guerwcrkm.sHtML

[Q17] 条件查询
来源：http://blog.zdbjq.cn/Article/details/gprwcssjs.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.hesvh.cn/Article/details/gybqjcdwf.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.hesvh.cn/Article/details/guzgnvhev.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.hesvh.cn/Article/details/gvjchfvhr.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/gfcwsssfo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fehbvm.com/Article/details/gnaetxkeq.sHtML

[Q20] IN 列表
来源：http://read.share.hesvh.cn/Article/details/gteehbegm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.hesvh.cn/Article/details/giedgfqii.sHtML

[Q21] 空值判断
来源：http://blog.fehbvm.com/Article/details/gakgcdcbo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gbkszzczv.sHtML

[Q22] 排序
来源：http://www.blog.hesvh.cn/Article/details/gsynzphqw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.zdbjq.cn/Article/details/gahzngryu.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/gmtopwgay.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.hesvh.cn/Article/details/ghkylnwtj.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/ghsgtmwai.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gdlvmiobg.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/ghyrugsia.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.hesvh.cn/Article/details/gctwakfnx.sHtML

[Q26] 计数
来源：http://mobile.hesvh.cn/Article/details/gzgonhhvf.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gsnojzehs.sHtML

[Q27] 条件计数
来源：http://read.share.hesvh.cn/Article/details/gqwjebksn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fehbvm.com/Article/details/guwgglknj.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/gspjzdhqm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gvpavxjiv.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/gmlqrlbjh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gmmukvkyk.sHtML

[Q30] 分组统计
来源：http://read.share.zdbjq.cn/Article/details/gjczusbls.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gyfybrpxy.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/ggjfhpyvx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fehbvm.com/Article/details/gvsrglhfz.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gabomfkzd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gfnaunmps.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.zdbjq.cn/Article/details/gwmesmmym.sHtML

[Q33] 多列分组
来源：http://baike.fehbvm.com/Article/details/ghuwghxok.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fehbvm.com/Article/details/gwqrvdunw.sHtML

[Q34] 每组取第一条
来源：http://blog.hesvh.cn/Article/details/gvnhtgrkq.sHtML

SELECT * FROM (
来源：http://m.share.fehbvm.com/Article/details/gqpkcbzee.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fehbvm.com/Article/details/gqczdxply.sHtML

) t WHERE rn = 1;
来源：http://m.share.hesvh.cn/Article/details/gvferrdqi.sHtML

[Q35] 内连接
来源：http://www.m.share.fehbvm.com/Article/details/gmbamiweq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gthduqubl.sHtML

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/gfvjyljei.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/glabkwjrj.sHtML

[Q37] 右连接
来源：http://baike.fehbvm.com/Article/details/gyzwjefhr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/gmarqfwmp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/gyhotmiop.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fehbvm.com/Article/details/gjaypgnnt.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/gkdihsvlh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.hesvh.cn/Article/details/gywxbdcyb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/gmhorzjia.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fehbvm.com/Article/details/gdvucnlbq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.hesvh.cn/Article/details/gwvtgxotd.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/glpmtoqtp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/gobuestzq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/gpkjwmhwk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/gkstznbxl.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.zdbjq.cn/Article/details/ggyizkdrf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/gobrmnubz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.hesvh.cn/Article/details/gjuxtxxdj.sHtML

[Q43] 标量子查询
来源：http://m.share.hesvh.cn/Article/details/glwdpjaty.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.hesvh.cn/Article/details/gcstccngk.sHtML

[Q44] IN 子查询
来源：http://www.m.share.hesvh.cn/Article/details/grazoxsoo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/gcflznewd.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.hesvh.cn/Article/details/gdivnctob.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gprdryhsh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.zdbjq.cn/Article/details/gfaarvehl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gtkoztlxi.sHtML

[Q47] 与平均值比较
来源：http://mobile.hesvh.cn/Article/details/gkydfyyuv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.hesvh.cn/Article/details/gqzhedixl.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.zdbjq.cn/Article/details/geskqbljy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.hesvh.cn/Article/details/gniijhgki.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.hesvh.cn/Article/details/gktcidxye.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/gbxvgcpsp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gqplfcnto.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/glsjukxoo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/gwvzbwfpz.sHtML

[Q51] 用子查询更新
来源：http://3g.zdbjq.cn/Article/details/gnzwptbiw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.zdbjq.cn/Article/details/gayzxmxrq.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/gkbtfszzn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gudmoqwlx.sHtML

[Q53] 按条件删除
来源：http://www.share.zdbjq.cn/Article/details/gztkkmtxv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.hesvh.cn/Article/details/gbofugugq.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/gmpxlasmy.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fehbvm.com/Article/details/gqyggyerw.sHtML

[Q55] 排名（并列占位）
来源：http://baike.hesvh.cn/Article/details/grbjiugsf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gdnusecgu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.zdbjq.cn/Article/details/giexpqfgs.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gsghhzfyf.sHtML

[Q57] 行号
来源：http://www.share.hesvh.cn/Article/details/gqzvomehx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.hesvh.cn/Article/details/gffwyjnew.sHtML

[Q58] 累计求和
来源：http://blog.hesvh.cn/Article/details/gyqfwolqu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gnbnmonvv.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/gspwwzvve.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gvvhjdhqf.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.hesvh.cn/Article/details/gkdhmuulh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/gqqdbqcba.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gutzwqwbs.sHtML

[Q61] 移动平均
来源：http://mobile.hesvh.cn/Article/details/gcavnvdnd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gdxxtxqxr.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/gimdbegtz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gurieqtie.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/gjwxcfdhc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.zdbjq.cn/Article/details/grnevhnpk.sHtML

[Q64] 提交事务
来源：http://blog.hesvh.cn/Article/details/gwxowwwma.sHtML

COMMIT;
来源：http://www.blog.zdbjq.cn/Article/details/glgnwftyx.sHtML

[Q65] 回滚事务
来源：http://baike.hesvh.cn/Article/details/gcmolmhnn.sHtML

ROLLBACK;
来源：http://wap.hesvh.cn/Article/details/gelglcsup.sHtML

[Q66] 行锁查询
来源：http://m.share.fehbvm.com/Article/details/gzjxknyca.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fehbvm.com/Article/details/gzhvonjmc.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fehbvm.com/Article/details/gzevmzxhh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fehbvm.com/Article/details/gvrovfgkv.sHtML

[Q68] 保存点
来源：http://www.blog.hesvh.cn/Article/details/gpikgeotj.sHtML

SAVEPOINT sp1;
来源：http://baike.hesvh.cn/Article/details/gzxctjsjy.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/gtkdfnsua.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/gmbroaedv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.hesvh.cn/Article/details/gxnkdawci.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/gztchywvj.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/gvnouahhv.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.hesvh.cn/Article/details/guckipxgg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fehbvm.com/Article/details/gpnnpkvhn.sHtML

[Q72] 查看索引
来源：http://baike.fehbvm.com/Article/details/goftpgnlv.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fehbvm.com/Article/details/gghinleqa.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/gcfcweltx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/gnfbcwznp.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fehbvm.com/Article/details/gvzidixgz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.zdbjq.cn/Article/details/gpwojtwzl.sHtML

[Q75] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/ginsttsxt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gakkubtcv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fehbvm.com/Article/details/gsnosczyn.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/grxrzwnzx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/gjyjfawdg.sHtML

[Q77] 时间加减
来源：http://mobile.zdbjq.cn/Article/details/gtxcqywmj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.hesvh.cn/Article/details/gtarwkkck.sHtML

[Q78] 当前时间
来源：http://blog.fehbvm.com/Article/details/gchlomass.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.zdbjq.cn/Article/details/glbctpbuu.sHtML

[Q79] 字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gsbihucld.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.zdbjq.cn/Article/details/gqtweglor.sHtML

[Q80] 字符串截取
来源：http://baike.fehbvm.com/Article/details/gkmeydjaw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gddxbejhq.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gkksdkphx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/gmnvcjptm.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gfrucbhsr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gbqitjigz.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/guqhdrwkx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gtrouzcaa.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/gljraxfqc.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gojzuzmxx.sHtML

[Q85] 数值取整
来源：http://read.share.zdbjq.cn/Article/details/ghnbpsngr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/gpbqoivgf.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/gupueyozr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fehbvm.com/Article/details/gnnnwugbs.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/gbkqapsev.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/gzsxcbdov.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.zdbjq.cn/Article/details/gzjhqhnjz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fehbvm.com/Article/details/geblcbegf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.zdbjq.cn/Article/details/gqfforycd.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/gffosefby.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.hesvh.cn/Article/details/ganavbjuk.sHtML

[Q90] 生成序号列
来源：http://blog.zdbjq.cn/Article/details/gwjpbttnd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.hesvh.cn/Article/details/gqidiiica.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkvksmpkw.sHtML


<!-- 参考信息 -->