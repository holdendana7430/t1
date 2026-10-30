代发 wailian999

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqehuccgs.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/glymqhtor.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gohbgkftb.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/ggxkfefci.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/gzfhynxoh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.zdbjq.cn/Article/details/gyfosqsix.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.zdbjq.cn/Article/details/gdecjznzb.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gkhugcyuc.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gnvgfcsfp.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/grttuvyzh.sHtML

Ruby: Thread.new { f }
来源：http://www.share.hesvh.cn/Article/details/giqwnsnrq.sHtML

C#:   Task.Run(() => F());
来源：http://3g.zdbjq.cn/Article/details/ggwbifeso.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/gjphshjar.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/gkrytrdwc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fehbvm.com/Article/details/gccfyxyyd.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gioxcqanv.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gcdbrlivn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/gaopbgjgr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.zdbjq.cn/Article/details/gvzxkaroz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gbggvsuhf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.zdbjq.cn/Article/details/gjcpacxpz.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/gqwimvcxj.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/gtrvlarif.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/gjpllafii.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.zdbjq.cn/Article/details/gdqibrdqq.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gjxlynibz.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gymuvtnpb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/gyxtoxkkz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gxkigpjgf.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/ggcygpmfr.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/gzstnczjo.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.zdbjq.cn/Article/details/gcmymwlkl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/grypedjtn.sHtML

