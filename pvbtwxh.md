代发 wailian999

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/gkawwzrmo.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/gfxfgpqct.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/gyznssqpv.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/gcpzmfylr.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/gyomqebsu.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/gxwlfsesu.sHtML

JS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gqqomujkx.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/glnbaeaex.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gxcqrbevz.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gizzznvxg.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.hesvh.cn/Article/details/ghqukoubp.sHtML

C#:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gfwxbebup.sHtML

[N09] 栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gqmnwkoka.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/gmpysxndp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/ggepjxheh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/ghyogqbbp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.zdbjq.cn/Article/details/gssuasedf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gqslmoiwe.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/gcrsdorzv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gjmrzybnv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/ghfnvmbhd.sHtML

[N10] 链表节点定义
来源：http://www.blog.zdbjq.cn/Article/details/gcacuskgn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fehbvm.com/Article/details/gceyxoukl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.fehbvm.com/Article/details/gbvubgnwz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gwhakxdov.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/gikbodkoj.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/gwojuiknr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.zdbjq.cn/Article/details/gqqamyuxp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.hesvh.cn/Article/details/gjemsztuc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/gjqshsjqo.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/gyavwxqpc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/gqwnzfcqg.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.zdbjq.cn/Article/details/gwbyrgrzd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gomfapkzs.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gersantww.sHtML

Java: // 手写递归
来源：http://baike.hesvh.cn/Article/details/gaftdslcb.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gyhziwmig.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gbkdlvbby.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gsjjznfrs.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fehbvm.com/Article/details/gcehwxtkt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/gelhmeltm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gumenyixr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gitmasloa.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gibikzzly.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gwmoqgbgd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/gtzqnvlnu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/gjwnufqjs.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gevmuzhdp.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvwswketx.sHtML

O. 并发与异步
来源：http://blog.fehbvm.com/Article/details/gdfsjsxpe.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxbinxsgl.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/gwhlwkiqx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.zdbjq.cn/Article/details/gxlxrrrsr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/gxyngyvri.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.hesvh.cn/Article/details/gditappxl.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gfanrbgth.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fehbvm.com/Article/details/gcpghztbr.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/gekvsokqh.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fehbvm.com/Article/details/gezclivel.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fehbvm.com/Article/details/grawmjgyu.sHtML

[O02] 使用线程池
来源：http://www.m.share.zdbjq.cn/Article/details/ggcppqcum.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.zdbjq.cn/Article/details/gczgfjcao.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/gdrilslci.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/guoonfjtv.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/glfbbytcz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/gdanoyqgs.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fehbvm.com/Article/details/gmmvwaxze.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/gyaecpusg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gnzvsrylc.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fehbvm.com/Article/details/glpokglno.sHtML

Py:   with lock: shared += 1
来源：http://m.share.zdbjq.cn/Article/details/gfgzewsdu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fehbvm.com/Article/details/gngyfeznf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.hesvh.cn/Article/details/gfoyfwwrs.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gmvckmbtb.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gchuxospu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/gzpiipjch.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fehbvm.com/Article/details/gxdfguxfg.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/guwmyzgwk.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gomvkpxmq.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.hesvh.cn/Article/details/gseynjyuc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fehbvm.com/Article/details/gujoxbihv.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/gqimpjizq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gnnthlxod.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.zdbjq.cn/Article/details/gcpbtfsed.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/goxaowuuv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.zdbjq.cn/Article/details/gjxxtapnr.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fehbvm.com/Article/details/ggmhbofap.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/gujrfxtox.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.zdbjq.cn/Article/details/gobetmlxc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.zdbjq.cn/Article/details/ggmvtkarx.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gpiabtuau.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gzgsvvxpx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.zdbjq.cn/Article/details/gcfcptrov.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/gplfzzlsr.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gxzzskvhr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fehbvm.com/Article/details/glchgsxjm.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/glzkitfza.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.zdbjq.cn/Article/details/gnjmmlrlx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.fehbvm.com/Article/details/gmvqnrmoc.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gbjseiorl.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gbnjxcdzm.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.hesvh.cn/Article/details/gfecxihig.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.zdbjq.cn/Article/details/gbisykbdj.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/gnoosbkse.sHtML

