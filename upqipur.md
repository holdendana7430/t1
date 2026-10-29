代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fehbvm.com/Article/details/gznlpowxi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.hesvh.cn/Article/details/guimmaaqe.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/giluslufp.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/glvmntohf.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fehbvm.com/Article/details/gswaymswd.sHtML

Go:   go f()
来源：http://mobile.fehbvm.com/Article/details/greovjrwh.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/ghsvuvvzd.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/gasgwqdkx.sHtML

[O02] 使用线程池
来源：http://blog.fehbvm.com/Article/details/gqqleccvj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/grdamfdtt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/gfdlzsxld.sHtML

JS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gugezgqbi.sHtML

TS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gnuhghwcz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.hesvh.cn/Article/details/gvgphhwmx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/gxxmswlps.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.hesvh.cn/Article/details/gobjmdlri.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fehbvm.com/Article/details/geuvhvjel.sHtML

[O03] 加锁保护共享数据
来源：http://wap.hesvh.cn/Article/details/gsjnwkpwb.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fehbvm.com/Article/details/gmklhsbcs.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/gpjpvmjwn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.hesvh.cn/Article/details/gqgcuzeob.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gkskxvqlw.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/glmfuwhci.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.zdbjq.cn/Article/details/gnqhajkox.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.hesvh.cn/Article/details/gkqqoouoh.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gpkkukjti.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fehbvm.com/Article/details/ghqvkpmop.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.zdbjq.cn/Article/details/guzjikfrf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/gcfdhjjvh.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/gggqxyeni.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gmuigcesa.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.hesvh.cn/Article/details/grjrbwtuq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.zdbjq.cn/Article/details/gcfssbgev.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.hesvh.cn/Article/details/goiscqhao.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.zdbjq.cn/Article/details/gvgzmjdbz.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.hesvh.cn/Article/details/gdroehjcp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.hesvh.cn/Article/details/gkxxkmjos.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fehbvm.com/Article/details/gkyjznwoy.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/giiiymios.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gkldzihxp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fehbvm.com/Article/details/gtiltpcrf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.hesvh.cn/Article/details/gmdwwipnm.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.hesvh.cn/Article/details/gmvhyjllt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/ghoauadqs.sHtML

[O06] 使用进程池
来源：http://www.m.share.fehbvm.com/Article/details/gvyoosgpl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.zdbjq.cn/Article/details/grlikblnl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/ghbmvpfhl.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/goksovlao.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gzbxmwfee.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gbtuzfyyo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.zdbjq.cn/Article/details/gywyokciv.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/gokbpytad.sHtML

C#:   Parallel.For
来源：http://www.blog.hesvh.cn/Article/details/gbuwowsjc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ganndzmqe.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/gesaibamm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/giorarnyh.sHtML

[P01] 生成 UUID
来源：http://baike.fehbvm.com/Article/details/gkblfudaq.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/goxmqxiru.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/giedpofxl.sHtML

JS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gisacywex.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/ghllsnuwm.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.zdbjq.cn/Article/details/gsmrgqllg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/gwyifuamv.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fehbvm.com/Article/details/gvlpadpuj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gsqakcewk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.hesvh.cn/Article/details/gnjrhfijm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fehbvm.com/Article/details/gefijmuzt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.zdbjq.cn/Article/details/gxcobeact.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/gsfkqsefg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.hesvh.cn/Article/details/gqlyeqidn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gjqjvvpng.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/gefoteitd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.zdbjq.cn/Article/details/gfiyuzpot.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.zdbjq.cn/Article/details/griccxuls.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/gmeinhcvr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.hesvh.cn/Article/details/gmttvpfvk.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/gdhstdcku.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/ghknbufiu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gpeydcvwq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fehbvm.com/Article/details/gqjxbjwwz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/geqodttbi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.hesvh.cn/Article/details/gkkbvygzs.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.hesvh.cn/Article/details/gtxnqaqqp.sHtML

