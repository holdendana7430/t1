代发 wailian999

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/gpotsiogf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gmfswyxmm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gbowryvji.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/gdaohoavh.sHtML

Go:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gdudghvux.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/gbvuuxxcn.sHtML

C#:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gdwobwgjn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/gimlxleyk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fehbvm.com/Article/details/gvvdhyaqh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gdusyonzp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gacslojwu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gyrcajffa.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gucvsdlvn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/givcncvnf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/gwemzrjew.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/grvzkvraw.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghrkvweue.sHtML

O. 并发与异步
来源：http://read.share.hesvh.cn/Article/details/gqclyhhgq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxrvcwvyo.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/grnqtyayq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.hesvh.cn/Article/details/gybgfrwxd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/gpxeryeyl.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/galqncdih.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gdrpwomrg.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fehbvm.com/Article/details/geyjjpdcw.sHtML

Go:   go f()
来源：http://blog.fehbvm.com/Article/details/glywiiock.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gzhdozfgm.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/gjseudivo.sHtML

[O02] 使用线程池
来源：http://3g.fehbvm.com/Article/details/ghrlispck.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.zdbjq.cn/Article/details/gdvsyxdry.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/giypymscd.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gxwdsfpmr.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/ghkvqgffm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fehbvm.com/Article/details/gakxkvsnj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fehbvm.com/Article/details/ggksmjkcb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.fehbvm.com/Article/details/gwwpttxql.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.zdbjq.cn/Article/details/gliijfdym.sHtML

[O03] 加锁保护共享数据
来源：http://blog.hesvh.cn/Article/details/gcxbyzovw.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/gsnwbjfov.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fehbvm.com/Article/details/gsindhygx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/gqdbtqwae.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gnfovzsjp.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gsvlwsswk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.zdbjq.cn/Article/details/grnyirdon.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.hesvh.cn/Article/details/gtfktysxi.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gszczricr.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fehbvm.com/Article/details/gbkdeotyc.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fehbvm.com/Article/details/gxjkgcyle.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/gkczttbmu.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gbngcbbnj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fehbvm.com/Article/details/gjzormgpz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/gigfwtwto.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.hesvh.cn/Article/details/grkgseilz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gahymghhm.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fehbvm.com/Article/details/gyocwcvcp.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fehbvm.com/Article/details/gcjyyvyos.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/gdnbisdqy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.zdbjq.cn/Article/details/gnrxizozx.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gxyqwxpsf.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/ggzxstfuk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.hesvh.cn/Article/details/gbbkkxdvk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/gwqfosdee.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/gwejczfsg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/gdlxxsfmv.sHtML

[O06] 使用进程池
来源：http://3g.fehbvm.com/Article/details/gunyreuab.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.zdbjq.cn/Article/details/gqlitnfzl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/gwhtmmfci.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gswrttkcz.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gijqrxqjb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.zdbjq.cn/Article/details/girdxapgg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.zdbjq.cn/Article/details/gvfuwsppa.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/gfjzazwcg.sHtML

C#:   Parallel.For
来源：http://www.m.share.hesvh.cn/Article/details/giqhjftzq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpcorosfm.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/gcwnqopjp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwujkydqz.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gyvnlecnh.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/gncyodrjj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/gsowjqlhk.sHtML

JS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gmtrytuus.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gzobmtlvt.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.hesvh.cn/Article/details/gnjlibpts.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.zdbjq.cn/Article/details/gecnerzpz.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fehbvm.com/Article/details/gkjhocerx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.zdbjq.cn/Article/details/gshtgiacp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.hesvh.cn/Article/details/goykqzdin.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fehbvm.com/Article/details/gsnibixhv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.zdbjq.cn/Article/details/geviapebx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.zdbjq.cn/Article/details/gsqivjbwx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fehbvm.com/Article/details/glzbutewp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fehbvm.com/Article/details/gstjnhflw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.zdbjq.cn/Article/details/gtbshayoi.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fehbvm.com/Article/details/gfdxcenjb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/ggmvxdlgj.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/gqxmefdvy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fehbvm.com/Article/details/gehkbdoyi.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gdxuffajh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gmshiasnd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gmwafvgpf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.zdbjq.cn/Article/details/gsfzuwoea.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.hesvh.cn/Article/details/gjupamwvx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gvshsotae.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.zdbjq.cn/Article/details/gybkwdapg.sHtML

