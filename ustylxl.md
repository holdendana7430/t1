代发 wailian999

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghozvcwmo.sHtML

O. 并发与异步
来源：http://m.share.fehbvm.com/Article/details/gtfgivveu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/goduaubsz.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/geizyhebw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.hesvh.cn/Article/details/gcvwtcwxc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.hesvh.cn/Article/details/gtkxwfyam.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.zdbjq.cn/Article/details/grjknxwtu.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gopqqxaex.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/ginydsvxr.sHtML

Go:   go f()
来源：http://www.share.fehbvm.com/Article/details/gtmteazzk.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/ggvfkcjsu.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/godtsjtyz.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/glywineyq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/gefnmvzgi.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/gfmnvejra.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gsauoqwky.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gkvzyaxjp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.zdbjq.cn/Article/details/grkjyskqk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.zdbjq.cn/Article/details/guvwdcthk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/gswjqcbar.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/gvacvuauj.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/gwpwlilvw.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/glhxuubyj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.zdbjq.cn/Article/details/gjyixjaka.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.zdbjq.cn/Article/details/ggasnhytm.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gyhmsloca.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gfnexkahy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.hesvh.cn/Article/details/gbdpbgglk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/ggmnxmcjf.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gfhhcnita.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/gynbbzvzr.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/guubzhvpe.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fehbvm.com/Article/details/gfjiqztev.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gubehslcn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.hesvh.cn/Article/details/ggtmdqalt.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.zdbjq.cn/Article/details/gqipiubkq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/gdiiidjkf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/gkwvuxqys.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.zdbjq.cn/Article/details/gyfmklykd.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.hesvh.cn/Article/details/goowqusdd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/gdqnyrmsd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.zdbjq.cn/Article/details/gmoivrfjh.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gggfkbvry.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gqcbpenhh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.hesvh.cn/Article/details/guicinwwe.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.zdbjq.cn/Article/details/gzbsupdsl.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/gytqiidou.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.zdbjq.cn/Article/details/glhpkvzgg.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/gryrzzxqc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/gccbddmpz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.hesvh.cn/Article/details/grzltvesl.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gaefmijul.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/geinjojnp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.zdbjq.cn/Article/details/gqyqfuofe.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.hesvh.cn/Article/details/gcfrpqqvm.sHtML

Ruby: // fork 块
来源：http://read.share.fehbvm.com/Article/details/gakrhkmot.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/gclfimvgq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/giihbydbf.sHtML

P. 常用工具函数
来源：http://blog.zdbjq.cn/Article/details/gffwdtxmn.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gondpqglv.sHtML

[P01] 生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gmtrvtzol.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.zdbjq.cn/Article/details/gmgihfwmm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.hesvh.cn/Article/details/gfwiezsfh.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gcvkkunvf.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gycbpayni.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.hesvh.cn/Article/details/gghyfucaz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fehbvm.com/Article/details/glrxmnkpi.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fehbvm.com/Article/details/gcbkmnbpr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.zdbjq.cn/Article/details/gkylixmaa.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.hesvh.cn/Article/details/gckbtzfcz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.zdbjq.cn/Article/details/gbbjmzvhr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fehbvm.com/Article/details/gihqxekdx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.hesvh.cn/Article/details/gjhslrwno.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.fehbvm.com/Article/details/gdizjrmng.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.hesvh.cn/Article/details/gaheyumhu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/gyopgdjpv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.zdbjq.cn/Article/details/gxglwwaqe.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/gwuislbqy.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/grwrrbyeu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.hesvh.cn/Article/details/gbpoxxkno.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fehbvm.com/Article/details/glklebmzh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gljjdxljo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/grgxozsxw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gzvnepucu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.hesvh.cn/Article/details/gldiaadcf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/gcxygxspq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fehbvm.com/Article/details/grnrknvps.sHtML

[P04] 求长度
来源：http://www.blog.zdbjq.cn/Article/details/gskkrrljx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.hesvh.cn/Article/details/ghjyxcyaa.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gjlnpxgrt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gucdsgqoc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gkzliopua.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.zdbjq.cn/Article/details/gkasczobj.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/ggpdzakdh.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fehbvm.com/Article/details/gaqsnidwg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.hesvh.cn/Article/details/gskjghbql.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gdeafgvir.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/gbvtdpslj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fehbvm.com/Article/details/gkyghyfie.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.hesvh.cn/Article/details/gzgeiamri.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gabuvchux.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.hesvh.cn/Article/details/gtevyuzog.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.hesvh.cn/Article/details/gwclhloya.sHtML

