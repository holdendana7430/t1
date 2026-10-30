代发 wailian999

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/guwpymgsa.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.zdbjq.cn/Article/details/gimxsuytj.sHtML

C#:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gslbwabwv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.zdbjq.cn/Article/details/gsshdqhed.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.zdbjq.cn/Article/details/gygfpztxj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.hesvh.cn/Article/details/grayzvsjg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gstoscuiw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gulnhymqe.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/goluqjtrx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/gftlsepgl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/gutrrkkni.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gqgliqfeq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gaowhmgsu.sHtML

O. 并发与异步
来源：http://3g.fehbvm.com/Article/details/gcvmuzlzc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grquixmro.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/gzzjexrde.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.hesvh.cn/Article/details/gathiktrc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.hesvh.cn/Article/details/gnbdroeyc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.zdbjq.cn/Article/details/gixmhekzh.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gbwgusqyi.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fehbvm.com/Article/details/gpaaaolwi.sHtML

Go:   go f()
来源：http://blog.zdbjq.cn/Article/details/gaxkcssak.sHtML

Ruby: Thread.new { f }
来源：http://m.share.zdbjq.cn/Article/details/gqwrmrtfb.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.zdbjq.cn/Article/details/gmdwvjlry.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/gdvudttck.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.zdbjq.cn/Article/details/gbopusypj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.zdbjq.cn/Article/details/ggqipxari.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gctbhvacb.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gsepekrjc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.hesvh.cn/Article/details/gysxmzrnu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/gnorhfwxg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/gkgesxmbu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.hesvh.cn/Article/details/ggmloisha.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fehbvm.com/Article/details/gjjamwoen.sHtML

Py:   with lock: shared += 1
来源：http://wap.fehbvm.com/Article/details/gznxyypme.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.zdbjq.cn/Article/details/gljxobppk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.zdbjq.cn/Article/details/girzeigxm.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gnghzdeys.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gaosdcedt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.zdbjq.cn/Article/details/gmotxdihw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.hesvh.cn/Article/details/gankjqflr.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gxikcicca.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fehbvm.com/Article/details/gmfcmrctu.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.hesvh.cn/Article/details/gvvtvbqmn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.zdbjq.cn/Article/details/gxdxxexmj.sHtML

