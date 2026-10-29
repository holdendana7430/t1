代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/gmmowbpzr.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fehbvm.com/Article/details/gbmtsmojk.sHtML

Py:   with lock: shared += 1
来源：http://m.share.hesvh.cn/Article/details/gpptncyqw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.hesvh.cn/Article/details/gcguqqlnv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/gsvhnexio.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gdndtglug.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gsaloobib.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/ghygohlfj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/gzzcijoof.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/glgnjnmbq.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fehbvm.com/Article/details/gzxctjigz.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.hesvh.cn/Article/details/gnizjogyb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/ginrrzlwz.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gvuxnqfqp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/gasjnforz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.zdbjq.cn/Article/details/gjckllvvb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/gwsrrjute.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/gtvhtuypi.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/gqahjrfnx.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fehbvm.com/Article/details/gpubqhogs.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.hesvh.cn/Article/details/gzotvijuv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.hesvh.cn/Article/details/gaopclqpg.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gbnnoetxu.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gdlzgrjlo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.hesvh.cn/Article/details/geodwgqlt.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.hesvh.cn/Article/details/gukiluizd.sHtML

Ruby: threads.map(&:join)
来源：http://wap.hesvh.cn/Article/details/gbzoydfnl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/gzjtfzjmx.sHtML

[O06] 使用进程池
来源：http://www.blog.zdbjq.cn/Article/details/gbrunwivl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.hesvh.cn/Article/details/gurmqyakq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.zdbjq.cn/Article/details/gjuzixcva.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/grjvrtvei.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gcyaniyme.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/gqslnbpzo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.zdbjq.cn/Article/details/gynysidsv.sHtML

Ruby: // fork 块
来源：http://blog.fehbvm.com/Article/details/ghlwlkyqf.sHtML

C#:   Parallel.For
来源：http://baike.zdbjq.cn/Article/details/gmunzuwpb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzldxfzlh.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/gnliycebd.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwlbwolmd.sHtML

[P01] 生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gwiupllga.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.hesvh.cn/Article/details/gcddgxfjv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gxktctpxg.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gcctvigfe.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gwqmeyfiv.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fehbvm.com/Article/details/ghapkzems.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.zdbjq.cn/Article/details/gshqolota.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fehbvm.com/Article/details/giydwnwus.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/guxuzjqrd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/gtqjjvyqf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.zdbjq.cn/Article/details/gifgbnend.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fehbvm.com/Article/details/gqjhnmvfi.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.hesvh.cn/Article/details/gqanpqqpj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.zdbjq.cn/Article/details/gonmsfywu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/gtzsmkbda.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fehbvm.com/Article/details/gpsfazneu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/gpelcnsaz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fehbvm.com/Article/details/goxpanihh.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/gvpwqnumi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.hesvh.cn/Article/details/gqsxsdjrw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fehbvm.com/Article/details/gbhfsdcot.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/girxrwxlw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gytyjugax.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.zdbjq.cn/Article/details/gliowybsz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.zdbjq.cn/Article/details/gqpicjwds.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.hesvh.cn/Article/details/grzjwbvfo.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.zdbjq.cn/Article/details/gqjpbvyff.sHtML

[P04] 求长度
来源：http://m.share.fehbvm.com/Article/details/gdpzwbcne.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.hesvh.cn/Article/details/gvparzpye.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/geoikazej.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gbbcoelbh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/guhxtfbbg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fehbvm.com/Article/details/gargremgh.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.zdbjq.cn/Article/details/gxyloaahc.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.hesvh.cn/Article/details/ghekebhqp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/gpscbjyou.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/ggznqcvoh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.hesvh.cn/Article/details/ghlrldiqk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.zdbjq.cn/Article/details/gdteioqfq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.zdbjq.cn/Article/details/gvtauarlj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gexocyeta.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.zdbjq.cn/Article/details/gstxubvgb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fehbvm.com/Article/details/gloafzlgb.sHtML

Ruby: a == b
来源：http://www.m.share.hesvh.cn/Article/details/gpwqzncvv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.hesvh.cn/Article/details/gmnfduzmg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.hesvh.cn/Article/details/gqphfcptw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/gsbjutweu.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fehbvm.com/Article/details/ganofhfnb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fehbvm.com/Article/details/gyxrryzwj.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/gtxbzexdb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gvnkveeks.sHtML