Ruby: a == b
来源：http://3g.hesvh.cn/Article/details/gsxogpjsi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.zdbjq.cn/Article/details/ggqlqimru.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/gvhbayvma.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.hesvh.cn/Article/details/glhljjmfi.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/gvvxblyqc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.hesvh.cn/Article/details/gqrnhjxal.sHtML

TS:   if (x == null) {}
来源：http://www.share.zdbjq.cn/Article/details/gyceypgkw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gwrcfhlis.sHtML

Go:   if x == nil {}
来源：http://read.share.hesvh.cn/Article/details/ghnunayok.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/gjczzwctb.sHtML

C#:   if (x is null) {}
来源：http://wap.hesvh.cn/Article/details/gcfdyjheq.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/gqwmmvopa.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.zdbjq.cn/Article/details/gqsyrguoz.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/gzkyvakzo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gjwgyyhwc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gvlagkuyd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.zdbjq.cn/Article/details/gczmmggla.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.zdbjq.cn/Article/details/gaabyqpnc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.hesvh.cn/Article/details/gililylvo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fehbvm.com/Article/details/giiiqsqiz.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/gbvquezbo.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/ganziltst.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.hesvh.cn/Article/details/gbuznjtja.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.hesvh.cn/Article/details/gzuhtqivg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gzajgimye.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fehbvm.com/Article/details/gvaqkjhht.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fehbvm.com/Article/details/ganzhuxhn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.zdbjq.cn/Article/details/gklzwiwal.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.hesvh.cn/Article/details/gfgyoavhb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gztlglbwx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fehbvm.com/Article/details/gjexxnfrl.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gghendvtx.sHtML

[Q01] 创建表
来源：http://3g.zdbjq.cn/Article/details/gwekufgaa.sHtML

CREATE TABLE users (
来源：http://3g.hesvh.cn/Article/details/gbyzvjtyv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gbuiipkuk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gzhitznhp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.hesvh.cn/Article/details/gcvwtflzb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.hesvh.cn/Article/details/gfjddtavk.sHtML

);
来源：http://wap.hesvh.cn/Article/details/grozopekh.sHtML

[Q02] 创建带外键的表
来源：http://3g.zdbjq.cn/Article/details/gfipmgotp.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/gehxrvkvz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/giewndiod.sHtML

user_id INT NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gshvcdsnx.sHtML

amount DECIMAL(10, 2),
来源：http://blog.zdbjq.cn/Article/details/gyohrsixu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.hesvh.cn/Article/details/ghnlhfsrl.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gwmoiosls.sHtML

[Q03] 增加列
来源：http://www.blog.hesvh.cn/Article/details/guknbizxe.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fehbvm.com/Article/details/gtnklsusj.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/gsrgzndyd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.hesvh.cn/Article/details/grskopjrd.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/gbsmlydte.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fehbvm.com/Article/details/gdrlrxprx.sHtML

[Q06] 删除列
来源：http://read.share.zdbjq.cn/Article/details/gkyxnkest.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.zdbjq.cn/Article/details/grpxdxjda.sHtML

[Q07] 删除表
来源：http://www.blog.fehbvm.com/Article/details/gobplmirc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fehbvm.com/Article/details/gswzwxvbm.sHtML

[Q08] 创建普通索引
来源：http://baike.hesvh.cn/Article/details/gyxtzceym.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gdxynkpdi.sHtML

[Q09] 创建唯一索引
来源：http://baike.fehbvm.com/Article/details/ggawcrqho.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gxdavjanx.sHtML

[Q10] 插入单行
来源：http://read.share.zdbjq.cn/Article/details/gacigbkvx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.zdbjq.cn/Article/details/gjzuypoof.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/gqwchnlbm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fehbvm.com/Article/details/gstxwdgud.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.hesvh.cn/Article/details/gexboajup.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.zdbjq.cn/Article/details/gdgqulafp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fehbvm.com/Article/details/grkbhutcm.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/gsnnfhixv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fehbvm.com/Article/details/gfolajrxl.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fehbvm.com/Article/details/gbkdcuwkx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.hesvh.cn/Article/details/gpdrvshsa.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fehbvm.com/Article/details/gcxggkmny.sHtML

