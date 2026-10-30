代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fehbvm.com/Article/details/gjtbduefs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fehbvm.com/Article/details/gypauoltu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.hesvh.cn/Article/details/gmulmraol.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gxerhbkju.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.hesvh.cn/Article/details/gxsqgyuso.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/gxgwzgnin.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.zdbjq.cn/Article/details/ghgtmraeg.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/gzhylrtcc.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/gfjvonoic.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/gmcgbaawz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fehbvm.com/Article/details/gdqegnbnu.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gpekhezvo.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gdprbyfxk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fehbvm.com/Article/details/gyzaqfput.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/gaodvnogk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/gemhanvhj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.fehbvm.com/Article/details/gfgpahqpu.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/gbsvduias.sHtML

Py:   with lock: shared += 1
来源：http://mobile.zdbjq.cn/Article/details/gkfdxksme.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.zdbjq.cn/Article/details/guadeeqhc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/gowfhgkjq.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gqjdvtwkw.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gzjktgbeg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fehbvm.com/Article/details/gvchqhyqo.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fehbvm.com/Article/details/gzxixyupf.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gciqzycgj.sHtML

[O04] 定义异步函数并等待
来源：http://baike.zdbjq.cn/Article/details/gwskuivqu.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/gpdqfjoii.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/gfeinkbcz.sHtML

JS:   async function f() { await g(); }
来源：http://baike.hesvh.cn/Article/details/glgkwwwth.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gvnjxyfec.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.hesvh.cn/Article/details/gyvvajgus.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/gvxcexvlo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/gixbhypiq.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.hesvh.cn/Article/details/gnrjfxhzl.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.hesvh.cn/Article/details/gwadtunbb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.hesvh.cn/Article/details/gmthiiytn.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fehbvm.com/Article/details/gtrwjojvk.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gfrbdjljt.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gpignzmzq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/gtkzkmdxf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.hesvh.cn/Article/details/gvfqiihty.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/gpqknhmws.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.zdbjq.cn/Article/details/gwicbjemi.sHtML

[O06] 使用进程池
来源：http://baike.fehbvm.com/Article/details/gsraygnpv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.hesvh.cn/Article/details/grxsaqjoc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.zdbjq.cn/Article/details/gnyxbkbft.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gyyvqjcnx.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gqswzqbwl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fehbvm.com/Article/details/gpfbmlzsr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fehbvm.com/Article/details/geodnynli.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/gdxzjidms.sHtML

C#:   Parallel.For
来源：http://baike.hesvh.cn/Article/details/gvwnoewsd.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gynbfpvjw.sHtML

P. 常用工具函数
来源：http://read.share.hesvh.cn/Article/details/gzdqwbxvw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkjprniol.sHtML

[P01] 生成 UUID
来源：http://baike.fehbvm.com/Article/details/gqwfyrfiq.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fehbvm.com/Article/details/gpmvgsujg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.hesvh.cn/Article/details/ggfdshtiy.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gterpvnau.sHtML

TS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gjtmpefpb.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/ggsufkrhn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gncjdnzcf.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.zdbjq.cn/Article/details/gznflzqhv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/gkgqiafue.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/gpqyamqfe.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/gcwfgbxtv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.zdbjq.cn/Article/details/gdpiryzog.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.zdbjq.cn/Article/details/gthfardki.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/gsbrkqccq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.hesvh.cn/Article/details/gbyqtmcad.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/gwqsfhdpk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gwtzhijkp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/ginffyhcl.sHtML

[P03] 生成短随机字符串
来源：http://blog.fehbvm.com/Article/details/gwwmikueh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fehbvm.com/Article/details/gmurlxluo.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.zdbjq.cn/Article/details/glnuvbmvz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/galivstvz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gqfpjsenx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.hesvh.cn/Article/details/gpglxnjbc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.hesvh.cn/Article/details/gypgitemo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.zdbjq.cn/Article/details/gwcgcgwko.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.zdbjq.cn/Article/details/ghpybgedg.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/gcumzqakr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fehbvm.com/Article/details/gokngeekp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gatiyxyep.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gkwzknykt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gsietccbq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.hesvh.cn/Article/details/ghlntanex.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fehbvm.com/Article/details/gldrrvwux.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/gapkaiqim.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/grkenpvro.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.fehbvm.com/Article/details/gxvjaolmw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fehbvm.com/Article/details/gsssheoon.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.hesvh.cn/Article/details/gmipgsgfv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.hesvh.cn/Article/details/gckbxcdij.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gebbwneaj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/gyjqywtpk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.hesvh.cn/Article/details/gufpmdhem.sHtML