JS:   async function f() { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gmvbhaiex.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gjahamkjf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.zdbjq.cn/Article/details/gwbnzzlcp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fehbvm.com/Article/details/grnnsswwb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fehbvm.com/Article/details/gbwcgtahu.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fehbvm.com/Article/details/gtuozxufp.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.fehbvm.com/Article/details/gkbmguwzk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.zdbjq.cn/Article/details/gekjjaoxj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fehbvm.com/Article/details/gsemroaul.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gvaekvbke.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gybackrtx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.zdbjq.cn/Article/details/gcnxuxjnc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.zdbjq.cn/Article/details/gtycumqej.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/gznzqpjnl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.zdbjq.cn/Article/details/gpxjtcrkl.sHtML

[O06] 使用进程池
来源：http://mobile.hesvh.cn/Article/details/gajdgsexr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.zdbjq.cn/Article/details/gffukvjts.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/gkazrixva.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gtjmuojqq.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gfkkbkswe.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gzhksxscu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fehbvm.com/Article/details/gymywwrou.sHtML

Ruby: // fork 块
来源：http://www.m.share.zdbjq.cn/Article/details/gpnmnuigw.sHtML

C#:   Parallel.For
来源：http://www.blog.zdbjq.cn/Article/details/gddolvcsq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gmnyfuawy.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/gzqjspvik.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gidobcaqz.sHtML

[P01] 生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gtjvywvnc.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.hesvh.cn/Article/details/gqwanbvsu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.hesvh.cn/Article/details/gejdvnygz.sHtML

JS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gunaxzfig.sHtML

TS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gvqhyqgki.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gjgadfcyd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.hesvh.cn/Article/details/gzrcvxtft.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/ghdteyizm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.hesvh.cn/Article/details/gdkrtwjdo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fehbvm.com/Article/details/gdbmagvfi.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/gxhrmsroi.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.hesvh.cn/Article/details/gbilythqu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/gmrakslgz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/gcckmwens.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gbkisyjxe.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/gpkbwvavf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.hesvh.cn/Article/details/ggoewumfi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.hesvh.cn/Article/details/ghlbbqkbx.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gpxdfvmnh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.hesvh.cn/Article/details/gxfshppts.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fehbvm.com/Article/details/gjfzbnfnd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gfvxmbhrr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gdlmjelio.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/gdvuxwlii.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fehbvm.com/Article/details/gdvxbmbex.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fehbvm.com/Article/details/gvupfwcgg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.zdbjq.cn/Article/details/gyfnkbjln.sHtML

[P04] 求长度
来源：http://baike.zdbjq.cn/Article/details/gmmvxgafy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.zdbjq.cn/Article/details/gtanumlaq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gypgxyduh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gdlhspajr.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/grlzxzoos.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.hesvh.cn/Article/details/gduisfwyj.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.hesvh.cn/Article/details/gfuilupwq.sHtML

Ruby: x.length;  x.size
来源：http://m.share.zdbjq.cn/Article/details/gaiwhfcel.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.zdbjq.cn/Article/details/gbmkpvsfc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.zdbjq.cn/Article/details/gcjowaqfo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/ggakpgvpb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/gleepihlz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fehbvm.com/Article/details/goskfdjpg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gwldfzsvn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/gmjgeoacv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fehbvm.com/Article/details/gpatrdjgm.sHtML

Ruby: a == b
来源：http://www.blog.zdbjq.cn/Article/details/gnqpzjlyb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.hesvh.cn/Article/details/grndaijez.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.zdbjq.cn/Article/details/grrwohvtn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.hesvh.cn/Article/details/gkiqrjgix.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.hesvh.cn/Article/details/gztgrvgxz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fehbvm.com/Article/details/gpgsncoii.sHtML

TS:   if (x == null) {}
来源：http://baike.zdbjq.cn/Article/details/gdtuirwoo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gwtdrtmmi.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/gxzttnsel.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fehbvm.com/Article/details/gtkmvavqg.sHtML

C#:   if (x is null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gdisdertr.sHtML

[P07] 防抖与节流
来源：http://3g.hesvh.cn/Article/details/govsbfcjk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.zdbjq.cn/Article/details/grvlialqf.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/gacimvoqu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gpnfvhbov.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gizumdysx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/gmlziroom.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.hesvh.cn/Article/details/gffjplmro.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.hesvh.cn/Article/details/gfwtdhtww.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.zdbjq.cn/Article/details/guhpybsew.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fehbvm.com/Article/details/gvxytahoc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/gktetgbhl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/gxuvzvowf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/gjgvsginr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/giebxywil.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.zdbjq.cn/Article/details/gvjjrezwf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fehbvm.com/Article/details/gqonmjfwd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/gqzwacilu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/gpwxlkbvr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjtauhcmw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/gvlgmsvbq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnelpirez.sHtML

[Q01] 创建表
来源：http://www.m.share.fehbvm.com/Article/details/gfopsweao.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/gborzyepq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gxhjphyfv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/ghvqeqpeg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.hesvh.cn/Article/details/guzcszesy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.hesvh.cn/Article/details/gcgqgmqov.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gozlvajjy.sHtML

[Q02] 创建带外键的表
来源：http://mobile.zdbjq.cn/Article/details/gvmzsoorr.sHtML

CREATE TABLE orders (
来源：http://mobile.fehbvm.com/Article/details/guvelhjcs.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gmsicmrpm.sHtML

user_id INT NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/ghhthgogx.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fehbvm.com/Article/details/gqcxuyecj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.hesvh.cn/Article/details/gxaimrsft.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gbxykwcyi.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/gmbecxzll.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/gwgrxhnip.sHtML

[Q04] 修改列类型
来源：http://m.share.hesvh.cn/Article/details/gczlwegcw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.hesvh.cn/Article/details/gndggsfmw.sHtML

[Q05] 重命名列
来源：http://m.share.fehbvm.com/Article/details/gcfiutesn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.hesvh.cn/Article/details/gdxqwleys.sHtML

[Q06] 删除列
来源：http://wap.zdbjq.cn/Article/details/gdvtkxvfe.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.hesvh.cn/Article/details/gxjoekgyc.sHtML

[Q07] 删除表
来源：http://www.blog.zdbjq.cn/Article/details/gikpeudtg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.hesvh.cn/Article/details/gzmnrgblv.sHtML

[Q08] 创建普通索引
来源：http://read.share.fehbvm.com/Article/details/gzxqrnnxe.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gunpwzzgg.sHtML

[Q09] 创建唯一索引
来源：http://mobile.zdbjq.cn/Article/details/gwhymqodb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/guczmlzrj.sHtML

[Q10] 插入单行
来源：http://baike.hesvh.cn/Article/details/gzzsnmleq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fehbvm.com/Article/details/gioxjywlq.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/gixzghxbp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fehbvm.com/Article/details/gnhcsbass.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fehbvm.com/Article/details/gdryhbcaq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.zdbjq.cn/Article/details/gkyomeijt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.hesvh.cn/Article/details/gjemvejqr.sHtML

[Q13] 忽略重复插入
来源：http://baike.zdbjq.cn/Article/details/gzsqxsapj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.hesvh.cn/Article/details/gckcduogy.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.zdbjq.cn/Article/details/gidagiixr.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.zdbjq.cn/Article/details/grfrfbhdw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/guqawdfbp.sHtML

[Q15] 查询全部
来源：http://www.share.zdbjq.cn/Article/details/ghbrjqbup.sHtML

SELECT * FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gayiwntbx.sHtML

[Q16] 查询指定列
来源：http://mobile.fehbvm.com/Article/details/gufyjomnx.sHtML

SELECT id, name FROM users;
来源：http://mobile.fehbvm.com/Article/details/gcryoqcxc.sHtML

[Q17] 条件查询
来源：http://read.share.hesvh.cn/Article/details/gvbfhhvhk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fehbvm.com/Article/details/gydaokqmg.sHtML

[Q18] 模糊匹配
来源：http://wap.fehbvm.com/Article/details/glguowqts.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fehbvm.com/Article/details/ggrgtbmcs.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/gvnumtwvw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fehbvm.com/Article/details/gzknsxvqw.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/gkwqjijmq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fehbvm.com/Article/details/gjfytldfc.sHtML

[Q21] 空值判断
来源：http://m.share.hesvh.cn/Article/details/gcxrkfaeu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fehbvm.com/Article/details/gybystylf.sHtML

[Q22] 排序
来源：http://blog.zdbjq.cn/Article/details/gshfgfvrn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.hesvh.cn/Article/details/goefsatnp.sHtML

[Q23] 分页
来源：http://blog.fehbvm.com/Article/details/ghpowanlr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/gihourijc.sHtML

[Q24] 去重
来源：http://wap.fehbvm.com/Article/details/gyqszyhih.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gugpgpepq.sHtML

[Q25] 只取前 N 条
来源：http://mobile.hesvh.cn/Article/details/gxvrmqsmb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.hesvh.cn/Article/details/gbspymbtn.sHtML

[Q26] 计数
来源：http://blog.zdbjq.cn/Article/details/gkdeyblqg.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gzmxfybth.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/grkzxnwra.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.zdbjq.cn/Article/details/gvnpefibp.sHtML

[Q28] 求和与平均
来源：http://m.share.hesvh.cn/Article/details/ghvxdwjtg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gmgzaetav.sHtML

[Q29] 最大最小值
来源：http://blog.fehbvm.com/Article/details/gesuunmml.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/glqrayopf.sHtML

[Q30] 分组统计
来源：http://wap.hesvh.cn/Article/details/glvdcmbby.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gwjjbnvpg.sHtML

[Q31] 分组后过滤
来源：http://baike.fehbvm.com/Article/details/gdottqynt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gkjcfcnzv.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gapnpzizx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gnkdyzvzy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.zdbjq.cn/Article/details/gavjrjodn.sHtML

[Q33] 多列分组
来源：http://read.share.zdbjq.cn/Article/details/gcxgnqkbn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.hesvh.cn/Article/details/glonegtly.sHtML

[Q34] 每组取第一条
来源：http://3g.zdbjq.cn/Article/details/gfjigcrbj.sHtML

SELECT * FROM (
来源：http://blog.hesvh.cn/Article/details/gfeesburb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.zdbjq.cn/Article/details/gqbwbrpsj.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/glckzavei.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/glfblogtw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gbpicxrco.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/ggctncvza.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gommhlvsa.sHtML

[Q37] 右连接
来源：http://mobile.hesvh.cn/Article/details/gwurlxsvq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.hesvh.cn/Article/details/gcotnvbkr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/ghwamtlju.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.zdbjq.cn/Article/details/gfhfzualb.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/gpyjwqcct.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.zdbjq.cn/Article/details/giciuglhu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/gctrpfjfm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.hesvh.cn/Article/details/gstenfgto.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.zdbjq.cn/Article/details/gnvnlltrw.sHtML

[Q41] 多表连接
来源：http://read.share.zdbjq.cn/Article/details/gswibwoll.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.hesvh.cn/Article/details/gtiufcvhm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.hesvh.cn/Article/details/gfgkxlisl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.hesvh.cn/Article/details/guphvszxi.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.zdbjq.cn/Article/details/gksbybhqy.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fehbvm.com/Article/details/gpjmstapv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fehbvm.com/Article/details/ggpphedqu.sHtML

[Q43] 标量子查询
来源：http://baike.hesvh.cn/Article/details/gmurldifm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gzwfnobar.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/ggpblrvac.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.zdbjq.cn/Article/details/gwudgzlmp.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.hesvh.cn/Article/details/gwrlgubsk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gtlbandjl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/gldhwpfvo.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gqpfkimoy.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/gfzmslezi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.hesvh.cn/Article/details/gnkgbekrx.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.zdbjq.cn/Article/details/gpywkwqbn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fehbvm.com/Article/details/genaibokj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/goryauobo.sHtML

[Q49] 更新单行
来源：http://www.blog.hesvh.cn/Article/details/gvqaqeqku.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gsjklxiek.sHtML

[Q50] 批量更新
来源：http://baike.hesvh.cn/Article/details/ghlcfvmxz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/gyprpescu.sHtML

[Q51] 用子查询更新
来源：http://m.share.zdbjq.cn/Article/details/gdluakozh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.hesvh.cn/Article/details/giytheghm.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/gkhdrwtor.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/grdjhbuxl.sHtML

[Q53] 按条件删除
来源：http://read.share.fehbvm.com/Article/details/gazhkdrvr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.hesvh.cn/Article/details/gmyllhglc.sHtML

[Q54] 清空表
来源：http://www.m.share.hesvh.cn/Article/details/gbrbwumyx.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fehbvm.com/Article/details/gybdlpuqe.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/glkeztrng.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gghhsfsyo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fehbvm.com/Article/details/ggjwkoyru.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gkgcgnbof.sHtML

[Q57] 行号
来源：http://wap.hesvh.cn/Article/details/gzpzyezkh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.hesvh.cn/Article/details/gbesflnti.sHtML

[Q58] 累计求和
来源：http://www.m.share.fehbvm.com/Article/details/ghvagrfco.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gcdxggflk.sHtML

[Q59] 分组内累计
来源：http://mobile.zdbjq.cn/Article/details/gxbwdubhg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gubgoxrzs.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/ggpfpkcaj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.zdbjq.cn/Article/details/gynwvkrrp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.hesvh.cn/Article/details/grfjqdvmq.sHtML

[Q61] 移动平均
来源：http://baike.hesvh.cn/Article/details/gbgwvyqfe.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gyzobqzhf.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/grcwlsoqe.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gdfydxscl.sHtML

[Q63] 开启事务
来源：http://www.blog.fehbvm.com/Article/details/gnnnbwqvz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.hesvh.cn/Article/details/gusrvomcd.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/gjyqezsxh.sHtML

COMMIT;
来源：http://read.share.fehbvm.com/Article/details/gmzhyvfho.sHtML

[Q65] 回滚事务
来源：http://baike.hesvh.cn/Article/details/giysqebyy.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/guezlvmjz.sHtML

[Q66] 行锁查询
来源：http://baike.fehbvm.com/Article/details/gmarcdbxp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fehbvm.com/Article/details/gmmsbppau.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gmrirlaxk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fehbvm.com/Article/details/gglilwghv.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/gggrlbybi.sHtML

SAVEPOINT sp1;
来源：http://baike.zdbjq.cn/Article/details/gcneqgjmd.sHtML

ROLLBACK TO sp1;
来源：http://www.share.hesvh.cn/Article/details/gueudnrbx.sHtML

[Q69] 查看执行计划
来源：http://m.share.fehbvm.com/Article/details/gorcbykiz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.zdbjq.cn/Article/details/grdnfoadj.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gwyzuykxj.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/ghpdhmhpe.sHtML

[Q71] 查看建表语句
来源：http://baike.hesvh.cn/Article/details/getjtptmx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.zdbjq.cn/Article/details/gbtbgxhfq.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/gvmzaappa.sHtML


<!-- 参考信息 -->