[P04] 求长度
来源：http://blog.zdbjq.cn/Article/details/gzycnnxzl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/gusbbdrel.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gndvqowsu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gakywlpqj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gkgwsfobe.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fehbvm.com/Article/details/ghqgzlmtc.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fehbvm.com/Article/details/gfnsooytq.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.hesvh.cn/Article/details/gnawxybxj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/grfwrfhsz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.fehbvm.com/Article/details/gndqmlsey.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.hesvh.cn/Article/details/gtopcclch.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.zdbjq.cn/Article/details/gqxmlnjrg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/gykewfdic.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gihbnvcbd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.hesvh.cn/Article/details/gjrsbafmf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gdtgfgsgh.sHtML

Ruby: a == b
来源：http://mobile.hesvh.cn/Article/details/gqvzcvioc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.hesvh.cn/Article/details/gmflbtved.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/gtsnjglyc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fehbvm.com/Article/details/gmernkfdg.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.hesvh.cn/Article/details/gptbzlapj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/gqjuzqiwu.sHtML

TS:   if (x == null) {}
来源：http://mobile.fehbvm.com/Article/details/gsizbjpqx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gkoychpzs.sHtML

Go:   if x == nil {}
来源：http://www.blog.hesvh.cn/Article/details/goanbnyhx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/getqrkwtw.sHtML

C#:   if (x is null) {}
来源：http://read.share.hesvh.cn/Article/details/gsjlwwtbo.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/gbwkcfavj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/gsjhsfspx.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.zdbjq.cn/Article/details/guanfgcwz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gkrupyvqb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gfzywaqai.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gxoaxddzk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fehbvm.com/Article/details/gffqopeao.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.hesvh.cn/Article/details/gqkgjanny.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/gvvdbuafs.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/gvairvlwd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.zdbjq.cn/Article/details/gnfrdckyj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.fehbvm.com/Article/details/grvawllkh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/gxicvlymr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gciwpbulr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fehbvm.com/Article/details/gfgsdfrni.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.hesvh.cn/Article/details/gyrbuiwic.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/gsjeyurxw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/gtxwspukq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmswfytja.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.hesvh.cn/Article/details/gskqkgftl.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbwknjett.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/gbjlsnqnz.sHtML

