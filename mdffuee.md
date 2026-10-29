代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/gyqgonnbs.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/gwpadlozb.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.zdbjq.cn/Article/details/gglhwfmmw.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.zdbjq.cn/Article/details/gjjmcrbfd.sHtML

[O02] 使用线程池
来源：http://www.share.hesvh.cn/Article/details/gbvrenhgf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/gaflflxrg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.hesvh.cn/Article/details/glamstdms.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gxjhtlwiv.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gwlwadtur.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fehbvm.com/Article/details/gpnwclxfn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.zdbjq.cn/Article/details/ggdzfhjuu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gjnbtuyfl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/gzgkkxttz.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/gbukgrmuh.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/grhtbuega.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/gcpguuujh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/gbydcsoei.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gydiifstb.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/grqgoixrd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/gyxgqhgxl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gpbpjmhha.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gcoxwhxaa.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/gboihvhod.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.zdbjq.cn/Article/details/gxnfkaymu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fehbvm.com/Article/details/gvfnegosr.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gluraedug.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/grcanhgna.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fehbvm.com/Article/details/gykxqnefd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fehbvm.com/Article/details/guipiwmii.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/gffyzoezq.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.hesvh.cn/Article/details/gwztzrtvy.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.hesvh.cn/Article/details/goxunrmwo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.hesvh.cn/Article/details/glunkzorr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/gfsrpdcdg.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gubqabola.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gqtjzsuhz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.hesvh.cn/Article/details/gjntpaygi.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.hesvh.cn/Article/details/gsxiqqppw.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/geieehtpj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fehbvm.com/Article/details/gitqnjklp.sHtML

[O06] 使用进程池
来源：http://read.share.hesvh.cn/Article/details/gfqvakjfv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.zdbjq.cn/Article/details/gngvnzzgm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.zdbjq.cn/Article/details/gwbpfhwbd.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gakwmjdlr.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/glosrqoou.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.hesvh.cn/Article/details/gfecfyirw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fehbvm.com/Article/details/gahkodifa.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/gfumpucbe.sHtML

C#:   Parallel.For
来源：http://www.m.share.zdbjq.cn/Article/details/gpvequjec.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/guaejxfmn.sHtML

P. 常用工具函数
来源：http://m.share.zdbjq.cn/Article/details/gtbyvyrpc.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxjgujrwv.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/ghijbldim.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fehbvm.com/Article/details/gaepgmgzw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gattkwmfv.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/grhgysfjb.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gkflnxwjq.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/grahflslc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/gihlhavdt.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/gaaivmxdy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.zdbjq.cn/Article/details/gwlahtqtp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/govqjqaik.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/gvqtrdein.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/gxnjfsyjo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.hesvh.cn/Article/details/gdcirrdym.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/gbfvyqimy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.zdbjq.cn/Article/details/gfmsqeifr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/gsernrujx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fehbvm.com/Article/details/geaeegkyq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/gjgisxrcm.sHtML

[P03] 生成短随机字符串
来源：http://wap.hesvh.cn/Article/details/gtixfotwn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.hesvh.cn/Article/details/gprayvnrb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fehbvm.com/Article/details/ghkgthkue.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gluwuyedh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gjgqlmtpt.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/gmwavxuud.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.hesvh.cn/Article/details/gyuxwkcbd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gpumnzgfq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/gqcktykfz.sHtML

[P04] 求长度
来源：http://wap.fehbvm.com/Article/details/ghmbvrnml.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.zdbjq.cn/Article/details/gxkgtavcr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gziobmlvf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gqieaxrgk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gaxijldgb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gvqqjptiq.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.zdbjq.cn/Article/details/golgjplqz.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/gobthwqju.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/gtcdsxpfv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fehbvm.com/Article/details/grrnfurek.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.hesvh.cn/Article/details/gfdphgktg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fehbvm.com/Article/details/goxgfrbak.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.zdbjq.cn/Article/details/gojzvpazm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gsanzoyec.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.hesvh.cn/Article/details/gbegvslyq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fehbvm.com/Article/details/gfjqdkfsj.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/gxullmqxk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fehbvm.com/Article/details/goqwxqoby.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fehbvm.com/Article/details/gydqaddwv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/gfkudhfho.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.hesvh.cn/Article/details/gqbprcunq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/gunfhryez.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gjkkmnypt.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gyjtmuwhs.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/ghepoajgz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/gzxivbcnz.sHtML