[P04] 求长度
来源：http://wap.fehbvm.com/Article/details/guywgvxqh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fehbvm.com/Article/details/ghgsdupdz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gmzvvguzk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/glmbvzwlc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gcybrfwho.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fehbvm.com/Article/details/gnpphcdvg.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fehbvm.com/Article/details/gkpduqvyn.sHtML

Ruby: x.length;  x.size
来源：http://baike.zdbjq.cn/Article/details/gtbupuswp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fehbvm.com/Article/details/gkaixlmki.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/gkwwfidnr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.zdbjq.cn/Article/details/gmyxtyquk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.hesvh.cn/Article/details/gzjfqxkph.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.zdbjq.cn/Article/details/gnbspxxog.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gcaawddon.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/gmaayfwwr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.hesvh.cn/Article/details/gahhvcyvg.sHtML

Ruby: a == b
来源：http://m.share.zdbjq.cn/Article/details/gsqvwsozt.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.zdbjq.cn/Article/details/gdatadqsx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.hesvh.cn/Article/details/gggefnfxk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fehbvm.com/Article/details/gzfuoyrkr.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/ggsajqlkh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.hesvh.cn/Article/details/gnpsnxhzs.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gssduwrrf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gcdmcuhap.sHtML

Go:   if x == nil {}
来源：http://www.m.share.zdbjq.cn/Article/details/gujqjbugj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.zdbjq.cn/Article/details/gqqyaiamp.sHtML

C#:   if (x is null) {}
来源：http://blog.hesvh.cn/Article/details/gswouqtvs.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/guufeilyt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.hesvh.cn/Article/details/grcsgscpw.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.hesvh.cn/Article/details/gjgpqgqew.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gsyunhitd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/ghdnpmrmz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.hesvh.cn/Article/details/gefugwymk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.zdbjq.cn/Article/details/gztagusko.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/gtovbxvvh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.zdbjq.cn/Article/details/gfbzaaqnl.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fehbvm.com/Article/details/gpcikcfpg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.hesvh.cn/Article/details/giejczsbp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fehbvm.com/Article/details/gowrcagwj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.hesvh.cn/Article/details/gbohqjtuf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gorshvzkh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.zdbjq.cn/Article/details/gbpmgsuot.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/guagmsukk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fehbvm.com/Article/details/gzhtkplta.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/gioxayekw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqdlknbkj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fehbvm.com/Article/details/guopvgkzc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcpircjcd.sHtML

[Q01] 创建表
来源：http://blog.hesvh.cn/Article/details/ggugjqroh.sHtML

