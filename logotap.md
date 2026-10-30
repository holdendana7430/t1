代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfatsdzfk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpmebhfx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fanxiaobao.xyz/Article/details/gshpdvwds.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfxvnnhf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.fanxiaobao.xyz/Article/details/gpsykbvmj.sHtML

[N10] 链表节点定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmtwgxfh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fanxiaobao.xyz/Article/details/gpsayngtc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqolvilwt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gluszussp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gktqqpqak.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghznrquzo.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fanxiaobao.xyz/Article/details/gekydeevq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fanxiaobao.xyz/Article/details/gtzjjcvit.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fanxiaobao.xyz/Article/details/ggmlmfrzt.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fanxiaobao.xyz/Article/details/grgqorkbc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbuvpbwr.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfxfpnbo.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fanxiaobao.xyz/Article/details/gfubcyrua.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fanxiaobao.xyz/Article/details/gucnaqooo.sHtML

Java: // 手写递归
来源：http://3g.fanxiaobao.xyz/Article/details/gfmlzqxby.sHtML

Go:   // 手写递归
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzhtyirn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fanxiaobao.xyz/Article/details/gthzniwat.sHtML

C#:   // 手写递归
来源：http://3g.fanxiaobao.xyz/Article/details/gpdjkxobk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqhojoue.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxknumcn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjixtrtf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fanxiaobao.xyz/Article/details/godqquxyy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyoducvog.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fanxiaobao.xyz/Article/details/ghyvnovyu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxxyrbft.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gllicgvdj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fanxiaobao.xyz/Article/details/goicpnqef.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxyfqcew.sHtML

O. 并发与异步
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfaswopus.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/grxzkeeln.sHtML

[O01] 启动一个线程
来源：http://read.share.fanxiaobao.xyz/Article/details/grdiaejlp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fanxiaobao.xyz/Article/details/gsfrstsvs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gtobsopsh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fanxiaobao.xyz/Article/details/gqkyncmhs.sHtML

TS:   // 同 JS
来源：http://blog.fanxiaobao.xyz/Article/details/gkrhskaay.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fanxiaobao.xyz/Article/details/gjtsuikfs.sHtML

Go:   go f()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtprhbztp.sHtML

Ruby: Thread.new { f }
来源：http://3g.fanxiaobao.xyz/Article/details/gajytxwuw.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjwxliuo.sHtML

[O02] 使用线程池
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdpulwpn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfywqozs.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fanxiaobao.xyz/Article/details/gifyewxhc.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmlkqcsn.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnofnpzl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwikhmrnc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fanxiaobao.xyz/Article/details/gqccibibp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjovhvyq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpaoibymn.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcculnqzw.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjcyphrh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehtsegdu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxlimmez.sHtML

TS:   // 同 JS
来源：http://wap.fanxiaobao.xyz/Article/details/gktxdluqp.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fanxiaobao.xyz/Article/details/gocasxvyw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fanxiaobao.xyz/Article/details/ghddqiccb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/glekfikbs.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkrpqudmk.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygcrfokp.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fanxiaobao.xyz/Article/details/gvidvskus.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fanxiaobao.xyz/Article/details/gmvfpriiz.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fanxiaobao.xyz/Article/details/glyiqykvp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geogjndat.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fanxiaobao.xyz/Article/details/giqeuscvl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fanxiaobao.xyz/Article/details/gbiegtqoh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfejhfup.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gmeokeghv.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fanxiaobao.xyz/Article/details/gxmvuhipk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fanxiaobao.xyz/Article/details/gyuqhzsuy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fanxiaobao.xyz/Article/details/gneubsfqj.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsalgeais.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fanxiaobao.xyz/Article/details/gotaxrzjb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fanxiaobao.xyz/Article/details/ghutyjxna.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fanxiaobao.xyz/Article/details/gewmylsum.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfihqylyg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvejutfp.sHtML

[O06] 使用进程池
来源：http://m.share.fanxiaobao.xyz/Article/details/giangqsfn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fanxiaobao.xyz/Article/details/gcskzdytg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fanxiaobao.xyz/Article/details/guhskwpso.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfdsonfj.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.fanxiaobao.xyz/Article/details/gncjafwku.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fanxiaobao.xyz/Article/details/gtylfrmbi.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrsdxgfo.sHtML

Ruby: // fork 块
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqkkhuwp.sHtML

C#:   Parallel.For
来源：http://3g.fanxiaobao.xyz/Article/details/gknovaphb.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsbfxzqz.sHtML

P. 常用工具函数
来源：http://baike.fanxiaobao.xyz/Article/details/gljrlierm.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ghaiobnti.sHtML