C#:   Parallel.For
来源：http://baike.hesvh.cn/Article/details/gjnjusysi.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghdjvkxzp.sHtML

P. 常用工具函数
来源：http://www.share.zdbjq.cn/Article/details/gldfvshqs.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwypyqxqr.sHtML

[P01] 生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gzqgyrrjb.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fehbvm.com/Article/details/gpeslwskg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fehbvm.com/Article/details/grhqbhcgu.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gxofudpui.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gmxdhstsx.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/glmcjzcgl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fehbvm.com/Article/details/gfrqfvdnq.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fehbvm.com/Article/details/gnvoukejl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fehbvm.com/Article/details/gtiuzcqyf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.hesvh.cn/Article/details/glehnrgsx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.hesvh.cn/Article/details/gtqxpulpk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fehbvm.com/Article/details/gqpbceylj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.hesvh.cn/Article/details/gyuijlrwy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.hesvh.cn/Article/details/gxduskrxy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gyakbkinh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/ganwuyzjm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fehbvm.com/Article/details/gmdvgkcsx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.hesvh.cn/Article/details/gwolyghdj.sHtML

[P03] 生成短随机字符串
来源：http://3g.hesvh.cn/Article/details/gblwfmlfa.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.hesvh.cn/Article/details/grecbfaub.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.hesvh.cn/Article/details/gyhegycgd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gaiuwvtll.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/ggbcsdhxn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.hesvh.cn/Article/details/gwwcjqglz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fehbvm.com/Article/details/gdowhmoyk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.zdbjq.cn/Article/details/gzmgzngkt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.hesvh.cn/Article/details/gdlrzcgvz.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/grejdyaff.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.zdbjq.cn/Article/details/gwqmiarlf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/glhudruck.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/goazazcfl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gocrbgxha.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fehbvm.com/Article/details/gzdphkjsa.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fehbvm.com/Article/details/gtuoxidew.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fehbvm.com/Article/details/gswtfmalq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.zdbjq.cn/Article/details/glicfxihi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.fehbvm.com/Article/details/gqzhzeafb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/gtvkxwchh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.zdbjq.cn/Article/details/gvjglvjfj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fehbvm.com/Article/details/gfcfkyixn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gpkrmcqmd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.hesvh.cn/Article/details/gjguvtvun.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fehbvm.com/Article/details/gjabbahla.sHtML

Ruby: a == b
来源：http://www.blog.fehbvm.com/Article/details/gxqsbckbo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fehbvm.com/Article/details/ghdyrsojr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fehbvm.com/Article/details/gbmiftgjy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.zdbjq.cn/Article/details/gmbjjtqmg.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.hesvh.cn/Article/details/ggbzrlcgb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.zdbjq.cn/Article/details/gmmsmwqxw.sHtML

TS:   if (x == null) {}
来源：http://wap.hesvh.cn/Article/details/gynfnwenj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gawxsqmzf.sHtML

Go:   if x == nil {}
来源：http://baike.hesvh.cn/Article/details/ghimqdrlc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.zdbjq.cn/Article/details/gavembjyl.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gpujvarvf.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/grmnznkzs.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/gmzkzbyhh.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.hesvh.cn/Article/details/ghneybkxb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gknoadcwd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gjvlcifeg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.hesvh.cn/Article/details/grlfzyrdo.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.zdbjq.cn/Article/details/gifkyqnfh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.zdbjq.cn/Article/details/gnokarrhb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fehbvm.com/Article/details/gkkcnpowg.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/gurwywdtp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/gipvjimts.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fehbvm.com/Article/details/gddhbdwpk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fehbvm.com/Article/details/gotfikkya.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gxhoxixpv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.hesvh.cn/Article/details/gjhncgrwp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.hesvh.cn/Article/details/gajxndlxa.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fehbvm.com/Article/details/gxmohvrmg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.hesvh.cn/Article/details/gmmqwnzim.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvsmqmluz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.zdbjq.cn/Article/details/givzxpqcy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gejjyyeih.sHtML