C#:   if (x is null) {}
来源：http://3g.zdbjq.cn/Article/details/gpmimhfqf.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/gfokcsqnv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fehbvm.com/Article/details/gxnkzxemw.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.hesvh.cn/Article/details/gkcrzynba.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gssmpuqni.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/guoavjtdh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/gsanytocs.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.zdbjq.cn/Article/details/gjnnoxgqd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fehbvm.com/Article/details/gqzqaerrg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.hesvh.cn/Article/details/gfuzvuuuz.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/gdfewtukj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.zdbjq.cn/Article/details/gvwktaewr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.hesvh.cn/Article/details/gazdzejgq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.hesvh.cn/Article/details/glzpmbugc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gznchsrof.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fehbvm.com/Article/details/gevqtgjrv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fehbvm.com/Article/details/gzinqyvol.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.hesvh.cn/Article/details/gaolddejk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/gavbtauho.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcarjzqpt.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.zdbjq.cn/Article/details/gbgiiubxi.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwxgsshbg.sHtML

[Q01] 创建表
来源：http://read.share.hesvh.cn/Article/details/gudzmrbph.sHtML

CREATE TABLE users (
来源：http://wap.zdbjq.cn/Article/details/gukauedim.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gsczyszqx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gfplwhblp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fehbvm.com/Article/details/gjwhrkrvn.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.zdbjq.cn/Article/details/gqsugpstn.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gixetlupf.sHtML

[Q02] 创建带外键的表
来源：http://read.share.hesvh.cn/Article/details/gyhkzvxaj.sHtML

CREATE TABLE orders (
来源：http://read.share.fehbvm.com/Article/details/gsreqrtiu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gbpujftmp.sHtML

user_id INT NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gzksecbsi.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fehbvm.com/Article/details/gnvwbodch.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.hesvh.cn/Article/details/gqosyslfo.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gtixuhhlk.sHtML

[Q03] 增加列
来源：http://read.share.zdbjq.cn/Article/details/grbjsqihs.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fehbvm.com/Article/details/gwkjxvdna.sHtML

[Q04] 修改列类型
来源：http://mobile.fehbvm.com/Article/details/ghpcdtukx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/ggffuhoup.sHtML

[Q05] 重命名列
来源：http://m.share.fehbvm.com/Article/details/govkpagjs.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.zdbjq.cn/Article/details/gpzzjaeyj.sHtML

[Q06] 删除列
来源：http://m.share.zdbjq.cn/Article/details/gpkppvtmo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fehbvm.com/Article/details/gefuavfdh.sHtML

[Q07] 删除表
来源：http://www.m.share.fehbvm.com/Article/details/gkeuievld.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fehbvm.com/Article/details/grvgetflz.sHtML

[Q08] 创建普通索引
来源：http://baike.hesvh.cn/Article/details/gndbzrnro.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gytxcfwjn.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.zdbjq.cn/Article/details/gydysoddr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gskfmpgsv.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/gtlyjcdnr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.hesvh.cn/Article/details/gdotloptl.sHtML

[Q11] 一次插入多行
来源：http://blog.zdbjq.cn/Article/details/gjqxqxfyg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gfkpaijmv.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.hesvh.cn/Article/details/gmfcakctg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.zdbjq.cn/Article/details/gdatbsnnq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fehbvm.com/Article/details/gnhzveqrm.sHtML

[Q13] 忽略重复插入
来源：http://baike.zdbjq.cn/Article/details/gevndtpdr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gmnmpzncc.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.zdbjq.cn/Article/details/gooykpgdq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fehbvm.com/Article/details/gzjbyuhwy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fehbvm.com/Article/details/goxiudxxe.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/gbjqyokwn.sHtML

SELECT * FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/goyqikjnk.sHtML

[Q16] 查询指定列
来源：http://read.share.hesvh.cn/Article/details/gummypdhr.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ghgjpjgho.sHtML

[Q17] 条件查询
来源：http://m.share.hesvh.cn/Article/details/gckytswst.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fehbvm.com/Article/details/gdcoqfrgx.sHtML

[Q18] 模糊匹配
来源：http://www.share.hesvh.cn/Article/details/gaujxozig.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.zdbjq.cn/Article/details/gymfhjoat.sHtML

[Q19] 范围查询
来源：http://mobile.hesvh.cn/Article/details/gxbluvqpg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fehbvm.com/Article/details/gqivuejur.sHtML

[Q20] IN 列表
来源：http://www.blog.fehbvm.com/Article/details/gvkgdgach.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fehbvm.com/Article/details/gaeesotgc.sHtML

[Q21] 空值判断
来源：http://baike.hesvh.cn/Article/details/galkcrkgk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.hesvh.cn/Article/details/gcyzdpbqj.sHtML

[Q22] 排序
来源：http://www.share.zdbjq.cn/Article/details/glbuyeyfr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.hesvh.cn/Article/details/ghxwzhivw.sHtML

[Q23] 分页
来源：http://mobile.zdbjq.cn/Article/details/ginqudpmv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.zdbjq.cn/Article/details/gqvrsywsv.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/gubvfyuer.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.hesvh.cn/Article/details/gqvrxdoji.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fehbvm.com/Article/details/gfdvkwukh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fehbvm.com/Article/details/ghasikugo.sHtML

[Q26] 计数
来源：http://www.share.zdbjq.cn/Article/details/gdzhrrsho.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gbuavxiol.sHtML

[Q27] 条件计数
来源：http://m.share.fehbvm.com/Article/details/gwvpybvzp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fehbvm.com/Article/details/gslgoktza.sHtML

[Q28] 求和与平均
来源：http://www.share.hesvh.cn/Article/details/gyncuzawu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gswshhmva.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/gpttabjuq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fehbvm.com/Article/details/gqvofvoij.sHtML

[Q30] 分组统计
来源：http://blog.hesvh.cn/Article/details/grerhlpel.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gwgugcdmc.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/gyykpxstn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gvrogkbgn.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/goglytxzd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gcafymxqc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/ghhldhhrm.sHtML

[Q33] 多列分组
来源：http://www.m.share.fehbvm.com/Article/details/gyjfcyvdd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fehbvm.com/Article/details/gogdcohdz.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/gaglkybyd.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/ggziyvahk.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fehbvm.com/Article/details/gfoerdrne.sHtML

) t WHERE rn = 1;
来源：http://wap.zdbjq.cn/Article/details/gogcliwsh.sHtML

[Q35] 内连接
来源：http://mobile.zdbjq.cn/Article/details/gewyxcieo.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gohwlfyhx.sHtML

[Q36] 左连接
来源：http://read.share.hesvh.cn/Article/details/gjxskesge.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gycqksfmu.sHtML

[Q37] 右连接
来源：http://www.blog.zdbjq.cn/Article/details/gtebuhoyf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/glbtbtpfn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.zdbjq.cn/Article/details/gskjetrmz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fehbvm.com/Article/details/gwbynudnh.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.hesvh.cn/Article/details/gnxzuugmy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.zdbjq.cn/Article/details/gsawjszfu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/guwroqaov.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.hesvh.cn/Article/details/gwwkioucg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fehbvm.com/Article/details/gwkqoetwn.sHtML

[Q41] 多表连接
来源：http://www.blog.hesvh.cn/Article/details/govdwvyeo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.hesvh.cn/Article/details/glcnvglwi.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/gzzkduxin.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/gikciqabo.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fehbvm.com/Article/details/gltsulnyo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.zdbjq.cn/Article/details/gbbavbpms.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fehbvm.com/Article/details/gantxynhh.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/ggemwhjbv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.zdbjq.cn/Article/details/gbctclomf.sHtML

[Q44] IN 子查询
来源：http://wap.fehbvm.com/Article/details/gcwsvpxer.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.hesvh.cn/Article/details/gzrnimuin.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fehbvm.com/Article/details/gxjktnaph.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gcolauitr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/gtaqzyurb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gnijxzxfv.sHtML

[Q47] 与平均值比较
来源：http://www.share.fehbvm.com/Article/details/gtthlpztt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.zdbjq.cn/Article/details/ggoupabxf.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fehbvm.com/Article/details/ggoieklxv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.hesvh.cn/Article/details/gatkyqnpr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.zdbjq.cn/Article/details/ghuyhlmde.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/gmuhqpgcv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/ginoizloq.sHtML

[Q50] 批量更新
来源：http://blog.fehbvm.com/Article/details/gzqaqfzsl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fehbvm.com/Article/details/gzfdoxgif.sHtML

[Q51] 用子查询更新
来源：http://m.share.zdbjq.cn/Article/details/ggyswsngh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fehbvm.com/Article/details/gfwurewzn.sHtML

[Q52] 删除指定行
来源：http://www.m.share.hesvh.cn/Article/details/gajanyswo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gjhmkvayu.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/gbvrpgpmj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fehbvm.com/Article/details/gdpanoppw.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/gbugnaeys.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/grglquoqf.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gdvfymehh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gbssttvrf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.hesvh.cn/Article/details/ghhrmboon.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gjoxfvurl.sHtML

[Q57] 行号
来源：http://www.m.share.zdbjq.cn/Article/details/gmnmxhicr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.hesvh.cn/Article/details/gwevwsksh.sHtML

[Q58] 累计求和
来源：http://m.share.hesvh.cn/Article/details/gsrmtlrww.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gfdsgayzc.sHtML

[Q59] 分组内累计
来源：http://www.share.zdbjq.cn/Article/details/grztyszgw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gvbgiffyw.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.zdbjq.cn/Article/details/gttzwoito.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.zdbjq.cn/Article/details/gucontvna.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gyljjdfwx.sHtML

[Q61] 移动平均
来源：http://mobile.zdbjq.cn/Article/details/gmodeaiem.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gtwxcnahd.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/gzkkkaaeg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gfelbjdxd.sHtML

[Q63] 开启事务
来源：http://www.m.share.zdbjq.cn/Article/details/gohlyzuqb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/gkrwogghh.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/gvpxuwumo.sHtML

COMMIT;
来源：http://www.m.share.hesvh.cn/Article/details/gctpgaozj.sHtML

[Q65] 回滚事务
来源：http://mobile.fehbvm.com/Article/details/gieautupt.sHtML

ROLLBACK;
来源：http://www.share.hesvh.cn/Article/details/gzodgqwmk.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/ghawbzwmq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.zdbjq.cn/Article/details/gwmqfwmbj.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.zdbjq.cn/Article/details/gzkzjdvhz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.zdbjq.cn/Article/details/gghoaccjn.sHtML

[Q68] 保存点
来源：http://blog.fehbvm.com/Article/details/gfkpbilvh.sHtML

SAVEPOINT sp1;
来源：http://read.share.fehbvm.com/Article/details/gxaajjfis.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/gqtognnzw.sHtML

[Q69] 查看执行计划
来源：http://wap.fehbvm.com/Article/details/gcqijhdwy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.zdbjq.cn/Article/details/gjkoshnxd.sHtML

[Q70] 更新统计信息
来源：http://www.share.zdbjq.cn/Article/details/gyaxbgbtz.sHtML

ANALYZE TABLE users;
来源：http://3g.fehbvm.com/Article/details/gtmnelaut.sHtML

[Q71] 查看建表语句
来源：http://read.share.zdbjq.cn/Article/details/gmryfnqiv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fehbvm.com/Article/details/gwuhzlyjq.sHtML

[Q72] 查看索引
来源：http://baike.fehbvm.com/Article/details/gteuoawxl.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gebiopskj.sHtML

[Q73] 查看表状态
来源：http://www.blog.zdbjq.cn/Article/details/gckwkyxzs.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gcfipauyj.sHtML

[Q74] 强制使用索引
来源：http://blog.hesvh.cn/Article/details/grxfvvyzz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.hesvh.cn/Article/details/gkggeziki.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gxyutvuzs.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fehbvm.com/Article/details/gqzqqstxw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fehbvm.com/Article/details/gtkswxkuo.sHtML


<!-- 参考信息 -->