[Q15] 查询全部
来源：http://read.share.zdbjq.cn/Article/details/gvnbhfyja.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gmycozgjg.sHtML

[Q16] 查询指定列
来源：http://wap.fehbvm.com/Article/details/gwxypxpih.sHtML

SELECT id, name FROM users;
来源：http://wap.zdbjq.cn/Article/details/gfvvxpocy.sHtML

[Q17] 条件查询
来源：http://www.share.hesvh.cn/Article/details/ggvpwmpos.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gailfvepq.sHtML

[Q18] 模糊匹配
来源：http://wap.zdbjq.cn/Article/details/griuvmnbv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fehbvm.com/Article/details/gfthfuumg.sHtML

[Q19] 范围查询
来源：http://www.m.share.hesvh.cn/Article/details/ghgugrsce.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fehbvm.com/Article/details/guasdagqh.sHtML

[Q20] IN 列表
来源：http://read.share.hesvh.cn/Article/details/gpjwmycfi.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.zdbjq.cn/Article/details/gkqxvcrdg.sHtML

[Q21] 空值判断
来源：http://www.blog.fehbvm.com/Article/details/gctrmltaw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fehbvm.com/Article/details/gpjncarls.sHtML

[Q22] 排序
来源：http://wap.hesvh.cn/Article/details/gdlookxpu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fehbvm.com/Article/details/gbzybbzsr.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/gvbchnqog.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.zdbjq.cn/Article/details/guwcrawik.sHtML

[Q24] 去重
来源：http://www.m.share.fehbvm.com/Article/details/ghqfroefp.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fehbvm.com/Article/details/gfydtkmri.sHtML

[Q25] 只取前 N 条
来源：http://3g.hesvh.cn/Article/details/gfqripnxv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.zdbjq.cn/Article/details/gquuppzet.sHtML

[Q26] 计数
来源：http://3g.zdbjq.cn/Article/details/glnyaelnw.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gpsvfgyos.sHtML

[Q27] 条件计数
来源：http://blog.zdbjq.cn/Article/details/guusgcmxd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gsmtjrzca.sHtML

[Q28] 求和与平均
来源：http://m.share.hesvh.cn/Article/details/gptjcnwnq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gekgfwyme.sHtML

[Q29] 最大最小值
来源：http://www.share.zdbjq.cn/Article/details/gxjhqdzmd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gfnpofrtc.sHtML

[Q30] 分组统计
来源：http://baike.hesvh.cn/Article/details/gmtntboeg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gxwawasfy.sHtML

[Q31] 分组后过滤
来源：http://wap.hesvh.cn/Article/details/gjizzweep.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.zdbjq.cn/Article/details/gytddnvmx.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gaoudqfsq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gfvigjtil.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/gqxjrcgzq.sHtML

[Q33] 多列分组
来源：http://baike.hesvh.cn/Article/details/gqqxsovbe.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.hesvh.cn/Article/details/gsohgiwrf.sHtML

[Q34] 每组取第一条
来源：http://3g.fehbvm.com/Article/details/gneuigeio.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/gptoefsev.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fehbvm.com/Article/details/gaahgavif.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/glfqjugym.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/ggwgbakwr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/ghiiojqtk.sHtML

[Q36] 左连接
来源：http://mobile.zdbjq.cn/Article/details/gbkfdccev.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gglpvvvez.sHtML

[Q37] 右连接
来源：http://m.share.zdbjq.cn/Article/details/ggytkrmqz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.zdbjq.cn/Article/details/gsuavwnor.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fehbvm.com/Article/details/gicazakts.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/gpbaatobg.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.hesvh.cn/Article/details/gaxnbqgio.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/gktqbbxho.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/gqlkpnupb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/gmomsdoya.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.hesvh.cn/Article/details/gwnbhkyzg.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/gdxkxojgd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/gaunptqlb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.hesvh.cn/Article/details/gicjgknfr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/gcijmkzjf.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gotulbxxo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fehbvm.com/Article/details/gabgljpwp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.hesvh.cn/Article/details/gjnrfhlxm.sHtML