[Q01] 创建表
来源：http://baike.fehbvm.com/Article/details/gaawoyysn.sHtML

CREATE TABLE users (
来源：http://wap.zdbjq.cn/Article/details/gtdhdtoiy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gumuyimnz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gekdwfdpq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/gsmyafzle.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/geuhygncq.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gmutxfsih.sHtML

[Q02] 创建带外键的表
来源：http://blog.hesvh.cn/Article/details/gggsmyzpq.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/gznixhhqb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gdytfjyxd.sHtML

user_id INT NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gttsbjcif.sHtML

amount DECIMAL(10, 2),
来源：http://blog.zdbjq.cn/Article/details/grfwtirzj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.hesvh.cn/Article/details/gebjklaoc.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/glwssrxpp.sHtML

[Q03] 增加列
来源：http://m.share.zdbjq.cn/Article/details/ggzsiixyj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.hesvh.cn/Article/details/ggpdteivl.sHtML

[Q04] 修改列类型
来源：http://www.share.fehbvm.com/Article/details/ggpdbcffv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.zdbjq.cn/Article/details/gyovzihag.sHtML

[Q05] 重命名列
来源：http://www.blog.hesvh.cn/Article/details/grapxjtyl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.zdbjq.cn/Article/details/ggzcppwft.sHtML

[Q06] 删除列
来源：http://read.share.hesvh.cn/Article/details/gujiebbyx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/ghoocwhqg.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/grctellso.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fehbvm.com/Article/details/gjobpstid.sHtML

[Q08] 创建普通索引
来源：http://3g.hesvh.cn/Article/details/gpwgmxygz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gtkpyeyso.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.hesvh.cn/Article/details/gbhwvkesu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gffijthzy.sHtML

[Q10] 插入单行
来源：http://read.share.hesvh.cn/Article/details/gluzejlpk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.zdbjq.cn/Article/details/gjsfusslk.sHtML

[Q11] 一次插入多行
来源：http://read.share.fehbvm.com/Article/details/gkolnorst.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/gextqjryx.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.hesvh.cn/Article/details/gojyhoxtz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fehbvm.com/Article/details/gyfholfhr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/gvvnrgyao.sHtML

[Q13] 忽略重复插入
来源：http://wap.zdbjq.cn/Article/details/gzmkxpskk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/gnyxxsznl.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.zdbjq.cn/Article/details/gozcblwlt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.hesvh.cn/Article/details/ghzxoqoln.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fehbvm.com/Article/details/geotrghdx.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/gbmmfmnnh.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/ggqjcrerh.sHtML

[Q16] 查询指定列
来源：http://3g.fehbvm.com/Article/details/gxbmhfesz.sHtML

SELECT id, name FROM users;
来源：http://read.share.zdbjq.cn/Article/details/grkkaqqsl.sHtML

[Q17] 条件查询
来源：http://wap.fehbvm.com/Article/details/gngisoois.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fehbvm.com/Article/details/gxucqecla.sHtML

[Q18] 模糊匹配
来源：http://3g.hesvh.cn/Article/details/grzxcxooe.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fehbvm.com/Article/details/gnpzitxjl.sHtML

[Q19] 范围查询
来源：http://baike.fehbvm.com/Article/details/glqglafwu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.zdbjq.cn/Article/details/gwzfoenmb.sHtML

[Q20] IN 列表
来源：http://baike.hesvh.cn/Article/details/gdizrgvvv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/gzlwwbppn.sHtML

[Q21] 空值判断
来源：http://blog.fehbvm.com/Article/details/goklvxqtc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gpyoadcxm.sHtML

[Q22] 排序
来源：http://blog.hesvh.cn/Article/details/gzpkmxxuf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gqoghmwpm.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/goselduor.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.hesvh.cn/Article/details/gmwwlewvb.sHtML

[Q24] 去重
来源：http://mobile.hesvh.cn/Article/details/gjmiaytka.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/goowmjvmq.sHtML

[Q25] 只取前 N 条
来源：http://blog.hesvh.cn/Article/details/gaovqiowg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.zdbjq.cn/Article/details/gomvqpwty.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/gcnbacnop.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gdesyfuwp.sHtML

[Q27] 条件计数
来源：http://blog.zdbjq.cn/Article/details/goyzsxzyy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fehbvm.com/Article/details/guvgebnlb.sHtML

[Q28] 求和与平均
来源：http://www.blog.hesvh.cn/Article/details/gucebywfm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gyogoeput.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/goasrbjwp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.hesvh.cn/Article/details/gybfzmzng.sHtML

[Q30] 分组统计
来源：http://baike.hesvh.cn/Article/details/gjtheolts.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gxwqzkulm.sHtML

[Q31] 分组后过滤
来源：http://mobile.hesvh.cn/Article/details/gucveaypp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gkkrcqmvj.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gclqpkudi.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/ghpzcoloi.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fehbvm.com/Article/details/gteiwbltx.sHtML

[Q33] 多列分组
来源：http://m.share.fehbvm.com/Article/details/gqllpdsqu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.hesvh.cn/Article/details/gixuirxng.sHtML

[Q34] 每组取第一条
来源：http://m.share.hesvh.cn/Article/details/gnwqkinzi.sHtML

SELECT * FROM (
来源：http://m.share.zdbjq.cn/Article/details/guzlmwung.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/gbjxmuxij.sHtML

) t WHERE rn = 1;
来源：http://wap.zdbjq.cn/Article/details/gjdedgpws.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/gxhjialea.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gwdkdebiz.sHtML

[Q36] 左连接
来源：http://www.m.share.hesvh.cn/Article/details/gxtmhwokd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gbnalkawt.sHtML

[Q37] 右连接
来源：http://blog.hesvh.cn/Article/details/grlfcdwtp.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.zdbjq.cn/Article/details/gpnstjgeo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fehbvm.com/Article/details/gnhxvzyns.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.hesvh.cn/Article/details/gnhkrvvlz.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.hesvh.cn/Article/details/gdvkrljux.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.hesvh.cn/Article/details/gbodpadox.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/gdseznhzw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fehbvm.com/Article/details/geoqbbcdd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fehbvm.com/Article/details/gcwarlzxr.sHtML

[Q41] 多表连接
来源：http://m.share.hesvh.cn/Article/details/gudehnzui.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fehbvm.com/Article/details/gozhoguav.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.hesvh.cn/Article/details/ghlqutgek.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.hesvh.cn/Article/details/gnifhuadd.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.zdbjq.cn/Article/details/gjfstydga.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.zdbjq.cn/Article/details/gmywmtpro.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.hesvh.cn/Article/details/gsxilhqfj.sHtML

[Q43] 标量子查询
来源：http://mobile.zdbjq.cn/Article/details/gxdgqkmlj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gueuktbwf.sHtML

[Q44] IN 子查询
来源：http://www.blog.fehbvm.com/Article/details/gcjyqexpb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/giktrdika.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.hesvh.cn/Article/details/garuvdlzb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gqutyiomp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.zdbjq.cn/Article/details/gdhvnqceq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gewjkrubf.sHtML

[Q47] 与平均值比较
来源：http://www.share.hesvh.cn/Article/details/gyaqdioeu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.zdbjq.cn/Article/details/giefixjzx.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.hesvh.cn/Article/details/ggojhitzi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.hesvh.cn/Article/details/gaaftikep.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.zdbjq.cn/Article/details/gsivnwshd.sHtML

[Q49] 更新单行
来源：http://mobile.zdbjq.cn/Article/details/gdixkoxpk.sHtML


<!-- 参考信息 -->