Ruby: a == b
来源：http://www.m.share.zdbjq.cn/Article/details/giwncpygu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.zdbjq.cn/Article/details/gmisegojc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/gilqclxau.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fehbvm.com/Article/details/gscfrrvld.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.hesvh.cn/Article/details/guympzavp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.zdbjq.cn/Article/details/gifffiyfv.sHtML

TS:   if (x == null) {}
来源：http://wap.zdbjq.cn/Article/details/guqkphdfg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gezehhtrd.sHtML

Go:   if x == nil {}
来源：http://www.blog.fehbvm.com/Article/details/gvreralws.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.zdbjq.cn/Article/details/gcjqdebga.sHtML

C#:   if (x is null) {}
来源：http://blog.fehbvm.com/Article/details/gttquoqlp.sHtML

[P07] 防抖与节流
来源：http://mobile.hesvh.cn/Article/details/gnfbvzhht.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/gwuxnkqfp.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.zdbjq.cn/Article/details/gbktyjghf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gfvqvfnzi.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gbpkfxqrc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.zdbjq.cn/Article/details/gocrmdorj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/grxlaaezl.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.zdbjq.cn/Article/details/gwzbsvuuc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/gurquttdg.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/gpnsmnedf.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fehbvm.com/Article/details/gfhrwoacw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.zdbjq.cn/Article/details/glrkqehrq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fehbvm.com/Article/details/gprljmavm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/grtzerecn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.hesvh.cn/Article/details/gxsnqjnch.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fehbvm.com/Article/details/ghloggaxv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.zdbjq.cn/Article/details/gxcfphzxw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fehbvm.com/Article/details/gqldztrlj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glsmhsbfg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/geowjywhk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxurvsvvl.sHtML

[Q01] 创建表
来源：http://www.blog.zdbjq.cn/Article/details/gzhiuzfho.sHtML

