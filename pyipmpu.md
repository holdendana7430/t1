代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/gyvjfdcsy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.zdbjq.cn/Article/details/gggmvitob.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/gkcrbkenn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/glpdzdvxz.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.hesvh.cn/Article/details/ghgbfiwxi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gvhecnomb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gxsglvrll.sHtML

Java: // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gwfmemaat.sHtML

Go:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gmrckbtqk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.hesvh.cn/Article/details/gcxqxcrax.sHtML

C#:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gsdwmujjq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/gmekxflex.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/gcolgpfpj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.zdbjq.cn/Article/details/gataygqmh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gqivsvcqz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gurdtrzib.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gujibdxyn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/gsmlbvpma.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.hesvh.cn/Article/details/gzfexncfm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gbizpyfok.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfxyamagm.sHtML

O. 并发与异步
来源：http://baike.fehbvm.com/Article/details/gszgcxofj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggwvdzgdn.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/gygsxsujs.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fehbvm.com/Article/details/guetesllq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gozmqczwt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/gjentrims.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gaadizbom.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/galuiijnc.sHtML

Go:   go f()
来源：http://www.blog.fehbvm.com/Article/details/gwbfpdovd.sHtML

Ruby: Thread.new { f }
来源：http://blog.zdbjq.cn/Article/details/gwwcmdjnl.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fehbvm.com/Article/details/gwmxbzhhn.sHtML

[O02] 使用线程池
来源：http://mobile.zdbjq.cn/Article/details/ghvebpbck.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fehbvm.com/Article/details/gllifecqt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/gqmzlsloo.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gzpcvgdvv.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/getoxoblu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.zdbjq.cn/Article/details/gcclxsbnz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.hesvh.cn/Article/details/gpjhsblxs.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/govrozkll.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fehbvm.com/Article/details/gwfvislkr.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/ghamomaot.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fehbvm.com/Article/details/gtnkhxsgb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.hesvh.cn/Article/details/gwjxjecdr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fehbvm.com/Article/details/gtaydqrtc.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gifmenolm.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/geilvbwfj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/gamtqyxkz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/gegzujtev.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gymgofeay.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.zdbjq.cn/Article/details/gploxxrlq.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/ghekubtue.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/gpblaiuyf.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gmrjrwgrr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gnhpvwnyv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fehbvm.com/Article/details/gqvduhygx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fehbvm.com/Article/details/gljnyajos.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.zdbjq.cn/Article/details/gguzhwdzn.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.hesvh.cn/Article/details/gctxwvdue.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.zdbjq.cn/Article/details/gourngwda.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/ghiigbvyi.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.hesvh.cn/Article/details/gsoanvxhx.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/glewlyhjj.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gmxplaysb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fehbvm.com/Article/details/gvmveqvsb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.zdbjq.cn/Article/details/gfjyibsvt.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gpvqjbfjm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.zdbjq.cn/Article/details/gqfghjnam.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/gjdkgxzrg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fehbvm.com/Article/details/grvepzwzj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fehbvm.com/Article/details/gasotpkxr.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gzrdcaxrx.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gjflhukya.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/gvpylmoue.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.hesvh.cn/Article/details/gkpfwvvtg.sHtML

Ruby: // fork 块
来源：http://www.share.fehbvm.com/Article/details/gocfwyglk.sHtML

C#:   Parallel.For
来源：http://read.share.fehbvm.com/Article/details/gszhhjfuw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpmprvfcq.sHtML

P. 常用工具函数
来源：http://www.m.share.hesvh.cn/Article/details/gffycowek.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gnzfvtxqj.sHtML

[P01] 生成 UUID
来源：http://baike.hesvh.cn/Article/details/gveekomfi.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.hesvh.cn/Article/details/gaemwcaou.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/galkcervl.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gedvymgea.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gqvzteguf.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/gzcvperym.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.zdbjq.cn/Article/details/gxgsldxow.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fehbvm.com/Article/details/gbnmkykpy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/gvzahjsxa.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/gstrnmaic.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.zdbjq.cn/Article/details/giwgpvupp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/gchnptyij.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fehbvm.com/Article/details/gpfpgokqj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/gellqzfcz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fehbvm.com/Article/details/gchtjxyyv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/gjromvaxq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.hesvh.cn/Article/details/gykgzuowh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fehbvm.com/Article/details/gxhpavjqj.sHtML