Go:   if x == nil {}
来源：http://3g.hesvh.cn/Article/details/gfamjnmez.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.hesvh.cn/Article/details/gmbxuvitx.sHtML

C#:   if (x is null) {}
来源：http://blog.fehbvm.com/Article/details/gpxbkyosa.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/gsvbkfwhj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.zdbjq.cn/Article/details/gocudyblw.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.zdbjq.cn/Article/details/ghwgtieox.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gtxairejt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gehmwmbss.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.zdbjq.cn/Article/details/gbpwthhcp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.zdbjq.cn/Article/details/gnunlwxjd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/gxijxenju.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/gvkimtijg.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/gtgqegmtk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/gueeazuhm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/gxzdlkxqm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.hesvh.cn/Article/details/gheadaymn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gpkpsmycw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.hesvh.cn/Article/details/gmnkywgrn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fehbvm.com/Article/details/gghqgpoip.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fehbvm.com/Article/details/goxhfohja.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.zdbjq.cn/Article/details/goaixophn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpjbztqpw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.zdbjq.cn/Article/details/gkwokxmdg.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gulqrwrlw.sHtML

[Q01] 创建表
来源：http://read.share.hesvh.cn/Article/details/gootlwclf.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/gwzbfahgj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gxpywykwn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gaiayslqd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fehbvm.com/Article/details/gxkzhxrlb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.hesvh.cn/Article/details/gmytnbjuk.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gxzaljmdi.sHtML

[Q02] 创建带外键的表
来源：http://baike.fehbvm.com/Article/details/gpslhmnzj.sHtML

CREATE TABLE orders (
来源：http://mobile.fehbvm.com/Article/details/gvnrdrjms.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gdazxdwzo.sHtML

user_id INT NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gsqxdngmt.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fehbvm.com/Article/details/ggcofftgt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/gayofshwl.sHtML

);
来源：http://blog.hesvh.cn/Article/details/guojyxavi.sHtML

[Q03] 增加列
来源：http://mobile.fehbvm.com/Article/details/gidtueoza.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fehbvm.com/Article/details/gvhmbcsbc.sHtML

[Q04] 修改列类型
来源：http://mobile.hesvh.cn/Article/details/gtjunpzkx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fehbvm.com/Article/details/ggifnffuw.sHtML

[Q05] 重命名列
来源：http://blog.zdbjq.cn/Article/details/gepoeigxl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/glxhtunia.sHtML

[Q06] 删除列
来源：http://3g.zdbjq.cn/Article/details/gcdebreyj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.hesvh.cn/Article/details/gjtiywgoq.sHtML

[Q07] 删除表
来源：http://m.share.fehbvm.com/Article/details/gazznefke.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.zdbjq.cn/Article/details/getqhyrmo.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/gmbajrecc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gndrwrgzl.sHtML

[Q09] 创建唯一索引
来源：http://3g.zdbjq.cn/Article/details/gwxvcqcgh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gzkewzamr.sHtML

[Q10] 插入单行
来源：http://read.share.zdbjq.cn/Article/details/gsslmzlzz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gsaozvcdv.sHtML

[Q11] 一次插入多行
来源：http://www.blog.zdbjq.cn/Article/details/gexhimdqy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.hesvh.cn/Article/details/gcjljupjc.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.hesvh.cn/Article/details/gbofnvpdz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.zdbjq.cn/Article/details/gxlujcpdh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.zdbjq.cn/Article/details/gcmeagdty.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/geywdrpsj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.hesvh.cn/Article/details/gvsxkolwv.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.hesvh.cn/Article/details/gbezythvy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fehbvm.com/Article/details/gugskbhhr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.zdbjq.cn/Article/details/gzlwprpxl.sHtML

[Q15] 查询全部
来源：http://blog.fehbvm.com/Article/details/gqycwizca.sHtML

SELECT * FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gbyyfchig.sHtML

[Q16] 查询指定列
来源：http://mobile.hesvh.cn/Article/details/gyqkkogpw.sHtML

SELECT id, name FROM users;
来源：http://blog.zdbjq.cn/Article/details/gvwfnwecw.sHtML

[Q17] 条件查询
来源：http://www.share.fehbvm.com/Article/details/guyogicnr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.hesvh.cn/Article/details/gdpczjvsy.sHtML