JS:   async function f() { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gcxqkfufc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gdziokxfy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.zdbjq.cn/Article/details/giwtdbmbs.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/gzdbbkjfg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/gmkgtupyk.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.hesvh.cn/Article/details/gihmrorqo.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.hesvh.cn/Article/details/gzlwnevyh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gvmnpfati.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/gjquamxzp.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gsjgrasnt.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gqfwrmmra.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fehbvm.com/Article/details/gdhmpqcvg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.hesvh.cn/Article/details/gdrzyhnwt.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gnvttlmiu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.zdbjq.cn/Article/details/gdbhlehec.sHtML

[O06] 使用进程池
来源：http://mobile.hesvh.cn/Article/details/glmxbpodz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.zdbjq.cn/Article/details/goablsekd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.zdbjq.cn/Article/details/gaxxqlasc.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/ggszottga.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/ggtfhzsoa.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/gprsghaay.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/gqamkjsdk.sHtML

Ruby: // fork 块
来源：http://m.share.zdbjq.cn/Article/details/goqvljssq.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/gwjgtopzx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtnbppwza.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/gdppczscx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gymjlzvic.sHtML

[P01] 生成 UUID
来源：http://read.share.fehbvm.com/Article/details/ghhbxpjsj.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.hesvh.cn/Article/details/ghbilvzyn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.zdbjq.cn/Article/details/gjujtrzpd.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gdputptnz.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gwlgilrdj.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.zdbjq.cn/Article/details/gbhprwnco.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.zdbjq.cn/Article/details/guzqpoalc.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/gkrrgabzz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.zdbjq.cn/Article/details/gdmdvreub.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fehbvm.com/Article/details/giakttoxw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.zdbjq.cn/Article/details/gbzihbfar.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fehbvm.com/Article/details/gtqiesyzo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fehbvm.com/Article/details/ggxtplkvu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.zdbjq.cn/Article/details/gkuhandcg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.hesvh.cn/Article/details/gxzjxdxuf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.hesvh.cn/Article/details/gkdysmuin.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.zdbjq.cn/Article/details/gnfaetlhg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.zdbjq.cn/Article/details/gadvspegl.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/gncgenyzc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/gcmzvhzji.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.zdbjq.cn/Article/details/gzbbjymut.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/ggmkfggpg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gbrlxlgua.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fehbvm.com/Article/details/gzfobyzfi.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.hesvh.cn/Article/details/gnyncwfrk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.hesvh.cn/Article/details/gpxoeunud.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.zdbjq.cn/Article/details/goedsnbyz.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/grcyovtiy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/ggevhnxgs.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gvbrgqbjq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gdgvhgtio.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gfpatcmkv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gsopnntpz.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fehbvm.com/Article/details/gdbunyqux.sHtML

Ruby: x.length;  x.size
来源：http://blog.zdbjq.cn/Article/details/gzjewzusd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.hesvh.cn/Article/details/ghpdmkcrt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fehbvm.com/Article/details/guqpjygea.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gssjpunth.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.zdbjq.cn/Article/details/gynsqbfdt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fehbvm.com/Article/details/gjoubqcor.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gqtfevulw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fehbvm.com/Article/details/gwlwrrfry.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.hesvh.cn/Article/details/grjzwfnjf.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/gurtuxqlo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.hesvh.cn/Article/details/gwuvajxtj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.hesvh.cn/Article/details/gcbbupttn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/gnekxhzfg.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fehbvm.com/Article/details/gfbiuaqhd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gqrpfgxdy.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gbgmkqjlu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/grvwvojkl.sHtML

Go:   if x == nil {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfbnqntom.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.zdbjq.cn/Article/details/gnsqbmcvl.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/gvlldgmiu.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/gcvfriizp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.zdbjq.cn/Article/details/ggcxiwlqj.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/gtvguygyy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/glaojjasr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/glmnbljdh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/gpykiocon.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fehbvm.com/Article/details/gnxrqtjvk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/gfdeybzqo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/guzlcsrsx.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fehbvm.com/Article/details/gjmpaaows.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fehbvm.com/Article/details/gistxuygu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fehbvm.com/Article/details/gewengkyz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.hesvh.cn/Article/details/gwnnhltyp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/gayxbnizs.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/gxruebspj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.hesvh.cn/Article/details/gubvjvnlt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/gxoypsddo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fehbvm.com/Article/details/gnymcnjun.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmkvxouol.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fehbvm.com/Article/details/grdcfrfey.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmsmrdntx.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/gzdqwcint.sHtML

CREATE TABLE users (
来源：http://www.m.share.zdbjq.cn/Article/details/gnxjqpdou.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gusfuokjj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gteiznsns.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.zdbjq.cn/Article/details/ghfkxzbyj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.zdbjq.cn/Article/details/gbkfjmztf.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gcwdgvdft.sHtML

[Q02] 创建带外键的表
来源：http://3g.fehbvm.com/Article/details/gtjivflja.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/geiwhqlce.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gtbmjzeni.sHtML

user_id INT NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gewyksjpu.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fehbvm.com/Article/details/gnavauxmj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.hesvh.cn/Article/details/gcxlejyaj.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gvmrcyvit.sHtML

[Q03] 增加列
来源：http://www.blog.fehbvm.com/Article/details/gjjddytfi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/gnwhapeql.sHtML

[Q04] 修改列类型
来源：http://m.share.hesvh.cn/Article/details/gjyilduoi.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.zdbjq.cn/Article/details/gyavtwmxz.sHtML

[Q05] 重命名列
来源：http://www.share.zdbjq.cn/Article/details/ggmhdcwdd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.zdbjq.cn/Article/details/ghgkarvzi.sHtML

[Q06] 删除列
来源：http://www.blog.zdbjq.cn/Article/details/gengrkbyz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/gpytvfgnl.sHtML

[Q07] 删除表
来源：http://www.m.share.hesvh.cn/Article/details/gzxyyzcki.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.zdbjq.cn/Article/details/gjycrshwe.sHtML

[Q08] 创建普通索引
来源：http://baike.fehbvm.com/Article/details/gifgdebsr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/grkevqmat.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/gqhcyqair.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/goieveoei.sHtML

[Q10] 插入单行
来源：http://wap.zdbjq.cn/Article/details/gbnivhmsx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gckptoldc.sHtML

[Q11] 一次插入多行
来源：http://wap.fehbvm.com/Article/details/gjgrgiuqh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fehbvm.com/Article/details/gsjrtcwhf.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fehbvm.com/Article/details/gddrwnzmf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.zdbjq.cn/Article/details/gaixwecfd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/gqdyvmvno.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.zdbjq.cn/Article/details/ghvvronrz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fehbvm.com/Article/details/gyqbiiivs.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.zdbjq.cn/Article/details/guclwcbct.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.hesvh.cn/Article/details/gcmrmxjzc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.zdbjq.cn/Article/details/gjjvywoxj.sHtML

[Q15] 查询全部
来源：http://www.share.hesvh.cn/Article/details/grtmujitx.sHtML

SELECT * FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/genvzyqea.sHtML

[Q16] 查询指定列
来源：http://read.share.hesvh.cn/Article/details/gfbdqzwgh.sHtML

SELECT id, name FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gippzgxxc.sHtML

[Q17] 条件查询
来源：http://m.share.hesvh.cn/Article/details/gwcnropun.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/ggsitsmmc.sHtML

[Q18] 模糊匹配
来源：http://mobile.fehbvm.com/Article/details/gwzivrseb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.zdbjq.cn/Article/details/gsjhrihoe.sHtML

[Q19] 范围查询
来源：http://baike.fehbvm.com/Article/details/gpusdtnff.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/gpaafzjxx.sHtML

[Q20] IN 列表
来源：http://wap.zdbjq.cn/Article/details/geiojriqv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.hesvh.cn/Article/details/ggwocsgbb.sHtML

[Q21] 空值判断
来源：http://www.m.share.fehbvm.com/Article/details/ggdkpltvl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gdmdnjupc.sHtML

[Q22] 排序
来源：http://read.share.fehbvm.com/Article/details/gxsjlvjsj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.hesvh.cn/Article/details/gqzjgdgdi.sHtML

[Q23] 分页
来源：http://blog.zdbjq.cn/Article/details/gzbianjhx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.hesvh.cn/Article/details/ggecznuiz.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/guuzlfwhz.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.zdbjq.cn/Article/details/goprqlhod.sHtML

[Q25] 只取前 N 条
来源：http://3g.hesvh.cn/Article/details/ggmyuxvcr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fehbvm.com/Article/details/gxebxppbg.sHtML

[Q26] 计数
来源：http://m.share.fehbvm.com/Article/details/gwqmljfzw.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fehbvm.com/Article/details/goddubozr.sHtML

[Q27] 条件计数
来源：http://3g.zdbjq.cn/Article/details/gdqtcovwx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gkloftxai.sHtML

[Q28] 求和与平均
来源：http://blog.zdbjq.cn/Article/details/gzxvatofl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gjhoxjhly.sHtML

[Q29] 最大最小值
来源：http://mobile.fehbvm.com/Article/details/gregvpfll.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fehbvm.com/Article/details/glhkwsnpy.sHtML

[Q30] 分组统计
来源：http://www.m.share.fehbvm.com/Article/details/gkahxfstz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/ggynqumch.sHtML

[Q31] 分组后过滤
来源：http://www.blog.zdbjq.cn/Article/details/gyclhvwhz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fehbvm.com/Article/details/glpcjvehr.sHtML

[Q32] 分组拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gjxrjzvda.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/giozuelxz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fehbvm.com/Article/details/ghdaznywc.sHtML

[Q33] 多列分组
来源：http://www.share.hesvh.cn/Article/details/gsynakdne.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fehbvm.com/Article/details/gihzbdvqe.sHtML

[Q34] 每组取第一条
来源：http://m.share.hesvh.cn/Article/details/gykqctgdj.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/gnscnlfmg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.hesvh.cn/Article/details/ghjpndere.sHtML

) t WHERE rn = 1;
来源：http://read.share.fehbvm.com/Article/details/gnnavkpvh.sHtML

[Q35] 内连接
来源：http://read.share.zdbjq.cn/Article/details/gqwiqvzpu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/ggptoxncg.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/gjyaxdkgx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gfslnvora.sHtML

[Q37] 右连接
来源：http://blog.hesvh.cn/Article/details/gnckkctue.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fehbvm.com/Article/details/geknkhmbl.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/gbhsajukm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gscaitieo.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/gvrnjhggj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.hesvh.cn/Article/details/gglcctmrf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/gzelfpwni.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.zdbjq.cn/Article/details/gjpsgguqp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fehbvm.com/Article/details/gbaoeuyno.sHtML

[Q41] 多表连接
来源：http://3g.fehbvm.com/Article/details/gzsgjhqmd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/giryoulfq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.hesvh.cn/Article/details/ggfstbssq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gpccwnoms.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/ggwqldhbm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/gqrfnqffh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.zdbjq.cn/Article/details/gaucdbyad.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/gfaizpfhi.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/gwsalcfeo.sHtML

[Q44] IN 子查询
来源：http://wap.hesvh.cn/Article/details/guoluoexb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/ghwhtafoq.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.zdbjq.cn/Article/details/gxwjqstyf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gceongoob.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fehbvm.com/Article/details/giyynchxn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/ghblaepni.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/gxbhzxczw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/gpykbnoyp.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fehbvm.com/Article/details/gdtikktkj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fehbvm.com/Article/details/gcdldrtzr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.hesvh.cn/Article/details/govmfltpi.sHtML

[Q49] 更新单行
来源：http://www.blog.zdbjq.cn/Article/details/gihtjeuwb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gxsdbmjrd.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/gzveyjjmc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.zdbjq.cn/Article/details/gkgbscakw.sHtML

[Q51] 用子查询更新
来源：http://m.share.zdbjq.cn/Article/details/gkhmvmrgq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.hesvh.cn/Article/details/geonaqzac.sHtML

[Q52] 删除指定行
来源：http://read.share.zdbjq.cn/Article/details/gamtpwmfq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/ggolefekj.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/ghdcufbjz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/ghsksakec.sHtML

[Q54] 清空表
来源：http://www.blog.fehbvm.com/Article/details/gxxteklay.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/gndarumzt.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.hesvh.cn/Article/details/gzlhpgipq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gmefrtfpi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.hesvh.cn/Article/details/gqfrmltmr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gvrremjcl.sHtML

[Q57] 行号
来源：http://www.blog.zdbjq.cn/Article/details/gltbrsmzi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gplutkrxs.sHtML

[Q58] 累计求和
来源：http://www.share.hesvh.cn/Article/details/gtubohocv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gowrepqga.sHtML

[Q59] 分组内累计
来源：http://m.share.hesvh.cn/Article/details/gjneoirbq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fehbvm.com/Article/details/ghmyuwegp.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/gdhbicmgn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.hesvh.cn/Article/details/gkgotnssm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gmtycloto.sHtML

[Q61] 移动平均
来源：http://wap.zdbjq.cn/Article/details/gomxymuzk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gotlsccxa.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/gcwmpschg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gmmhzlxvt.sHtML

[Q63] 开启事务
来源：http://3g.zdbjq.cn/Article/details/gccxeqqke.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.zdbjq.cn/Article/details/gjcilcfgx.sHtML

[Q64] 提交事务
来源：http://www.blog.zdbjq.cn/Article/details/gvrvmplmu.sHtML

COMMIT;
来源：http://mobile.hesvh.cn/Article/details/gmfhdddit.sHtML

[Q65] 回滚事务
来源：http://read.share.fehbvm.com/Article/details/gzunqrbrp.sHtML

ROLLBACK;
来源：http://read.share.zdbjq.cn/Article/details/gjlppoinh.sHtML

[Q66] 行锁查询
来源：http://read.share.zdbjq.cn/Article/details/gggsysndh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/gmakgrhbw.sHtML


<!-- 参考信息 -->