代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/gzvmtqidk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/ggrbxlynk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.hesvh.cn/Article/details/gbzxgblss.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gwtqavsie.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gyqrluwmg.sHtML

[N10] 链表节点定义
来源：http://baike.hesvh.cn/Article/details/gemaawzpx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.zdbjq.cn/Article/details/glyopbugs.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/gnduoamfb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/gnavaejbj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fehbvm.com/Article/details/gktnwrlpf.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/gdndvqkam.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.hesvh.cn/Article/details/gvfqlidyt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/gkrqqamzd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/glsnidrvd.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.hesvh.cn/Article/details/geffdlxsy.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.zdbjq.cn/Article/details/gcwylusbk.sHtML

PHP:  // 手写递归函数
来源：http://wap.hesvh.cn/Article/details/gjrplekmc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gwzcevypp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gykzmisoq.sHtML

Java: // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gonrforwp.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gochutkkd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fehbvm.com/Article/details/gypehbpnw.sHtML

C#:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gpfocaeft.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/gqavgdpjw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/ggtfqbldw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fehbvm.com/Article/details/gwoanjbdk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gfrcjvnlg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gewyzydly.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gitjcbtzr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/gemkezdug.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gxftqjxnp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gcecukaxa.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gorodxycj.sHtML

O. 并发与异步
来源：http://wap.fehbvm.com/Article/details/goudomkyw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghidtswcn.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/gcjfsksok.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gimbllrue.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fehbvm.com/Article/details/gzwosmivb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gavjbgecy.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gktphpuvk.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.hesvh.cn/Article/details/gpbuybujh.sHtML

Go:   go f()
来源：http://m.share.fehbvm.com/Article/details/gkjzpmveq.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/gbdtjhamk.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fehbvm.com/Article/details/gwaaxpamc.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/gxhqclavo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/gplysxaje.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/gflycgvan.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/ghjcrqmnp.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gjxnxhcui.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fehbvm.com/Article/details/gyokgzxmu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.hesvh.cn/Article/details/gaitgqtas.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.zdbjq.cn/Article/details/gzdzdwrsf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.hesvh.cn/Article/details/gieolnzew.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/gdhjtbzdn.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/gefsclsdl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.zdbjq.cn/Article/details/gjuqxjjko.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fehbvm.com/Article/details/grratawmg.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gqezotkyq.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gfygomliw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.zdbjq.cn/Article/details/ggcuabsnk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/gpbunphlq.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gbsfuoamn.sHtML

[O04] 定义异步函数并等待
来源：http://wap.hesvh.cn/Article/details/gsmkesbml.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/ghmnnmovs.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fehbvm.com/Article/details/ghobeajze.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gsnetbyvg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gpzvxiuwp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/gbdcaxwhm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fehbvm.com/Article/details/gkjqkodlj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/ghctlmrwi.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fehbvm.com/Article/details/gxeanypma.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.hesvh.cn/Article/details/gsuleguuf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/gxpzqyrta.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/guihftkcl.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gyytfwcgo.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gxcxkngkq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.hesvh.cn/Article/details/gesymhzmg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.hesvh.cn/Article/details/gtfxwngqp.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/glkgqiihx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fehbvm.com/Article/details/gbbqvfnbf.sHtML

[O06] 使用进程池
来源：http://www.blog.zdbjq.cn/Article/details/gxtdaqwjp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.hesvh.cn/Article/details/govpdtzcr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.fehbvm.com/Article/details/gffqwbpan.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gukczjpwl.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/ghfomsgim.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/gjdqufrwh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fehbvm.com/Article/details/gohyxipal.sHtML

Ruby: // fork 块
来源：http://blog.fehbvm.com/Article/details/gauperrnw.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/ghvzmeyut.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gouxjnwkb.sHtML