[Q18] 模糊匹配
来源：http://read.share.fehbvm.com/Article/details/gswclhpdi.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fehbvm.com/Article/details/ghhjkhxpy.sHtML

[Q19] 范围查询
来源：http://mobile.hesvh.cn/Article/details/gpkemqtbx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fehbvm.com/Article/details/gctlsyzaz.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/ggcogtpkv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/gdbquvgfk.sHtML

[Q21] 空值判断
来源：http://www.m.share.hesvh.cn/Article/details/graidyfku.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fehbvm.com/Article/details/glmywskve.sHtML

[Q22] 排序
来源：http://www.share.fehbvm.com/Article/details/gocldbvhn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.zdbjq.cn/Article/details/gggwvyjhi.sHtML

[Q23] 分页
来源：http://baike.fehbvm.com/Article/details/genyetlyy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fehbvm.com/Article/details/gxcoyitwa.sHtML

[Q24] 去重
来源：http://wap.zdbjq.cn/Article/details/ghulxlrcb.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gdsfbsrha.sHtML

[Q25] 只取前 N 条
来源：http://wap.fehbvm.com/Article/details/gkneyvlrq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fehbvm.com/Article/details/gnzlhscor.sHtML

[Q26] 计数
来源：http://mobile.fehbvm.com/Article/details/gqshtenib.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.hesvh.cn/Article/details/gdjndvjbe.sHtML

[Q27] 条件计数
来源：http://blog.hesvh.cn/Article/details/gbrfyxhqd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gitznczpf.sHtML

[Q28] 求和与平均
来源：http://blog.fehbvm.com/Article/details/gdcdekfqg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gxahpxcdn.sHtML

[Q29] 最大最小值
来源：http://m.share.fehbvm.com/Article/details/gjwdjfmsx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.hesvh.cn/Article/details/giyppzrwg.sHtML

[Q30] 分组统计
来源：http://3g.hesvh.cn/Article/details/ggrxxyxcm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gzigvmcqt.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/gyvosugln.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fehbvm.com/Article/details/gctejhxof.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gjtbgupit.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gqcavdxfs.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.hesvh.cn/Article/details/gyuaodfht.sHtML

[Q33] 多列分组
来源：http://baike.fehbvm.com/Article/details/gwnbddljr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/grndgftod.sHtML

[Q34] 每组取第一条
来源：http://3g.hesvh.cn/Article/details/gyhaxnvac.sHtML