[P01] 生成 UUID
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyjpoeco.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fanxiaobao.xyz/Article/details/gerlogpxp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugalwtvs.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fanxiaobao.xyz/Article/details/gkkfagory.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fanxiaobao.xyz/Article/details/gieryzhmv.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fanxiaobao.xyz/Article/details/gmrekpopl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fanxiaobao.xyz/Article/details/gwneecrbi.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrcypouj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxfboyxu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fanxiaobao.xyz/Article/details/gqndrzvit.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fanxiaobao.xyz/Article/details/gtmeqqswn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gasvgmcsq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnmkcsyf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fanxiaobao.xyz/Article/details/gvxxhjfmr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fanxiaobao.xyz/Article/details/gafqtpdsw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghscvpro.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gesheyzvl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fanxiaobao.xyz/Article/details/gyewpwtsp.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuiivjte.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzyfeyls.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fanxiaobao.xyz/Article/details/geeznpykc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojfgpmvw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fanxiaobao.xyz/Article/details/gjltnwthc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwuqqlkd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fanxiaobao.xyz/Article/details/gokqltgnq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fanxiaobao.xyz/Article/details/grialggxp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fanxiaobao.xyz/Article/details/gjdqurtrn.sHtML

[P04] 求长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkztojdy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fanxiaobao.xyz/Article/details/gmurmeypz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fanxiaobao.xyz/Article/details/glrdsqwzg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fanxiaobao.xyz/Article/details/gijdommch.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fanxiaobao.xyz/Article/details/gveemvfjs.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fanxiaobao.xyz/Article/details/gqiuwpijo.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fanxiaobao.xyz/Article/details/gswvwojqn.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fanxiaobao.xyz/Article/details/gdcpyvhfj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmizguniz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fanxiaobao.xyz/Article/details/gueibdbiu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqaipbfm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fanxiaobao.xyz/Article/details/gkfjaagxd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fanxiaobao.xyz/Article/details/gqazseafb.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fanxiaobao.xyz/Article/details/gpvqwsaob.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpdkugcx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.fanxiaobao.xyz/Article/details/gfsphbzmf.sHtML

Ruby: a == b
来源：http://3g.fanxiaobao.xyz/Article/details/giansrjdy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fanxiaobao.xyz/Article/details/gmodhbwtg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gajowczfe.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fanxiaobao.xyz/Article/details/gacvbnift.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaefmuugr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fanxiaobao.xyz/Article/details/ganxdcvub.sHtML

TS:   if (x == null) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgychwvc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gyonzeqyq.sHtML

Go:   if x == nil {}
来源：http://blog.fanxiaobao.xyz/Article/details/gkarwjlqj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fanxiaobao.xyz/Article/details/gugpxlfwg.sHtML

C#:   if (x is null) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/groeutmwu.sHtML

[P07] 防抖与节流
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpyvzews.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fanxiaobao.xyz/Article/details/gmaaafeff.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxxhrdwj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyteqafg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gijnwckul.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gglxjimfv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fanxiaobao.xyz/Article/details/gasvcwcen.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzhuqhdp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fanxiaobao.xyz/Article/details/grfrqymqf.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwelkkxhy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fanxiaobao.xyz/Article/details/glbotachv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvzbison.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fanxiaobao.xyz/Article/details/gtadsisfi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrxcykkm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fanxiaobao.xyz/Article/details/gvyfakwgn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fanxiaobao.xyz/Article/details/gppzdfzvf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fanxiaobao.xyz/Article/details/gsttmizvo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fanxiaobao.xyz/Article/details/gtzqnxlnv.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujfxowld.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyocpexam.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gfozxefur.sHtML

[Q01] 创建表
来源：http://mobile.fanxiaobao.xyz/Article/details/gexdoaeai.sHtML

CREATE TABLE users (
来源：http://baike.fanxiaobao.xyz/Article/details/gizsqaeaf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fanxiaobao.xyz/Article/details/gjaehirys.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fanxiaobao.xyz/Article/details/gsojgjkxc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fanxiaobao.xyz/Article/details/guahamuvu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fanxiaobao.xyz/Article/details/goyxhriel.sHtML

);
来源：http://baike.fanxiaobao.xyz/Article/details/gdwhgwtfc.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fanxiaobao.xyz/Article/details/gyaxmpgod.sHtML

CREATE TABLE orders (
来源：http://3g.fanxiaobao.xyz/Article/details/gisqqesgf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fanxiaobao.xyz/Article/details/gapwkipdu.sHtML

user_id INT NOT NULL,
来源：http://mobile.fanxiaobao.xyz/Article/details/gzuxhnhbm.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fanxiaobao.xyz/Article/details/ghdekrslq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhzoanno.sHtML

);
来源：http://3g.fanxiaobao.xyz/Article/details/gdgckcmef.sHtML

[Q03] 增加列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkuyzzwrn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fanxiaobao.xyz/Article/details/geutdxedk.sHtML

[Q04] 修改列类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdonrutm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwyrmskbe.sHtML

[Q05] 重命名列
来源：http://blog.fanxiaobao.xyz/Article/details/ghbhqyziw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdogxsvek.sHtML

[Q06] 删除列
来源：http://3g.fanxiaobao.xyz/Article/details/gdjkxpxky.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqjqhpmt.sHtML

[Q07] 删除表
来源：http://3g.fanxiaobao.xyz/Article/details/gnocwsvlg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gkrraegcs.sHtML

[Q08] 创建普通索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzuarxnb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdybtaym.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdldxjzc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fanxiaobao.xyz/Article/details/gbwunkogw.sHtML