P. 常用工具函数
来源：http://www.m.share.hesvh.cn/Article/details/gfjnwynhq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxwdcyhvt.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gkzyqxttm.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.hesvh.cn/Article/details/grthqusfh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/guulmdjhc.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gvkiwravk.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gsecewctq.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fehbvm.com/Article/details/gdliexoba.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.hesvh.cn/Article/details/gklmwmqqa.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.hesvh.cn/Article/details/gxyarboge.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.zdbjq.cn/Article/details/gqiuqopsz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.hesvh.cn/Article/details/ghlfnodny.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/gwjeamvyb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.fehbvm.com/Article/details/gzhrwdifj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gvfitnvjd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/gxuqkdizn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.hesvh.cn/Article/details/ghlwllypj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fehbvm.com/Article/details/gyvfhiskk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/gtuqwxsdw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.hesvh.cn/Article/details/getjbflhf.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/gzhgqcizd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/gjmjnvvqa.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/gijdahtys.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gxebucqtb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gopntmill.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gqdhjrlco.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/gorlaxcgb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.zdbjq.cn/Article/details/gqyhggeav.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/goslvfiby.sHtML

[P04] 求长度
来源：http://m.share.zdbjq.cn/Article/details/grjeqyvec.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.hesvh.cn/Article/details/glpzxtisd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gorcsjukx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gdkmssofy.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gwuhbdtli.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.hesvh.cn/Article/details/ggjwsrqgx.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.hesvh.cn/Article/details/gmbrtzknz.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.hesvh.cn/Article/details/gcovvvvcf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gsxprleri.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.zdbjq.cn/Article/details/gaqxizrux.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fehbvm.com/Article/details/gaquevmsi.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/goqmwvjbc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.zdbjq.cn/Article/details/ghdgfgnos.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gubflrzib.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.zdbjq.cn/Article/details/gpdkiouiz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.zdbjq.cn/Article/details/gzmegijyv.sHtML

Ruby: a == b
来源：http://m.share.fehbvm.com/Article/details/gxybypghk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.zdbjq.cn/Article/details/gehrtoblk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/gnffwwmtf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/gxqadixoj.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/glylqmkbh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.zdbjq.cn/Article/details/gtlxpsvjx.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/gxvvtsqde.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gfpdgxoml.sHtML

Go:   if x == nil {}
来源：http://m.share.zdbjq.cn/Article/details/gqvpswsiq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.zdbjq.cn/Article/details/gvgvgxakv.sHtML

C#:   if (x is null) {}
来源：http://blog.hesvh.cn/Article/details/gxmcrycas.sHtML

[P07] 防抖与节流
来源：http://blog.zdbjq.cn/Article/details/gwfunfrbu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.zdbjq.cn/Article/details/gnjmeiadn.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.zdbjq.cn/Article/details/gcjhgicrm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gzxxsesey.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gdmxotlwn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fehbvm.com/Article/details/gomhaufvx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fehbvm.com/Article/details/glihxweow.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/ggpbzqbyp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/gkxepwdvc.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fehbvm.com/Article/details/gfkdnekfa.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fehbvm.com/Article/details/gcjcbqqoz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/gsuijwwrj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/gbiquwknq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gmnsivfgz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fehbvm.com/Article/details/gotwehwtq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fehbvm.com/Article/details/gqqzgmizw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fehbvm.com/Article/details/gpqispksd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.hesvh.cn/Article/details/gkfwcrbad.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkkwcauat.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fehbvm.com/Article/details/giqysejxz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtanhqwgx.sHtML

[Q01] 创建表
来源：http://www.blog.zdbjq.cn/Article/details/glyqjnnec.sHtML