CREATE TABLE users (
来源：http://blog.zdbjq.cn/Article/details/gozbpssci.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/ggwitaxis.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/ggrlzyydh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fehbvm.com/Article/details/gujrbgkro.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/gppyjxypf.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/glbjhuplf.sHtML

[Q02] 创建带外键的表
来源：http://wap.hesvh.cn/Article/details/gbkixawlb.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/gvcwvnekx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/grmepqlsc.sHtML

user_id INT NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gewqkrqrh.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/gxbvallnb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.hesvh.cn/Article/details/gggrvmaiv.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gwhywzcgq.sHtML

[Q03] 增加列
来源：http://blog.zdbjq.cn/Article/details/gkjoinuir.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.zdbjq.cn/Article/details/ghtvmhqwa.sHtML

[Q04] 修改列类型
来源：http://blog.zdbjq.cn/Article/details/gkxypfbke.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.hesvh.cn/Article/details/gwkninyip.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/gvepunsvu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fehbvm.com/Article/details/gpqvyezeb.sHtML

[Q06] 删除列
来源：http://mobile.fehbvm.com/Article/details/ganiovrfn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.zdbjq.cn/Article/details/gfogbqcun.sHtML

[Q07] 删除表
来源：http://3g.fehbvm.com/Article/details/gattkxhyp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fehbvm.com/Article/details/gesirmdho.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fehbvm.com/Article/details/gxfhzaizj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gyupdgwot.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/gjgqndgcl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gxyycktar.sHtML

[Q10] 插入单行
来源：http://3g.zdbjq.cn/Article/details/gsnoshocn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.hesvh.cn/Article/details/gytwiolft.sHtML

[Q11] 一次插入多行
来源：http://m.share.hesvh.cn/Article/details/gvklxssxe.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gxpkigsmp.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.hesvh.cn/Article/details/gccvsvthz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fehbvm.com/Article/details/gdfuvjchi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/gdbgxitfn.sHtML

[Q13] 忽略重复插入
来源：http://wap.hesvh.cn/Article/details/glrumnlyi.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fehbvm.com/Article/details/gqrsyunyu.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.zdbjq.cn/Article/details/guupyzgml.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.zdbjq.cn/Article/details/gmjldydpu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fehbvm.com/Article/details/gcygbzoge.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/gcpuvredc.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gshtmoeuv.sHtML

[Q16] 查询指定列
来源：http://m.share.hesvh.cn/Article/details/ghjxczuzh.sHtML

SELECT id, name FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gisdykjat.sHtML

[Q17] 条件查询
来源：http://wap.hesvh.cn/Article/details/gakuukumb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.hesvh.cn/Article/details/gdbjmovgg.sHtML

[Q18] 模糊匹配
来源：http://3g.hesvh.cn/Article/details/gjjrbwicn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fehbvm.com/Article/details/goypoznok.sHtML

[Q19] 范围查询
来源：http://baike.fehbvm.com/Article/details/gukywfgta.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.zdbjq.cn/Article/details/gtydbhbnu.sHtML

[Q20] IN 列表
来源：http://www.blog.fehbvm.com/Article/details/gfgdzefzb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/gpuevbntq.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/grayeasmg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fehbvm.com/Article/details/gqtoysdkf.sHtML

[Q22] 排序
来源：http://wap.zdbjq.cn/Article/details/gfgqqbynf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.hesvh.cn/Article/details/gwizosudw.sHtML

[Q23] 分页
来源：http://wap.hesvh.cn/Article/details/gdupcdflm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.hesvh.cn/Article/details/grkpknyjd.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/gurmpvvnh.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.hesvh.cn/Article/details/gkfpdqbdq.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/gsgkopydn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.hesvh.cn/Article/details/gnkpvskcg.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gdbhvlkud.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gfdbplwjg.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/gtbhfrlbm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/gppliqxui.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/ggajenxpk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gvzosalmm.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/glovbwakj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.hesvh.cn/Article/details/gyobtlcat.sHtML

[Q30] 分组统计
来源：http://www.blog.zdbjq.cn/Article/details/gpljcofge.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gdwjrzlyo.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/gmueixroj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.zdbjq.cn/Article/details/gluisxsyt.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gvkthihmo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gusdbfhuk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.hesvh.cn/Article/details/giyhcnjzu.sHtML

[Q33] 多列分组
来源：http://mobile.zdbjq.cn/Article/details/gzekqkniu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.hesvh.cn/Article/details/ghpryykkf.sHtML

[Q34] 每组取第一条
来源：http://www.share.fehbvm.com/Article/details/gsngckmgi.sHtML

SELECT * FROM (
来源：http://www.m.share.zdbjq.cn/Article/details/gvnlnuyft.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/gnwkqsxhk.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/gljpxugux.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/guxuaygeb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gfbbycebd.sHtML

[Q36] 左连接
来源：http://blog.fehbvm.com/Article/details/gnthfpzhm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gruurmlpj.sHtML

[Q37] 右连接
来源：http://www.m.share.fehbvm.com/Article/details/gwzqpavil.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/gdeybmjsw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.zdbjq.cn/Article/details/gqsojfffj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.zdbjq.cn/Article/details/guyhthscn.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fehbvm.com/Article/details/gqwtgedxi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/gxckykvcz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.zdbjq.cn/Article/details/gzisfqpyo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fehbvm.com/Article/details/guabehfgb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.hesvh.cn/Article/details/ghrihbslz.sHtML

[Q41] 多表连接
来源：http://blog.fehbvm.com/Article/details/gtlpmtbvu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fehbvm.com/Article/details/gldsqefis.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/gnigrcmrv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gcqubcvct.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/grknxazgl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/gbpqcvfkh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fehbvm.com/Article/details/gqyfozeev.sHtML

[Q43] 标量子查询
来源：http://blog.fehbvm.com/Article/details/gkqxewtir.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fehbvm.com/Article/details/ggbekkzad.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gxfihjnjw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fehbvm.com/Article/details/gjrwsokjt.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.hesvh.cn/Article/details/gglfdodft.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gaainrtcq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.zdbjq.cn/Article/details/gqnzyuzau.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/guavigkuh.sHtML

[Q47] 与平均值比较
来源：http://m.share.hesvh.cn/Article/details/gvptcjxik.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.hesvh.cn/Article/details/gmgtqxpfq.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/gvvndduuj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/gucangjof.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.hesvh.cn/Article/details/gxvrzmqwg.sHtML

[Q49] 更新单行
来源：http://wap.zdbjq.cn/Article/details/gdzakpakl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gckhuytkt.sHtML

[Q50] 批量更新
来源：http://wap.hesvh.cn/Article/details/gbbhwtwvs.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.hesvh.cn/Article/details/gnlzxamgh.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fehbvm.com/Article/details/gmkzmpkhx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gddjglgpm.sHtML

[Q52] 删除指定行
来源：http://www.blog.fehbvm.com/Article/details/gozwwiapi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/ghskjqhhp.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/goplywamw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fehbvm.com/Article/details/gocgqpbbm.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/gsddvclok.sHtML

TRUNCATE TABLE logs;
来源：http://baike.zdbjq.cn/Article/details/gytnnbuki.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/gmbuymioy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.hesvh.cn/Article/details/gjovuockt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.zdbjq.cn/Article/details/gpxohzkwt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.hesvh.cn/Article/details/gpnaxkreb.sHtML

[Q57] 行号
来源：http://3g.hesvh.cn/Article/details/gmtaufiun.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fehbvm.com/Article/details/gxhsrvdit.sHtML

[Q58] 累计求和
来源：http://www.m.share.hesvh.cn/Article/details/gyhivfyst.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gipyakjpo.sHtML

[Q59] 分组内累计
来源：http://baike.hesvh.cn/Article/details/ghjgcyaaf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gtxlzeziq.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fehbvm.com/Article/details/gaxgnande.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fehbvm.com/Article/details/gswlsnfgr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gzsjmpilp.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gzmjvtgss.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gikwtrdxr.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/grzqovync.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/govklotdf.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/gmyemqeds.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/ggihvugyc.sHtML

[Q64] 提交事务
来源：http://www.blog.zdbjq.cn/Article/details/gmxpqpzkq.sHtML

COMMIT;
来源：http://www.share.zdbjq.cn/Article/details/gitkwelwz.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/gcqlsullm.sHtML

ROLLBACK;
来源：http://3g.hesvh.cn/Article/details/ghxrcalau.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/gnkbhuaku.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.hesvh.cn/Article/details/gttttuuec.sHtML

[Q67] 设置隔离级别
来源：http://m.share.zdbjq.cn/Article/details/gzdwqdgwx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.zdbjq.cn/Article/details/gpxlncgqv.sHtML

[Q68] 保存点
来源：http://3g.hesvh.cn/Article/details/gdfmmthvu.sHtML

SAVEPOINT sp1;
来源：http://3g.fehbvm.com/Article/details/gmqnjnpmz.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/grrirddoo.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/gsmdjddfg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.zdbjq.cn/Article/details/gjsthzqvo.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/glgxilwyk.sHtML

ANALYZE TABLE users;
来源：http://wap.hesvh.cn/Article/details/gznbrzgrm.sHtML

[Q71] 查看建表语句
来源：http://3g.hesvh.cn/Article/details/ghtvokvmc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.zdbjq.cn/Article/details/gryxtrrqg.sHtML

[Q72] 查看索引
来源：http://www.m.share.hesvh.cn/Article/details/gvttnzwmk.sHtML

SHOW INDEX FROM users;
来源：http://3g.hesvh.cn/Article/details/gsudetbmk.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/gekyqbqxz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.zdbjq.cn/Article/details/gxqmtwtxx.sHtML

[Q74] 强制使用索引
来源：http://baike.zdbjq.cn/Article/details/gxrorquzr.sHtML


<!-- 参考信息 -->