[P03] 生成短随机字符串
来源：http://blog.zdbjq.cn/Article/details/gzzvqedci.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/gsyijcioh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fehbvm.com/Article/details/gnwehkqxs.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/ggxbzcbmx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gwecmwfie.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.zdbjq.cn/Article/details/ghabnzrog.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fehbvm.com/Article/details/ggbhpsrho.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/gwvgjnsgv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.hesvh.cn/Article/details/gglysidba.sHtML

[P04] 求长度
来源：http://www.share.fehbvm.com/Article/details/gheovgqqq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.fehbvm.com/Article/details/gyzhurwrh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gaqcisrbf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gapfhevgj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gabwaubvk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.zdbjq.cn/Article/details/gqbuslwpy.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.zdbjq.cn/Article/details/gdahtdamw.sHtML

Ruby: x.length;  x.size
来源：http://www.share.zdbjq.cn/Article/details/gngatihce.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gcbvzgsez.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.zdbjq.cn/Article/details/gbhapwoxw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.hesvh.cn/Article/details/ghqstlvbs.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.zdbjq.cn/Article/details/gwfslxygk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.zdbjq.cn/Article/details/glnnvnmvf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/ghvmdqnur.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/gpcvtfota.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.hesvh.cn/Article/details/grpifydgi.sHtML

Ruby: a == b
来源：http://www.m.share.zdbjq.cn/Article/details/gsuejfnjn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fehbvm.com/Article/details/gauzgoixu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.zdbjq.cn/Article/details/gniulcmdm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/gjemwrovu.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gojzpnfrx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/glqsgwjjo.sHtML

TS:   if (x == null) {}
来源：http://wap.hesvh.cn/Article/details/gdqlbunxh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gzbcpezei.sHtML

Go:   if x == nil {}
来源：http://blog.hesvh.cn/Article/details/gxjipkfch.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.zdbjq.cn/Article/details/gtxvmuwoh.sHtML

C#:   if (x is null) {}
来源：http://blog.hesvh.cn/Article/details/glsqsnevl.sHtML

[P07] 防抖与节流
来源：http://3g.zdbjq.cn/Article/details/gijozbrun.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fehbvm.com/Article/details/gxweyaigg.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fehbvm.com/Article/details/gjigtchqs.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gtuczbwwl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gyrvpliwx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fehbvm.com/Article/details/gxokknwrp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/gqooqdwde.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.zdbjq.cn/Article/details/giccbthzu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.zdbjq.cn/Article/details/gbeurhllb.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/gmyapsvsa.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.hesvh.cn/Article/details/gkzhkgvwb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/gsahprccm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.hesvh.cn/Article/details/gjolfqqdf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/genwpsgez.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.zdbjq.cn/Article/details/gpyuiwxfz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.zdbjq.cn/Article/details/gwljnbcgl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.hesvh.cn/Article/details/gywcgcvim.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/gyghgiexk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmmkobhxw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.zdbjq.cn/Article/details/geieploxy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gamptdyzl.sHtML

[Q01] 创建表
来源：http://3g.zdbjq.cn/Article/details/gonxykivn.sHtML