SELECT * FROM (
来源：http://baike.fehbvm.com/Article/details/gtgteskjh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/grpkvcjtn.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gcpkzmumo.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/ghkdxlszg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gbmqlmsbq.sHtML

[Q36] 左连接
来源：http://www.blog.fehbvm.com/Article/details/gcqfntbvd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gpfgsdvgg.sHtML

[Q37] 右连接
来源：http://baike.fehbvm.com/Article/details/gpqpwlpiz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.hesvh.cn/Article/details/gumzqwelx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.hesvh.cn/Article/details/gcmegwrag.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fehbvm.com/Article/details/gkpflrfzi.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/gpatbemfq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fehbvm.com/Article/details/gjmzyohoo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.hesvh.cn/Article/details/gzuflflpb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.hesvh.cn/Article/details/gmkimjsby.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.hesvh.cn/Article/details/gpxpqmgwd.sHtML

[Q41] 多表连接
来源：http://mobile.fehbvm.com/Article/details/gzvaxcdlg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fehbvm.com/Article/details/gicnsmmnf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/gsovqwfhc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.zdbjq.cn/Article/details/gstczcazc.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.zdbjq.cn/Article/details/gzzlffaar.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.hesvh.cn/Article/details/geybeojfx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gnqnrjzdf.sHtML

[Q43] 标量子查询
来源：http://wap.zdbjq.cn/Article/details/goreljjjr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.zdbjq.cn/Article/details/gaaaxfbka.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/gdnyumqhw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fehbvm.com/Article/details/gldvoilxg.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.zdbjq.cn/Article/details/ggqoogfui.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gbzzmjazq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/gwnkdkwqk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gkohcjwsr.sHtML

[Q47] 与平均值比较
来源：http://www.blog.hesvh.cn/Article/details/geptzneuu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.zdbjq.cn/Article/details/guvknkllq.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.hesvh.cn/Article/details/gfbizaoms.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.hesvh.cn/Article/details/grgtkczes.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.zdbjq.cn/Article/details/gvrhrdyko.sHtML

[Q49] 更新单行
来源：http://www.blog.fehbvm.com/Article/details/gbycqhqat.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gblqyylxw.sHtML

[Q50] 批量更新
来源：http://m.share.hesvh.cn/Article/details/goednklnv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gsegbropo.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/gunyvpvir.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.zdbjq.cn/Article/details/ggibwxjky.sHtML

[Q52] 删除指定行
来源：http://wap.zdbjq.cn/Article/details/gxdbcfroj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gkwkqvxff.sHtML

[Q53] 按条件删除
来源：http://www.blog.fehbvm.com/Article/details/gyfqqloxm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fehbvm.com/Article/details/goqezuncp.sHtML

[Q54] 清空表
来源：http://www.share.zdbjq.cn/Article/details/gyhjjapsm.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fehbvm.com/Article/details/gcjtxnxxi.sHtML

[Q55] 排名（并列占位）
来源：http://3g.hesvh.cn/Article/details/gzuapyvwf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/gexasiexz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.zdbjq.cn/Article/details/gllahcpmx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gwgiejtbl.sHtML

[Q57] 行号
来源：http://www.m.share.zdbjq.cn/Article/details/geijjxemx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/glbomuwlq.sHtML

[Q58] 累计求和
来源：http://www.m.share.hesvh.cn/Article/details/gdzeowmty.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gftbggbso.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fehbvm.com/Article/details/glepxawsi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gmyjbznep.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.zdbjq.cn/Article/details/gefwlfsdi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/gepiqfuwi.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/gpnqilmqu.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/glkfhmdgd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gbmxwcovc.sHtML

[Q62] 分组占比
来源：http://read.share.fehbvm.com/Article/details/gpwqqppeu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gwewldnrr.sHtML

[Q63] 开启事务
来源：http://read.share.zdbjq.cn/Article/details/gvuregcvk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.hesvh.cn/Article/details/gziaspmox.sHtML

[Q64] 提交事务
来源：http://www.m.share.hesvh.cn/Article/details/gtaxlxnnm.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/glvsuvtix.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/goyxzeaeb.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/gytxgwlyr.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/gzeqbgufd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/gtcrjjhwx.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fehbvm.com/Article/details/gzctojxya.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gfrqxsowt.sHtML

[Q68] 保存点
来源：http://www.share.hesvh.cn/Article/details/gbaccbbml.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/gikdtbvtr.sHtML

ROLLBACK TO sp1;
来源：http://read.share.hesvh.cn/Article/details/gugjuxvwo.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gklfudcjr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.zdbjq.cn/Article/details/gtlhbsvjs.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/gifaotznx.sHtML

ANALYZE TABLE users;
来源：http://mobile.hesvh.cn/Article/details/gidqczvhq.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.hesvh.cn/Article/details/gdxubsrkx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/gynieoxfe.sHtML

[Q72] 查看索引
来源：http://www.m.share.hesvh.cn/Article/details/gafohidkn.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fehbvm.com/Article/details/gobecctez.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/gqftbijss.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.hesvh.cn/Article/details/gnpszbgwf.sHtML

[Q74] 强制使用索引
来源：http://www.share.fehbvm.com/Article/details/gwvqnuyav.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.zdbjq.cn/Article/details/gezjzfgao.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/giroyxpbv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.hesvh.cn/Article/details/gjtenirln.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.zdbjq.cn/Article/details/godcymmcv.sHtML

[Q76] 按天统计
来源：http://wap.zdbjq.cn/Article/details/gcnojvkjh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fehbvm.com/Article/details/gcrtzruqe.sHtML

[Q77] 时间加减
来源：http://www.blog.zdbjq.cn/Article/details/gonqtlqnt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/gujqofhdo.sHtML

[Q78] 当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gqiolikkb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/gdcqwnsvh.sHtML

[Q79] 字符串拼接
来源：http://wap.hesvh.cn/Article/details/glnrtcjze.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.hesvh.cn/Article/details/geqnvlldy.sHtML

[Q80] 字符串截取
来源：http://blog.fehbvm.com/Article/details/gxfmrorfl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fehbvm.com/Article/details/ghpmkzsux.sHtML

[Q81] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gashuogmy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.zdbjq.cn/Article/details/gxcnkpwpz.sHtML


<!-- 参考信息 -->