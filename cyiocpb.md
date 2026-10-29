代发 wailian999

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/gbaawvkhy.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/gedyiznla.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.hesvh.cn/Article/details/gqxrvlxtl.sHtML

[N08] 生成全排列
来源：http://read.share.fehbvm.com/Article/details/gldbepwcx.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/gfqlsprrx.sHtML

PHP:  // 手写递归交换
来源：http://mobile.zdbjq.cn/Article/details/gxynxfvwc.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gbuzxjnlb.sHtML

TS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gfaepruxi.sHtML

Java: // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gmwnpnnbu.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/guatoncbm.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.zdbjq.cn/Article/details/gpudjzyqj.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gewjmqfex.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/ggdyxkmuc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.zdbjq.cn/Article/details/goyyhaukv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/glfrcgnnk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gtkvthjya.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/gnmuppnnu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/gdzaikcdm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.hesvh.cn/Article/details/gqjrtxkvw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gloncrqxa.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.zdbjq.cn/Article/details/ggrpqxyww.sHtML

[N10] 链表节点定义
来源：http://baike.fehbvm.com/Article/details/gdgjxynyb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.zdbjq.cn/Article/details/gyixhbemt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/gqsczplmc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fehbvm.com/Article/details/ggdxcjzlu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/gysifjxdb.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/giknvqefd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/gdgfylomz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/gglayedql.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.zdbjq.cn/Article/details/gwtybomze.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/guiqtojzl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.hesvh.cn/Article/details/gasbjebta.sHtML

PHP:  // 手写递归函数
来源：http://3g.hesvh.cn/Article/details/gniejhgyz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gelwzvfsj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gexsnaoaq.sHtML

Java: // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gxgdbwpvb.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/geoqexnmx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/gkwlvrknc.sHtML

C#:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gnibzehlc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fehbvm.com/Article/details/gdvyggoiv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/gnxbkuoex.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fehbvm.com/Article/details/gbbibvzam.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/glnjeffya.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/ggmctboou.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gyeschjeh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/grsuyszmp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/gisptqvli.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gsfrasjrm.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gnxlaewiq.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/glkbnayvs.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gnjonccma.sHtML

[O01] 启动一个线程
来源：http://www.blog.zdbjq.cn/Article/details/gpciqrzbz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/gvxuecpid.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/gluffdjda.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/gdcchihuj.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/ggljaubvo.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gvwvnowgi.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/gdydkcgbh.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gcnyipftt.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/guxymuyjf.sHtML

[O02] 使用线程池
来源：http://baike.fehbvm.com/Article/details/gnylyuqqb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/gzqwlthcs.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/gimgobmxy.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gpwftesjh.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gtatihjao.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/gmaofgtki.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/gzllqtdro.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fehbvm.com/Article/details/goavaggho.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fehbvm.com/Article/details/gsmdicjrk.sHtML

[O03] 加锁保护共享数据
来源：http://3g.hesvh.cn/Article/details/ghrhhbnsw.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/gqljwuhgz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/gygzgrzll.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.hesvh.cn/Article/details/gulikxwnv.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gsrclloib.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gbqzdyjya.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/grhwmewcz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/griwvsovq.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/grimbkayp.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.hesvh.cn/Article/details/gzphjhhqb.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.zdbjq.cn/Article/details/gngwsmrhd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.hesvh.cn/Article/details/gnozeyzzt.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/ghybnfsvv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gcwdroshf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.hesvh.cn/Article/details/gzknmvixm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/gwwkxihhp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/gwsnjhwse.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/gaqzjwkmq.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.hesvh.cn/Article/details/gsdydybzj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/ghtebrcaz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.zdbjq.cn/Article/details/grrwrlkbs.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gjoqezsbw.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gqurrpkou.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/gknjwcsfr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.hesvh.cn/Article/details/gjifljxiz.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gkejdrkli.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fehbvm.com/Article/details/grqemiasy.sHtML

[O06] 使用进程池
来源：http://blog.zdbjq.cn/Article/details/gwpzljccs.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.hesvh.cn/Article/details/grspxqjqc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/gucfumvdx.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/glvsjcagh.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gyltzmcme.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.zdbjq.cn/Article/details/guuxhwewv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/gyoczbsif.sHtML

Ruby: // fork 块
来源：http://3g.hesvh.cn/Article/details/gdtpvhjmm.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/gwoaghtnx.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwmkykkvl.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/gcrvhiqxz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghghkaxrp.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/gyvmsodti.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/gmuvjvcll.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.hesvh.cn/Article/details/gaioqrhmc.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gbgfytogv.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gvfxqagxv.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.hesvh.cn/Article/details/giysorcye.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gshoyzlbl.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/gvkjvetni.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.zdbjq.cn/Article/details/gcxioemdo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.zdbjq.cn/Article/details/gcpyiwfsu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.zdbjq.cn/Article/details/gdvnntcgz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.hesvh.cn/Article/details/gnyqvvadq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.hesvh.cn/Article/details/gluzvqojx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.zdbjq.cn/Article/details/ggamwpiab.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gtphyqurk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fehbvm.com/Article/details/gennvwubu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/ghkotlmfm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/grdqewenh.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gtedhhjno.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.zdbjq.cn/Article/details/guadmznyz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.zdbjq.cn/Article/details/gbfkbcsuc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gbelbbjoa.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/grfwczojf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fehbvm.com/Article/details/ggonrpykg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.hesvh.cn/Article/details/gguybafng.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fehbvm.com/Article/details/gstvgdxcp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.hesvh.cn/Article/details/gdmzhqlfb.sHtML