CREATE TABLE users (
来源：http://blog.fehbvm.com/Article/details/gkmfsvfiv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gqmmyztii.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gwguzlizk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.hesvh.cn/Article/details/gxmantvek.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.zdbjq.cn/Article/details/gplrmzzjn.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gwyovviea.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.hesvh.cn/Article/details/gfytlqxva.sHtML

CREATE TABLE orders (
来源：http://blog.hesvh.cn/Article/details/gsejomdpx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gdmrgrbkt.sHtML

user_id INT NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gkbszxrls.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/geuzpfbaq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/gdshilhxv.sHtML

);
来源：http://blog.hesvh.cn/Article/details/geuagmihd.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/gyhtbvmic.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fehbvm.com/Article/details/gtyibolkw.sHtML

[Q04] 修改列类型
来源：http://www.m.share.zdbjq.cn/Article/details/gadzqacia.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fehbvm.com/Article/details/gitltjtqq.sHtML

[Q05] 重命名列
来源：http://blog.zdbjq.cn/Article/details/gssnntfwd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fehbvm.com/Article/details/gmjykbzrd.sHtML

[Q06] 删除列
来源：http://mobile.zdbjq.cn/Article/details/gyrohxczk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fehbvm.com/Article/details/gwccmtsyq.sHtML

[Q07] 删除表
来源：http://m.share.fehbvm.com/Article/details/grncjjzsm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.zdbjq.cn/Article/details/gnvcbqmep.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fehbvm.com/Article/details/gohlvrkgl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gxcxtxaov.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/gkfiaqlff.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gbuqidoyu.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/ghbnritys.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/gfmywcdlq.sHtML

[Q11] 一次插入多行
来源：http://mobile.hesvh.cn/Article/details/gccmfvyfs.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.hesvh.cn/Article/details/gtsosfvyb.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fehbvm.com/Article/details/glwcfildy.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fehbvm.com/Article/details/gwvourueb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/gtknrvmct.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.zdbjq.cn/Article/details/geixdhzoq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.zdbjq.cn/Article/details/gqtadnijt.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.zdbjq.cn/Article/details/giifcrxty.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.zdbjq.cn/Article/details/gkrpkjtiw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.hesvh.cn/Article/details/gzaqopjnt.sHtML

[Q15] 查询全部
来源：http://blog.fehbvm.com/Article/details/gwxlldczz.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/gyjzhyfig.sHtML

[Q16] 查询指定列
来源：http://baike.fehbvm.com/Article/details/gdolzxrrs.sHtML

SELECT id, name FROM users;
来源：http://read.share.zdbjq.cn/Article/details/ghaaqmapg.sHtML

[Q17] 条件查询
来源：http://baike.hesvh.cn/Article/details/gluuatxjc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.zdbjq.cn/Article/details/gnxuyuxuf.sHtML

[Q18] 模糊匹配
来源：http://baike.fehbvm.com/Article/details/gppabakrv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/gftisjonb.sHtML

[Q19] 范围查询
来源：http://www.share.fehbvm.com/Article/details/gbceuuhal.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/gvgalekng.sHtML

[Q20] IN 列表
来源：http://read.share.zdbjq.cn/Article/details/gsqojfhli.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gqsqaoynj.sHtML

[Q21] 空值判断
来源：http://www.blog.fehbvm.com/Article/details/grcyuzvux.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.zdbjq.cn/Article/details/gtpfckoiq.sHtML

[Q22] 排序
来源：http://mobile.zdbjq.cn/Article/details/gexeijsme.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.hesvh.cn/Article/details/gtfsdenlk.sHtML

[Q23] 分页
来源：http://mobile.zdbjq.cn/Article/details/ghzapbzcg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.zdbjq.cn/Article/details/guhpjjywj.sHtML

[Q24] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gkujcigtm.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fehbvm.com/Article/details/gulffxqhk.sHtML

[Q25] 只取前 N 条
来源：http://baike.hesvh.cn/Article/details/graqwjsux.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/gbdxtgsye.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/gecowityy.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.hesvh.cn/Article/details/gtiapctao.sHtML

[Q27] 条件计数
来源：http://www.share.fehbvm.com/Article/details/gvswqupof.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fehbvm.com/Article/details/glpflayfc.sHtML

[Q28] 求和与平均
来源：http://www.m.share.zdbjq.cn/Article/details/gtotgsooz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/glzfuzeul.sHtML

[Q29] 最大最小值
来源：http://read.share.hesvh.cn/Article/details/gjolwqfhj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gfonvsykz.sHtML

[Q30] 分组统计
来源：http://m.share.hesvh.cn/Article/details/ghgnyisze.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gmwtqeoli.sHtML

[Q31] 分组后过滤
来源：http://3g.hesvh.cn/Article/details/gidlmsica.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fehbvm.com/Article/details/gwhbakowm.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/glyyswdzv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gbdunmfzm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fehbvm.com/Article/details/gcnyquizp.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/gdfhdgeaj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/gkymlwnvv.sHtML

[Q34] 每组取第一条
来源：http://read.share.fehbvm.com/Article/details/gbkpueaiw.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/guoditfsf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.zdbjq.cn/Article/details/gzktwwnnr.sHtML

) t WHERE rn = 1;
来源：http://mobile.hesvh.cn/Article/details/grmbbqmya.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/gyqdnatss.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/glgkjsedc.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/gapxelpnk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gaerijgml.sHtML