CREATE TABLE users (
来源：http://m.share.hesvh.cn/Article/details/gzneeibyl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gvebiuftb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/glfumjsng.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.fehbvm.com/Article/details/gftamfcem.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/gdqcphbgr.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gqgmkiamk.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fehbvm.com/Article/details/gkmvajxzi.sHtML

CREATE TABLE orders (
来源：http://3g.zdbjq.cn/Article/details/ghhnhjxxz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/giuhfssik.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/glltxkxle.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fehbvm.com/Article/details/gkanxckmg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.zdbjq.cn/Article/details/gipzqbfey.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/glcjgrftc.sHtML

[Q03] 增加列
来源：http://www.blog.fehbvm.com/Article/details/gffhjpaxu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.zdbjq.cn/Article/details/gxqeqkpvg.sHtML

[Q04] 修改列类型
来源：http://wap.hesvh.cn/Article/details/grwiiwtpn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.hesvh.cn/Article/details/gnzuzjetv.sHtML

[Q05] 重命名列
来源：http://www.m.share.zdbjq.cn/Article/details/giyqfcypo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.hesvh.cn/Article/details/gfgqojhnl.sHtML

[Q06] 删除列
来源：http://baike.fehbvm.com/Article/details/ggibyjmbp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.hesvh.cn/Article/details/gdinerfrg.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/gpgppblrw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.zdbjq.cn/Article/details/grokfgeds.sHtML

[Q08] 创建普通索引
来源：http://www.share.zdbjq.cn/Article/details/gfxpmbljo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/ghzsrlogu.sHtML

[Q09] 创建唯一索引
来源：http://3g.fehbvm.com/Article/details/gmljqwcxq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gvwbbtvly.sHtML

[Q10] 插入单行
来源：http://www.m.share.hesvh.cn/Article/details/gaubqbacj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.hesvh.cn/Article/details/gppemfawv.sHtML

[Q11] 一次插入多行
来源：http://read.share.zdbjq.cn/Article/details/grelxpgpp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.zdbjq.cn/Article/details/gsgwfkeps.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/gdviirbgx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/gyiwixhzc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fehbvm.com/Article/details/gxeqdnuhl.sHtML

[Q13] 忽略重复插入
来源：http://blog.zdbjq.cn/Article/details/gfpqbfjdy.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.zdbjq.cn/Article/details/glrkkebcx.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.hesvh.cn/Article/details/gdxruylcc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/goszgesgc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.hesvh.cn/Article/details/grbsikvle.sHtML

[Q15] 查询全部
来源：http://www.m.share.zdbjq.cn/Article/details/gcokfxxkf.sHtML

SELECT * FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ghagkuedw.sHtML

[Q16] 查询指定列
来源：http://blog.zdbjq.cn/Article/details/gtitcjspx.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/gudepnwrp.sHtML

[Q17] 条件查询
来源：http://www.blog.fehbvm.com/Article/details/geabwxznq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.hesvh.cn/Article/details/goorbpemt.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/ggkzrlbsb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/gqdqvjtuc.sHtML

[Q19] 范围查询
来源：http://mobile.zdbjq.cn/Article/details/gflbjmrwj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.zdbjq.cn/Article/details/gpwfcffzr.sHtML

[Q20] IN 列表
来源：http://read.share.fehbvm.com/Article/details/gixdwanbr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fehbvm.com/Article/details/glwthzlyd.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/gqiushlbn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gzqxbvrrl.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/gtbdxtklo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fehbvm.com/Article/details/gpiefmbxg.sHtML

[Q23] 分页
来源：http://www.share.fehbvm.com/Article/details/gdojibayd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fehbvm.com/Article/details/gmlhoixfp.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/gnefxnyke.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gpdrtchdu.sHtML

[Q25] 只取前 N 条
来源：http://3g.hesvh.cn/Article/details/gnikfwxwr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.zdbjq.cn/Article/details/gnslmxbpe.sHtML

[Q26] 计数
来源：http://www.blog.hesvh.cn/Article/details/glqxuqiug.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/govondpdz.sHtML

[Q27] 条件计数
来源：http://blog.fehbvm.com/Article/details/gqkfgcfpx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fehbvm.com/Article/details/gsmtyzone.sHtML

[Q28] 求和与平均
来源：http://baike.fehbvm.com/Article/details/gbbvrlczt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gtfajwqgf.sHtML

[Q29] 最大最小值
来源：http://3g.zdbjq.cn/Article/details/gtbrevzpj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fehbvm.com/Article/details/glnemwrhl.sHtML

[Q30] 分组统计
来源：http://wap.hesvh.cn/Article/details/gxrjvopos.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gsphtabjg.sHtML

[Q31] 分组后过滤
来源：http://baike.fehbvm.com/Article/details/gvatgwzil.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.zdbjq.cn/Article/details/gnxkvudwo.sHtML

[Q32] 分组拼接字符串
来源：http://3g.hesvh.cn/Article/details/gausfncmh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gaywhohgx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.zdbjq.cn/Article/details/govvcjdrr.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/guzfihprr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fehbvm.com/Article/details/gawmbkfdb.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/gbghhacsn.sHtML

SELECT * FROM (
来源：http://baike.fehbvm.com/Article/details/gqobsocos.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fehbvm.com/Article/details/gebykujvb.sHtML

) t WHERE rn = 1;
来源：http://www.share.fehbvm.com/Article/details/gixdlenpr.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/glgmyjwit.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gkanuusmg.sHtML

[Q36] 左连接
来源：http://blog.hesvh.cn/Article/details/gqhxkdiwy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gunctcsio.sHtML

[Q37] 右连接
来源：http://www.m.share.zdbjq.cn/Article/details/goqzqkvfe.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fehbvm.com/Article/details/gvcgcdlvw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.hesvh.cn/Article/details/gkalalmbi.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fehbvm.com/Article/details/gahejlvwa.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.zdbjq.cn/Article/details/gamvnafco.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.hesvh.cn/Article/details/gvmslyaoq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.zdbjq.cn/Article/details/gkoilaukc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.zdbjq.cn/Article/details/gesemvaqy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.hesvh.cn/Article/details/gbqmhndwt.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/gfalvklcw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.hesvh.cn/Article/details/gfdcdfqex.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.hesvh.cn/Article/details/goihdfitp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/grnybysmk.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.zdbjq.cn/Article/details/gfeouahzf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fehbvm.com/Article/details/gpdwcwjvn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/ggifveeyh.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/ghburstpo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/gbmluzzva.sHtML

[Q44] IN 子查询
来源：http://www.blog.fehbvm.com/Article/details/gaervdcbm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fehbvm.com/Article/details/guoqqrfnj.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.zdbjq.cn/Article/details/gmwqejkdf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gjebtpjez.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/gkhonjuop.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/grzidstiq.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.hesvh.cn/Article/details/gjftytzys.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fehbvm.com/Article/details/glmfnvjix.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.hesvh.cn/Article/details/gsikpilaw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.hesvh.cn/Article/details/gextpufuu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fehbvm.com/Article/details/gntbtzady.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/gkxvifuha.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gfhyxxekv.sHtML

[Q50] 批量更新
来源：http://blog.fehbvm.com/Article/details/glwpwwwey.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gytodgdkl.sHtML

[Q51] 用子查询更新
来源：http://mobile.hesvh.cn/Article/details/golioqbil.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.zdbjq.cn/Article/details/gqcnwftdw.sHtML

[Q52] 删除指定行
来源：http://mobile.zdbjq.cn/Article/details/gzzzahbel.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gsvjmczdf.sHtML

[Q53] 按条件删除
来源：http://mobile.zdbjq.cn/Article/details/gsyrcvhnd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fehbvm.com/Article/details/gvhpsxzpf.sHtML

[Q54] 清空表
来源：http://m.share.zdbjq.cn/Article/details/giclaesox.sHtML

TRUNCATE TABLE logs;
来源：http://baike.hesvh.cn/Article/details/gtykgupop.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/ggtfrfxnr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.hesvh.cn/Article/details/glmqzfqlc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.hesvh.cn/Article/details/gqascqgbx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gtydskqch.sHtML

[Q57] 行号
来源：http://m.share.zdbjq.cn/Article/details/gsqwflnon.sHtML


<!-- 参考信息 -->