[P04] 求长度
来源：http://m.share.zdbjq.cn/Article/details/gexdjsayd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.zdbjq.cn/Article/details/gdxbarzdy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gyoigurld.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gtzixdnmc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gxofakdat.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gmoulzpab.sHtML

Go:   len(arr);  len(m)
来源：http://blog.zdbjq.cn/Article/details/glzliwhka.sHtML

Ruby: x.length;  x.size
来源：http://baike.hesvh.cn/Article/details/gkgckprtn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fehbvm.com/Article/details/gzulgslxf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/gsoyhahtt.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.zdbjq.cn/Article/details/gokycjllk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fehbvm.com/Article/details/gaixkelvu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fehbvm.com/Article/details/gizsywwsx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gefmkudep.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.hesvh.cn/Article/details/gapyihlso.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.zdbjq.cn/Article/details/gieiqagql.sHtML

Ruby: a == b
来源：http://m.share.fehbvm.com/Article/details/gfvsbthxy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.hesvh.cn/Article/details/grwqrumpb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fehbvm.com/Article/details/ggwdijtbm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/gabwonosx.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fehbvm.com/Article/details/gcrjbvokw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.zdbjq.cn/Article/details/gjctshqvr.sHtML

TS:   if (x == null) {}
来源：http://wap.zdbjq.cn/Article/details/gdalkmnil.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gcupaxifk.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/gagtmuozm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.hesvh.cn/Article/details/gzsqhekcr.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/gxlugbajs.sHtML

[P07] 防抖与节流
来源：http://www.m.share.hesvh.cn/Article/details/gtdvexabb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.zdbjq.cn/Article/details/gunnavosm.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/gecyrufyy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gqembeory.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/geturlovk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.zdbjq.cn/Article/details/gzitpwtso.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fehbvm.com/Article/details/gehypqjwr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.zdbjq.cn/Article/details/gjxlaxkbr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fehbvm.com/Article/details/gjgueildw.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fehbvm.com/Article/details/gywkivjie.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.zdbjq.cn/Article/details/geghqhsil.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fehbvm.com/Article/details/giatgkqpn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/gevkxqwed.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gzqzdkiqo.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.zdbjq.cn/Article/details/gngphvmfd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fehbvm.com/Article/details/gwvvqbwyc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fehbvm.com/Article/details/gzixmdlry.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.zdbjq.cn/Article/details/gqspcxjcp.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtspzcskt.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fehbvm.com/Article/details/gpaybekty.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzuxbpztc.sHtML

[Q01] 创建表
来源：http://blog.zdbjq.cn/Article/details/gdiagreom.sHtML