[Q10] 插入单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdheyyafh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fanxiaobao.xyz/Article/details/gbcskbfri.sHtML

[Q11] 一次插入多行
来源：http://baike.fanxiaobao.xyz/Article/details/gcojpjnip.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmlfkduk.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fanxiaobao.xyz/Article/details/gpnauorvw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwxjbhva.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqfkfpap.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fanxiaobao.xyz/Article/details/greaqbufv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvqkwcpd.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fanxiaobao.xyz/Article/details/guaehnfwf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmtrrdha.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkghkkkbv.sHtML

[Q15] 查询全部
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdhuavia.sHtML

SELECT * FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtwovask.sHtML

[Q16] 查询指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/geitnluif.sHtML

SELECT id, name FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmwbecps.sHtML

[Q17] 条件查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gdimxnvei.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhtcutwo.sHtML

[Q18] 模糊匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/geaivsmle.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhdpoiwd.sHtML

[Q19] 范围查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzkmadzp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fanxiaobao.xyz/Article/details/gwkevbfvr.sHtML

[Q20] IN 列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbfqalbd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/graksxmyl.sHtML

[Q21] 空值判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gswpznalo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fanxiaobao.xyz/Article/details/gavpqlrdw.sHtML

[Q22] 排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojnlmnih.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyopckzmv.sHtML

[Q23] 分页
来源：http://read.share.fanxiaobao.xyz/Article/details/gvieifjjy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girgclpoy.sHtML

[Q24] 去重
来源：http://www.share.fanxiaobao.xyz/Article/details/gauuorvch.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gjtcjzvuz.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gclfujmbo.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fanxiaobao.xyz/Article/details/gtyjdrteh.sHtML

[Q26] 计数
来源：http://wap.fanxiaobao.xyz/Article/details/gkvgxozbw.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gazmpxgwx.sHtML

[Q27] 条件计数
来源：http://baike.fanxiaobao.xyz/Article/details/gtyiyiwsn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gjxbmhdbe.sHtML

[Q28] 求和与平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkwixpqu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gpcvzahac.sHtML

[Q29] 最大最小值
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmgwgvdd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdheublmt.sHtML

[Q30] 分组统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfrvngho.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gptiuuqsj.sHtML

[Q31] 分组后过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gweajtgzp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzerzzvr.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gteygbmbm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gvmtolfbo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gineesxcx.sHtML

[Q33] 多列分组
来源：http://blog.fanxiaobao.xyz/Article/details/gzngtqptf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjladqao.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuliadqk.sHtML

SELECT * FROM (
来源：http://baike.fanxiaobao.xyz/Article/details/gvxtjigpc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fanxiaobao.xyz/Article/details/gjzpvdzct.sHtML

) t WHERE rn = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gabwbcsdm.sHtML

[Q35] 内连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbegvhjv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gxoevgynl.sHtML

[Q36] 左连接
来源：http://read.share.fanxiaobao.xyz/Article/details/geuuceifl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghebddpis.sHtML

[Q37] 右连接
来源：http://3g.fanxiaobao.xyz/Article/details/gzmkiinlc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugmfvklt.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fanxiaobao.xyz/Article/details/gszezhjpw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzivaikj.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fanxiaobao.xyz/Article/details/glwayunkv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fanxiaobao.xyz/Article/details/gnppfvmrt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gqcizxwkt.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geftdnoku.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqbtiydf.sHtML

[Q41] 多表连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gagbgakps.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fanxiaobao.xyz/Article/details/ggjdpmpzk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fanxiaobao.xyz/Article/details/gepzwxyyr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gbgzanqmx.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrymdrgz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsaiurgs.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrcdcyqp.sHtML

[Q43] 标量子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvyzlpjc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fanxiaobao.xyz/Article/details/gfbcwlioh.sHtML

[Q44] IN 子查询
来源：http://baike.fanxiaobao.xyz/Article/details/gynsgvkdz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdramehbu.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gallxofrk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchhoxlza.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxkqryjg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjczcqvus.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhnysyqw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzovtintd.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fanxiaobao.xyz/Article/details/ghpzeicbw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fanxiaobao.xyz/Article/details/gfokgqdcw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gpephjiih.sHtML

[Q49] 更新单行
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxuzwuge.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gmcvaqjjt.sHtML

[Q50] 批量更新
来源：http://wap.fanxiaobao.xyz/Article/details/gqjghusaj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxteemebd.sHtML

[Q51] 用子查询更新
来源：http://3g.fanxiaobao.xyz/Article/details/gtvfsuhlu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrabjytd.sHtML

[Q52] 删除指定行
来源：http://m.share.fanxiaobao.xyz/Article/details/gojjngvij.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/guzfdkpeq.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggthdvlrs.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gbuwrqsnk.sHtML

[Q54] 清空表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptgztsfe.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbizwcpf.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gffmbpjin.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghunfhuic.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganldjomt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrhjubei.sHtML

[Q57] 行号
来源：http://baike.fanxiaobao.xyz/Article/details/gphcaetxp.sHtML


<!-- 参考信息 -->