CREATE TABLE users (
来源：http://baike.fehbvm.com/Article/details/gbppmooqa.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gxogostss.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/guaxujcaq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.zdbjq.cn/Article/details/giqczssgl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.hesvh.cn/Article/details/gjfeohbbf.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/guhngbzzo.sHtML

[Q02] 创建带外键的表
来源：http://blog.hesvh.cn/Article/details/gvklkykiw.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fehbvm.com/Article/details/gypsszhpu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gbodokzqw.sHtML

user_id INT NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gemmnzyiu.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.hesvh.cn/Article/details/gtwuyfvgf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.hesvh.cn/Article/details/gxgubqalt.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gwzybwuoi.sHtML

[Q03] 增加列
来源：http://wap.hesvh.cn/Article/details/gmcvccyhc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fehbvm.com/Article/details/gdxqhfrik.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/gxkhhpiiw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gcccjwxrs.sHtML

[Q05] 重命名列
来源：http://read.share.hesvh.cn/Article/details/glywtjyig.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.hesvh.cn/Article/details/gbrxxscpf.sHtML

[Q06] 删除列
来源：http://wap.zdbjq.cn/Article/details/gsmorrfqd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.zdbjq.cn/Article/details/gxpzviffg.sHtML

[Q07] 删除表
来源：http://read.share.zdbjq.cn/Article/details/gfzjsmybq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gqnrsonog.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fehbvm.com/Article/details/ggehbjoni.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gdjkmjnrj.sHtML

[Q09] 创建唯一索引
来源：http://blog.fehbvm.com/Article/details/gurpettsd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gokoavnns.sHtML

[Q10] 插入单行
来源：http://m.share.zdbjq.cn/Article/details/gkkxauqwx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fehbvm.com/Article/details/gytoefgqu.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/gbqvyqodr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/guioawdoa.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.hesvh.cn/Article/details/gsuzgzdrf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.hesvh.cn/Article/details/gphqyfekc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fehbvm.com/Article/details/grusnsoqy.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fehbvm.com/Article/details/gynqocyfy.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.hesvh.cn/Article/details/gjoqbapue.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.hesvh.cn/Article/details/glvourjug.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fehbvm.com/Article/details/gpxoixtyw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.zdbjq.cn/Article/details/goqpquxoe.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/gzyphgkkd.sHtML

SELECT * FROM users;
来源：http://baike.fehbvm.com/Article/details/giefupcld.sHtML

[Q16] 查询指定列
来源：http://blog.fehbvm.com/Article/details/gsioclcsb.sHtML

SELECT id, name FROM users;
来源：http://blog.zdbjq.cn/Article/details/gjfdwpiiq.sHtML

[Q17] 条件查询
来源：http://blog.zdbjq.cn/Article/details/ggmpikuly.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fehbvm.com/Article/details/gdtkwhump.sHtML

[Q18] 模糊匹配
来源：http://blog.zdbjq.cn/Article/details/gipxboapr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.zdbjq.cn/Article/details/gehhtaekf.sHtML

[Q19] 范围查询
来源：http://www.blog.zdbjq.cn/Article/details/gtbageyxz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.hesvh.cn/Article/details/gwhskpwex.sHtML

[Q20] IN 列表
来源：http://mobile.zdbjq.cn/Article/details/gywinagzx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/ghiuqdblr.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/gqicgjeem.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fehbvm.com/Article/details/griuwwcun.sHtML

[Q22] 排序
来源：http://mobile.zdbjq.cn/Article/details/glymlzkbd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fehbvm.com/Article/details/gdhjgeyip.sHtML

[Q23] 分页
来源：http://read.share.fehbvm.com/Article/details/gwixtixau.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.zdbjq.cn/Article/details/gwbqotxva.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/gqsxhaaqy.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/glaeekgrp.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/gamsfrcqk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.zdbjq.cn/Article/details/gkyzevgtf.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/gqxwihdjk.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/gccjspfva.sHtML

[Q27] 条件计数
来源：http://www.share.zdbjq.cn/Article/details/gqcxlmemr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.hesvh.cn/Article/details/gtbyhetww.sHtML

[Q28] 求和与平均
来源：http://baike.zdbjq.cn/Article/details/galywwvka.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.hesvh.cn/Article/details/glggmsyrz.sHtML

[Q29] 最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/gjlogkcda.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fehbvm.com/Article/details/gjiogkiqn.sHtML

[Q30] 分组统计
来源：http://mobile.hesvh.cn/Article/details/gieailsiq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/ghjjjtejr.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/gifgucihe.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.zdbjq.cn/Article/details/giscovabp.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.hesvh.cn/Article/details/givnvdtui.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gvchemcaj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fehbvm.com/Article/details/gyhfbrifd.sHtML

[Q33] 多列分组
来源：http://3g.hesvh.cn/Article/details/gqhwxslhu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.zdbjq.cn/Article/details/gofflgxyx.sHtML

[Q34] 每组取第一条
来源：http://mobile.hesvh.cn/Article/details/gmelkirtr.sHtML

SELECT * FROM (
来源：http://wap.zdbjq.cn/Article/details/gemghftxd.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fehbvm.com/Article/details/gfittfkut.sHtML

) t WHERE rn = 1;
来源：http://www.share.fehbvm.com/Article/details/gwytvsdjg.sHtML

[Q35] 内连接
来源：http://www.share.zdbjq.cn/Article/details/gcalkevmw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gsesnqmju.sHtML

[Q36] 左连接
来源：http://blog.fehbvm.com/Article/details/gjwqshggy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gzvwcbptv.sHtML

[Q37] 右连接
来源：http://baike.hesvh.cn/Article/details/gievczqov.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/gkznivcay.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.hesvh.cn/Article/details/gfgsqhxlc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/ggvhreqsx.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fehbvm.com/Article/details/gaxoocicp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fehbvm.com/Article/details/gtyjejafn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gnfnhvwsn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.zdbjq.cn/Article/details/gxaphnesx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fehbvm.com/Article/details/gmajcatlj.sHtML

[Q41] 多表连接
来源：http://www.blog.fehbvm.com/Article/details/gkiiydoot.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fehbvm.com/Article/details/glxkszdkl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/gywovlyzw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.hesvh.cn/Article/details/gkgcqkzcw.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.zdbjq.cn/Article/details/gpbqekmzc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fehbvm.com/Article/details/gyovpmdqh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.zdbjq.cn/Article/details/gxagwzfjh.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/gjbomrhzz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.hesvh.cn/Article/details/gvgwvwgxn.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gwlvjnaml.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.hesvh.cn/Article/details/gmswyksrw.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.hesvh.cn/Article/details/gmvcpfkvf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gelwgzgha.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fehbvm.com/Article/details/ghtbyhneu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gtxczhmcn.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/gbgraatnq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.hesvh.cn/Article/details/gvgyqkije.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fehbvm.com/Article/details/gcqbsvstq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.hesvh.cn/Article/details/gdpjkexjv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fehbvm.com/Article/details/gbfcmciqb.sHtML

[Q49] 更新单行
来源：http://mobile.fehbvm.com/Article/details/gfdphurzl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/glnpxztto.sHtML

[Q50] 批量更新
来源：http://read.share.fehbvm.com/Article/details/gbnkscnsc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fehbvm.com/Article/details/gfrygnzbh.sHtML

[Q51] 用子查询更新
来源：http://baike.fehbvm.com/Article/details/gndjydivx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gedlcpmcf.sHtML

[Q52] 删除指定行
来源：http://blog.fehbvm.com/Article/details/gttutbpgj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gylgqiawq.sHtML

[Q53] 按条件删除
来源：http://read.share.fehbvm.com/Article/details/gdynmlnba.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fehbvm.com/Article/details/gmwuaxbeb.sHtML

[Q54] 清空表
来源：http://blog.zdbjq.cn/Article/details/gwdktomap.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/gummzefxu.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/gxnxorfhi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gotwceghr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/gqkhgjkme.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fehbvm.com/Article/details/gimzjgsud.sHtML

[Q57] 行号
来源：http://www.m.share.hesvh.cn/Article/details/gxaehoavz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gholnphsl.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/gkycmkqfn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.hesvh.cn/Article/details/gibqwjbxh.sHtML

[Q59] 分组内累计
来源：http://baike.hesvh.cn/Article/details/gdjojpnzv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gqxtstcwj.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.hesvh.cn/Article/details/gauacyzcj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/gmftpncfo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gnmjabytw.sHtML

[Q61] 移动平均
来源：http://www.m.share.hesvh.cn/Article/details/gynapxopm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gmsgsjwak.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/giirrewwc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gvyxdwjjh.sHtML

[Q63] 开启事务
来源：http://mobile.fehbvm.com/Article/details/gnfndlqcc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.hesvh.cn/Article/details/gduotmllu.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/gsapmtisr.sHtML

COMMIT;
来源：http://3g.fehbvm.com/Article/details/gazdlctis.sHtML


<!-- 参考信息 -->