[Q37] 右连接
来源：http://m.share.zdbjq.cn/Article/details/gjtlqjkea.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.zdbjq.cn/Article/details/gfbdkwuyk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.zdbjq.cn/Article/details/ggefjythc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.hesvh.cn/Article/details/gveipiong.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.hesvh.cn/Article/details/gdvbxpsmp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/gcjjntkgz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/gvdjmwweb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.hesvh.cn/Article/details/gxlgibmxi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fehbvm.com/Article/details/gnztuiozr.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/ghcdavrst.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/getimuhzj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/gdlhmcueg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.hesvh.cn/Article/details/gmgnfefgc.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fehbvm.com/Article/details/ggifbxaun.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.hesvh.cn/Article/details/ggnxdzmyt.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.zdbjq.cn/Article/details/gkmgowwfv.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/grdiorgfs.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/gozwfrlcn.sHtML

[Q44] IN 子查询
来源：http://baike.fehbvm.com/Article/details/gwqjahake.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fehbvm.com/Article/details/gdgrvaalv.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.zdbjq.cn/Article/details/goekbehwg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gqgxcjbsb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/gmlwayaxi.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/geoxzbnrl.sHtML

[Q47] 与平均值比较
来源：http://wap.fehbvm.com/Article/details/gbyagtpoc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.zdbjq.cn/Article/details/gxznunxpv.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.hesvh.cn/Article/details/gtrxjapzi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fehbvm.com/Article/details/grchxbysc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.hesvh.cn/Article/details/gncngwvre.sHtML

[Q49] 更新单行
来源：http://m.share.fehbvm.com/Article/details/gshihkzoy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gidjpiiwm.sHtML

[Q50] 批量更新
来源：http://wap.fehbvm.com/Article/details/ghknuprru.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gafopzvyd.sHtML

[Q51] 用子查询更新
来源：http://www.blog.hesvh.cn/Article/details/gyneakckt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fehbvm.com/Article/details/grzxdcigl.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/gwzviiser.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gfsywkziy.sHtML

[Q53] 按条件删除
来源：http://baike.hesvh.cn/Article/details/glemycbnc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.hesvh.cn/Article/details/glkcrsiwz.sHtML

[Q54] 清空表
来源：http://www.blog.hesvh.cn/Article/details/gwapyprsk.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/gefmkojrz.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/gsxnsdtve.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/glzfqakvs.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/gkeurgasy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gevafjoro.sHtML

[Q57] 行号
来源：http://blog.hesvh.cn/Article/details/gvvlgleub.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gzxaoqnxn.sHtML

[Q58] 累计求和
来源：http://m.share.fehbvm.com/Article/details/gcovhdkrs.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gegatsfuc.sHtML

[Q59] 分组内累计
来源：http://wap.zdbjq.cn/Article/details/ggsnhsrex.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gjjczvfmq.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.zdbjq.cn/Article/details/gdvidxoti.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fehbvm.com/Article/details/gxdixghjy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.hesvh.cn/Article/details/gvqoebmpl.sHtML

[Q61] 移动平均
来源：http://wap.fehbvm.com/Article/details/gzhddqlow.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gbhgqlkej.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/gudlrorpm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gkxndntnz.sHtML


<!-- 参考信息 -->