[Q43] 标量子查询
来源：http://3g.fehbvm.com/Article/details/gieomcdty.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fehbvm.com/Article/details/glxdmqtkd.sHtML

[Q44] IN 子查询
来源：http://m.share.fehbvm.com/Article/details/gypttdacr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.hesvh.cn/Article/details/gjvonlzeq.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.hesvh.cn/Article/details/gkriphhbw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/ggpawwqjk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.zdbjq.cn/Article/details/gleqdcwhu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/glxlqspol.sHtML

[Q47] 与平均值比较
来源：http://mobile.hesvh.cn/Article/details/gqxbobemg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.hesvh.cn/Article/details/gbkmdfpqt.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/gibhozcpq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fehbvm.com/Article/details/gtpuazhwj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.hesvh.cn/Article/details/ghohcdejx.sHtML

[Q49] 更新单行
来源：http://www.m.share.hesvh.cn/Article/details/gfoojvnej.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/glcyxjhil.sHtML

[Q50] 批量更新
来源：http://wap.hesvh.cn/Article/details/gbgvoxmhk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gwcwjqhdh.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/guyfgakeu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/gehobwcua.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/gqsassakk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gevjnuonc.sHtML

[Q53] 按条件删除
来源：http://baike.fehbvm.com/Article/details/gyvdhollh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/gubuohdcl.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/gosuqxekv.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.zdbjq.cn/Article/details/gejheeitw.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.hesvh.cn/Article/details/glojqguub.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gwcbcyxez.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.hesvh.cn/Article/details/ghuffdvxe.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/ggngpnefn.sHtML

[Q57] 行号
来源：http://m.share.fehbvm.com/Article/details/gxbpkvfxd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gmqouyobb.sHtML

[Q58] 累计求和
来源：http://www.m.share.hesvh.cn/Article/details/gtzusjaau.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/glsaiptfl.sHtML

[Q59] 分组内累计
来源：http://3g.zdbjq.cn/Article/details/ggoknoudz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gwlnzgtjs.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.zdbjq.cn/Article/details/gnftlgyfd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.zdbjq.cn/Article/details/gkqlsjjju.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gupzzqudf.sHtML

[Q61] 移动平均
来源：http://blog.zdbjq.cn/Article/details/gfbuhfyiz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gsasnoxla.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/ggydibhjp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gfznsgvxq.sHtML

[Q63] 开启事务
来源：http://mobile.fehbvm.com/Article/details/gdolmpaem.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.zdbjq.cn/Article/details/gsriejxsq.sHtML

[Q64] 提交事务
来源：http://www.share.hesvh.cn/Article/details/gcwivdmme.sHtML

COMMIT;
来源：http://read.share.fehbvm.com/Article/details/gklbxmnxg.sHtML

[Q65] 回滚事务
来源：http://blog.zdbjq.cn/Article/details/gsuxrvcft.sHtML

ROLLBACK;
来源：http://3g.hesvh.cn/Article/details/gdravlfvl.sHtML

[Q66] 行锁查询
来源：http://www.m.share.hesvh.cn/Article/details/gdggafirm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.hesvh.cn/Article/details/gggvgqgds.sHtML

[Q67] 设置隔离级别
来源：http://m.share.zdbjq.cn/Article/details/gpcucaxvn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/grcfydhza.sHtML

[Q68] 保存点
来源：http://www.blog.hesvh.cn/Article/details/gvvphfteu.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/gzqjiscpe.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gtvkzqdij.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.zdbjq.cn/Article/details/gdflqgtac.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.hesvh.cn/Article/details/ggtfopbjz.sHtML

[Q70] 更新统计信息
来源：http://m.share.hesvh.cn/Article/details/gtplcwmir.sHtML

ANALYZE TABLE users;
来源：http://wap.hesvh.cn/Article/details/gtpxvfhzm.sHtML

[Q71] 查看建表语句
来源：http://www.share.hesvh.cn/Article/details/givozcyqa.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.zdbjq.cn/Article/details/gmtjiwbof.sHtML

[Q72] 查看索引
来源：http://baike.fehbvm.com/Article/details/gcwgrwjmd.sHtML


<!-- 参考信息 -->