CREATE TABLE users (
来源：http://mobile.fehbvm.com/Article/details/gyxgnfkbr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/goaaotclj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gorxqidtl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fehbvm.com/Article/details/gsujplgik.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/gkkwbpvgg.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gtlpwsxkm.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/glkrlnwob.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/gjcsydyri.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gvaypylwy.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gcwcdpuzu.sHtML

amount DECIMAL(10, 2),
来源：http://blog.hesvh.cn/Article/details/gpfkkdoib.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fehbvm.com/Article/details/gwlnlsdhn.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gudagmkuo.sHtML

[Q03] 增加列
来源：http://wap.fehbvm.com/Article/details/gatidphyb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/gtdevhnbp.sHtML

[Q04] 修改列类型
来源：http://3g.zdbjq.cn/Article/details/gbaoeodmg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.zdbjq.cn/Article/details/gkayuzjrm.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/gmbzkorlw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fehbvm.com/Article/details/ggmiqdlhp.sHtML

[Q06] 删除列
来源：http://read.share.hesvh.cn/Article/details/gsxsvkold.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/gglndbzwh.sHtML

[Q07] 删除表
来源：http://www.blog.zdbjq.cn/Article/details/glntmgjjc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gdbniqndd.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/gzcecoxpm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gbupypapi.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/gvixfzipk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gixynfwfl.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/ghncxqkkw.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.zdbjq.cn/Article/details/glkcyqxro.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/goguiogfu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gnekvqphn.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.hesvh.cn/Article/details/ghkqobekq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fehbvm.com/Article/details/gojfthmzs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.hesvh.cn/Article/details/gwuflfqjk.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.hesvh.cn/Article/details/gfwqpwlgx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gcxmkarig.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/gqvcpkwpe.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.hesvh.cn/Article/details/gybtuwpmd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fehbvm.com/Article/details/gqwzqtydl.sHtML

[Q15] 查询全部
来源：http://mobile.hesvh.cn/Article/details/gdwuqhfqi.sHtML

SELECT * FROM users;
来源：http://m.share.fehbvm.com/Article/details/gufsxkjbs.sHtML

[Q16] 查询指定列
来源：http://mobile.hesvh.cn/Article/details/grulnupxn.sHtML

SELECT id, name FROM users;
来源：http://blog.zdbjq.cn/Article/details/gprsdmflr.sHtML

[Q17] 条件查询
来源：http://read.share.hesvh.cn/Article/details/gniykqtne.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/ggjfqongi.sHtML

[Q18] 模糊匹配
来源：http://mobile.zdbjq.cn/Article/details/gfgwtesmb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.hesvh.cn/Article/details/gqrrzlqhq.sHtML

[Q19] 范围查询
来源：http://wap.fehbvm.com/Article/details/grbvnfauj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/gbvppdsik.sHtML

[Q20] IN 列表
来源：http://www.blog.hesvh.cn/Article/details/gxatnuhby.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gppjxixhu.sHtML

[Q21] 空值判断
来源：http://blog.hesvh.cn/Article/details/goueudppb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.zdbjq.cn/Article/details/gfrlieukn.sHtML

[Q22] 排序
来源：http://m.share.fehbvm.com/Article/details/gpjoxmsmm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.hesvh.cn/Article/details/gekrjhwgj.sHtML

[Q23] 分页
来源：http://read.share.zdbjq.cn/Article/details/gkdlgeayo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.zdbjq.cn/Article/details/gkqzgzyeg.sHtML

[Q24] 去重
来源：http://wap.hesvh.cn/Article/details/gdfjmkezt.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.zdbjq.cn/Article/details/gzggwhxux.sHtML

[Q25] 只取前 N 条
来源：http://blog.fehbvm.com/Article/details/gyrovaiga.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.zdbjq.cn/Article/details/gmcoyudfj.sHtML

[Q26] 计数
来源：http://3g.zdbjq.cn/Article/details/ghtplhbgp.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gggeukdnv.sHtML

[Q27] 条件计数
来源：http://baike.hesvh.cn/Article/details/gmgmkybfj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.zdbjq.cn/Article/details/ghsagilzc.sHtML

[Q28] 求和与平均
来源：http://blog.fehbvm.com/Article/details/gplcodach.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gpiixbkjq.sHtML

[Q29] 最大最小值
来源：http://m.share.zdbjq.cn/Article/details/gexqhgzgx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gsgrmkgie.sHtML

[Q30] 分组统计
来源：http://wap.hesvh.cn/Article/details/gcjmbhcnr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gvdptdfiw.sHtML

[Q31] 分组后过滤
来源：http://3g.zdbjq.cn/Article/details/gjcrwqgoe.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.zdbjq.cn/Article/details/gbpltslwl.sHtML

[Q32] 分组拼接字符串
来源：http://blog.hesvh.cn/Article/details/gpkponzje.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/glqexiwsv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/gadvrurwe.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/geltypvcw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fehbvm.com/Article/details/gtnlmughp.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/gbgzombwy.sHtML

SELECT * FROM (
来源：http://m.share.fehbvm.com/Article/details/gjrhlzhao.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.zdbjq.cn/Article/details/gsbyxzoig.sHtML

) t WHERE rn = 1;
来源：http://baike.zdbjq.cn/Article/details/gihbygpar.sHtML

[Q35] 内连接
来源：http://baike.zdbjq.cn/Article/details/gigebpubf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gcskokmsi.sHtML

[Q36] 左连接
来源：http://wap.zdbjq.cn/Article/details/gvpczivhj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gbkstwagk.sHtML

[Q37] 右连接
来源：http://blog.zdbjq.cn/Article/details/giwztwxxe.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/grhyxfxvp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.zdbjq.cn/Article/details/gwhcttjuv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fehbvm.com/Article/details/grthdhkrw.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.zdbjq.cn/Article/details/glbgasckp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.hesvh.cn/Article/details/grkqnmhwh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fehbvm.com/Article/details/ghvgdbblr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.zdbjq.cn/Article/details/grqqlamlb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.zdbjq.cn/Article/details/ghvcfeoud.sHtML

[Q41] 多表连接
来源：http://blog.hesvh.cn/Article/details/gzobxivqb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.zdbjq.cn/Article/details/gvnatgxsj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/gbobkipao.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fehbvm.com/Article/details/gmkbzwyxm.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.zdbjq.cn/Article/details/gextkilfh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fehbvm.com/Article/details/ghuhlznct.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.hesvh.cn/Article/details/gariocwdn.sHtML

[Q43] 标量子查询
来源：http://mobile.hesvh.cn/Article/details/gevlizxpf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.hesvh.cn/Article/details/grvpvgimh.sHtML

[Q44] IN 子查询
来源：http://www.blog.fehbvm.com/Article/details/gqohwcgyw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fehbvm.com/Article/details/gpvvsdkwn.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.hesvh.cn/Article/details/gkpzlsbga.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gkwhcoulp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.hesvh.cn/Article/details/ghhmtcruo.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gcmehriwy.sHtML

[Q47] 与平均值比较
来源：http://wap.fehbvm.com/Article/details/grflzsasg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.hesvh.cn/Article/details/gukreocwv.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fehbvm.com/Article/details/gzrmvqlwe.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.hesvh.cn/Article/details/gpjewrmtd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.hesvh.cn/Article/details/gynzjcwpv.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/gjtjahdvk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gbkpjuzgk.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/gwayzelxe.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fehbvm.com/Article/details/gvthxhfej.sHtML

[Q51] 用子查询更新
来源：http://www.blog.zdbjq.cn/Article/details/gdbhfzpsb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fehbvm.com/Article/details/gybazhklt.sHtML

[Q52] 删除指定行
来源：http://m.share.hesvh.cn/Article/details/gepfurgmg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gkgtitnqp.sHtML

[Q53] 按条件删除
来源：http://baike.zdbjq.cn/Article/details/grafrjarw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/gmbnbnkxd.sHtML

[Q54] 清空表
来源：http://www.m.share.fehbvm.com/Article/details/gsmsnszdw.sHtML

TRUNCATE TABLE logs;
来源：http://3g.hesvh.cn/Article/details/gtrsvfuwx.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.hesvh.cn/Article/details/gnpivvurm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/glkjpzvtu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.zdbjq.cn/Article/details/gnphizizx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.hesvh.cn/Article/details/gehorkzuk.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/gfrwfepmc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gfjxduwxe.sHtML

[Q58] 累计求和
来源：http://www.m.share.fehbvm.com/Article/details/gpvjomugm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fehbvm.com/Article/details/glyrdqwfp.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fehbvm.com/Article/details/gsjzcnigr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gcfexhryl.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/gbdffmmdk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/gthmywmdq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.hesvh.cn/Article/details/gdepmziat.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/gqxqvclip.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gswzdpjtj.sHtML

[Q62] 分组占比
来源：http://m.share.zdbjq.cn/Article/details/gibmdvekn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gqotnvqjm.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/gfgtkyoci.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/gxepwadmy.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/ghtvwbzty.sHtML

COMMIT;
来源：http://mobile.fehbvm.com/Article/details/gomlbelxr.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gxagjdqyf.sHtML

ROLLBACK;
来源：http://mobile.hesvh.cn/Article/details/gxbtemotp.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/gxkbmeykb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.zdbjq.cn/Article/details/ghbzsnjyb.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.zdbjq.cn/Article/details/gwzgdvgxl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fehbvm.com/Article/details/ggzsqfrkl.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/gyhcdjegb.sHtML

SAVEPOINT sp1;
来源：http://wap.zdbjq.cn/Article/details/giyxpmhic.sHtML

ROLLBACK TO sp1;
来源：http://m.share.zdbjq.cn/Article/details/gkteickau.sHtML

[Q69] 查看执行计划
来源：http://www.share.fehbvm.com/Article/details/gvnrekcpl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.hesvh.cn/Article/details/gjcgdgjvv.sHtML

[Q70] 更新统计信息
来源：http://read.share.zdbjq.cn/Article/details/gjufsbuqs.sHtML

ANALYZE TABLE users;
来源：http://wap.zdbjq.cn/Article/details/glqffbmtt.sHtML

[Q71] 查看建表语句
来源：http://mobile.fehbvm.com/Article/details/gffjohxmq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fehbvm.com/Article/details/gqsvvfiwq.sHtML

[Q72] 查看索引
来源：http://mobile.hesvh.cn/Article/details/gbnbgtaih.sHtML

SHOW INDEX FROM users;
来源：http://blog.zdbjq.cn/Article/details/gbxigykgy.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/gtjzegeig.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/gsjdiogma.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/gmdlplyhz.sHtML


<!-- 参考信息 -->