CREATE TABLE users (
来源：http://blog.fehbvm.com/Article/details/gckooenmf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/grdceswxm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gempiojrw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fehbvm.com/Article/details/gliljzmpk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.hesvh.cn/Article/details/gaimnoxtj.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gjboauivs.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/guitjxopt.sHtML

CREATE TABLE orders (
来源：http://www.share.fehbvm.com/Article/details/gegauowlc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gchrkdbuy.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gjubnelha.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.zdbjq.cn/Article/details/gvppjlzph.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fehbvm.com/Article/details/gtuweglfx.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gjlgozbvz.sHtML

[Q03] 增加列
来源：http://3g.hesvh.cn/Article/details/gjippibsc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.hesvh.cn/Article/details/glcqwmbhv.sHtML

[Q04] 修改列类型
来源：http://www.m.share.zdbjq.cn/Article/details/gmpfhrvdv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gntasdjmn.sHtML

[Q05] 重命名列
来源：http://mobile.zdbjq.cn/Article/details/grmmiwkbu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/gxkydezqp.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/gblwujhpr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.hesvh.cn/Article/details/gtqamtyyp.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/gsyynshhy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.zdbjq.cn/Article/details/guqyubklw.sHtML

[Q08] 创建普通索引
来源：http://mobile.zdbjq.cn/Article/details/gbixflkdx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gchzfrdkx.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/glzysvjqp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gugiluptm.sHtML

[Q10] 插入单行
来源：http://3g.fehbvm.com/Article/details/gbvlhezsa.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gcxtozrnb.sHtML

[Q11] 一次插入多行
来源：http://baike.hesvh.cn/Article/details/gwpepohfo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gxykxuaye.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fehbvm.com/Article/details/giniaoaac.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fehbvm.com/Article/details/gwnlrygjz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.zdbjq.cn/Article/details/gssggqhzz.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fehbvm.com/Article/details/gpagmfibl.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fehbvm.com/Article/details/gjgdydtwq.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.zdbjq.cn/Article/details/gpbeoftfu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.hesvh.cn/Article/details/gpgioxxij.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.zdbjq.cn/Article/details/gvqwdjsxl.sHtML

[Q15] 查询全部
来源：http://blog.zdbjq.cn/Article/details/gnpidhzgn.sHtML

SELECT * FROM users;
来源：http://3g.hesvh.cn/Article/details/gtwllpjve.sHtML

[Q16] 查询指定列
来源：http://blog.fehbvm.com/Article/details/gwonsckzz.sHtML

SELECT id, name FROM users;
来源：http://www.share.hesvh.cn/Article/details/gsyfmhyzp.sHtML

[Q17] 条件查询
来源：http://read.share.zdbjq.cn/Article/details/gwzlrpnqm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.hesvh.cn/Article/details/gsycavsib.sHtML

[Q18] 模糊匹配
来源：http://read.share.hesvh.cn/Article/details/gzjuardom.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fehbvm.com/Article/details/gjzgbpmbo.sHtML

[Q19] 范围查询
来源：http://read.share.hesvh.cn/Article/details/gfypkmqbd.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.hesvh.cn/Article/details/gwlpesgil.sHtML

[Q20] IN 列表
来源：http://wap.hesvh.cn/Article/details/gvpqdxcqb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fehbvm.com/Article/details/gcedhihlt.sHtML

[Q21] 空值判断
来源：http://www.blog.zdbjq.cn/Article/details/gmtcmnpki.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.hesvh.cn/Article/details/gmzzknxgm.sHtML

[Q22] 排序
来源：http://3g.zdbjq.cn/Article/details/gidklaneb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/gxiuioswo.sHtML

[Q23] 分页
来源：http://wap.fehbvm.com/Article/details/gxjgudnxn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fehbvm.com/Article/details/ggmfgjvvu.sHtML

[Q24] 去重
来源：http://m.share.zdbjq.cn/Article/details/grytjpnds.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.zdbjq.cn/Article/details/gmmcibquc.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.hesvh.cn/Article/details/gjaelzegk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/gryjpzjiy.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/goykezxdg.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fehbvm.com/Article/details/giktgmnuf.sHtML

[Q27] 条件计数
来源：http://m.share.hesvh.cn/Article/details/gbdtlrxcw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gqepcoyce.sHtML

[Q28] 求和与平均
来源：http://blog.zdbjq.cn/Article/details/ggsbjakab.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/geehihgjp.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/grydgiagh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.hesvh.cn/Article/details/gvldxaufk.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/gbmrratsi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gyirigdnb.sHtML

[Q31] 分组后过滤
来源：http://baike.zdbjq.cn/Article/details/gchcwysdw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.zdbjq.cn/Article/details/gncwwgnoc.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gjadwjncp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/geufxbzne.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/gnlcskmer.sHtML

[Q33] 多列分组
来源：http://www.blog.hesvh.cn/Article/details/gykskrnlt.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.hesvh.cn/Article/details/gdowgzrvx.sHtML

[Q34] 每组取第一条
来源：http://wap.hesvh.cn/Article/details/gpnibfltf.sHtML

SELECT * FROM (
来源：http://m.share.fehbvm.com/Article/details/gjjiefpxh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/giotkrzma.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/gnakunisp.sHtML

[Q35] 内连接
来源：http://3g.hesvh.cn/Article/details/gammgxeac.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gvxjtmnru.sHtML

[Q36] 左连接
来源：http://www.blog.hesvh.cn/Article/details/gyxjchzrb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gczddvroo.sHtML

[Q37] 右连接
来源：http://3g.fehbvm.com/Article/details/gwckzkzsj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.hesvh.cn/Article/details/gmbxnhfqu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fehbvm.com/Article/details/gxtotlrym.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fehbvm.com/Article/details/gajgtgbra.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/gnlumrady.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/gakmeqmsq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.hesvh.cn/Article/details/gnovkpjlh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/gngswrifz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.zdbjq.cn/Article/details/gyzbxkbnp.sHtML

[Q41] 多表连接
来源：http://blog.hesvh.cn/Article/details/gydzysdyh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/gfysxfdtn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/gnfvdhgjl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/ghbxaegcn.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.zdbjq.cn/Article/details/gppvvzydz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fehbvm.com/Article/details/gbpjucuzm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/ghxvknsdk.sHtML

[Q43] 标量子查询
来源：http://wap.zdbjq.cn/Article/details/gdhlrnxab.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.zdbjq.cn/Article/details/griwnmgfw.sHtML

[Q44] IN 子查询
来源：http://wap.fehbvm.com/Article/details/gzgeilxrf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fehbvm.com/Article/details/gpwbatadx.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/goggapxut.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gyboiiplc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/gtpwglimx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gfambwluo.sHtML

[Q47] 与平均值比较
来源：http://m.share.zdbjq.cn/Article/details/gjhfofhgh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/ghupvawoo.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fehbvm.com/Article/details/gsdehpyke.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fehbvm.com/Article/details/gpcdsytcu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/goijlmfcj.sHtML

[Q49] 更新单行
来源：http://wap.hesvh.cn/Article/details/grvwbqqbb.sHtML


<!-- 参考信息 -->