代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/guozrfizn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/gypjgujmg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gfrjsdmuf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/ghnvqkywa.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/ghcsltnub.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/gpeqatltu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/gtvhmikrr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/glregyfpw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gicrhjhki.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/ghbdjqugk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/goxyahdsj.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/gbqmhomfk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.hesvh.cn/Article/details/gkgouglqf.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gbxbuksei.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gddmfezhx.sHtML

PHP:  $s === strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gnxwyydqe.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gelbxqwlh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gytbcwqkp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/gnkffnawz.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/giwrikhlg.sHtML

Ruby: s == s.reverse
来源：http://mobile.zdbjq.cn/Article/details/grsclcjbt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gzhbathaz.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.zdbjq.cn/Article/details/gszaasele.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/gjptbcvwf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fehbvm.com/Article/details/gffddwihn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fehbvm.com/Article/details/grebvephz.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.zdbjq.cn/Article/details/grjlfyvjd.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/gztacomly.sHtML

Go:   // 手写 map[int]int
来源：http://blog.zdbjq.cn/Article/details/gpjcjnadn.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/gkxtlxcmb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.hesvh.cn/Article/details/gkeexhima.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/gxvdfvjbf.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.zdbjq.cn/Article/details/geehqrwrp.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.hesvh.cn/Article/details/gzrpgvivh.sHtML

JS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gjkfaocqh.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gjhaviqcj.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gsabnlcwa.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gcjyiphav.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.zdbjq.cn/Article/details/gfmhlvljs.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gkdplxdrd.sHtML

[N09] 栈与队列
来源：http://wap.hesvh.cn/Article/details/goxwwrbzv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/gusighlmc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gwgzzthvb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gvrmoffpb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.zdbjq.cn/Article/details/guwpzzfjd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/gkiwzdzax.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/gusnudbid.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gmgnelice.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fehbvm.com/Article/details/gahhfpckg.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/guvnkbslo.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/gwmfqvofc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fehbvm.com/Article/details/gbgaaembi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.zdbjq.cn/Article/details/gcaxhvlyf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.hesvh.cn/Article/details/gzogyfnwb.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/griswcwvn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.hesvh.cn/Article/details/gzlvqvlyy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.hesvh.cn/Article/details/gqaecbppg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.zdbjq.cn/Article/details/gihasinff.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fehbvm.com/Article/details/grleqdnik.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.hesvh.cn/Article/details/gvexxhljh.sHtML

PHP:  // 手写递归函数
来源：http://blog.hesvh.cn/Article/details/gtixlijhj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gkbnqtomm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gzkdxaqdn.sHtML

Java: // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gjlbqaulf.sHtML

Go:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gnnafqhzl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.zdbjq.cn/Article/details/ghjbmslsb.sHtML

C#:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gsujdrmik.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/gsvuxqyox.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/gemvpkjwx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/gufbnsiwd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gmyirejje.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gvqqrtygg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gaojfarnn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.hesvh.cn/Article/details/gjkjedsld.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/gvwxsphoi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gahonvmki.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gijzzhijj.sHtML

O. 并发与异步
来源：http://read.share.fehbvm.com/Article/details/gfqlkszig.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gewbtecri.sHtML

[O01] 启动一个线程
来源：http://blog.fehbvm.com/Article/details/gislntxav.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/gzhlwazqd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/grtxbjxlw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/gkbyvuozl.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gtuepooqw.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.hesvh.cn/Article/details/gencxfbmk.sHtML

Go:   go f()
来源：http://www.share.fehbvm.com/Article/details/ghiymhqqe.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fehbvm.com/Article/details/gleufhcft.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.hesvh.cn/Article/details/guulhlwdp.sHtML

[O02] 使用线程池
来源：http://3g.fehbvm.com/Article/details/gjirqqvkz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/gsqfecbzj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/gaeuozylj.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gtdqwfzda.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gjazxfsuk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fehbvm.com/Article/details/gjqoktyzi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.zdbjq.cn/Article/details/ggfpkhfop.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.fehbvm.com/Article/details/gmqgphoyg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.zdbjq.cn/Article/details/gapmbkdzs.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/grhhwtlfr.sHtML

Py:   with lock: shared += 1
来源：http://3g.fehbvm.com/Article/details/gqycftwmg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gqpxerpru.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fehbvm.com/Article/details/gyebjfdyu.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/guwgdpebx.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gxazsctaj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.zdbjq.cn/Article/details/gcpjcotjl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.hesvh.cn/Article/details/gulflmdfk.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gtjzgkqtm.sHtML

[O04] 定义异步函数并等待
来源：http://3g.hesvh.cn/Article/details/gcsnjbqys.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fehbvm.com/Article/details/gyctnxtyd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/gwxonppwr.sHtML

JS:   async function f() { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gmaxqrjqi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gzjrzyfot.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/giaeynpaj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/ggptqdles.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/grrtyszyw.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/gxvdqdzsz.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.zdbjq.cn/Article/details/gwehfmskt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gbsmkmdzg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.zdbjq.cn/Article/details/gkbqgdnbw.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gerwkwpqk.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gjpphycjg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.zdbjq.cn/Article/details/gtvbpgngj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fehbvm.com/Article/details/gscothhyk.sHtML

Ruby: threads.map(&:join)
来源：http://blog.hesvh.cn/Article/details/gzqjewuju.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.zdbjq.cn/Article/details/ggximzlqo.sHtML

[O06] 使用进程池
来源：http://blog.fehbvm.com/Article/details/ggvncplai.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.hesvh.cn/Article/details/gogryqhwz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/gkdzyceqt.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gloogvguf.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gsqgyuyyl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.hesvh.cn/Article/details/grqlvgzsm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.hesvh.cn/Article/details/gswowoenn.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/gjjdgdjju.sHtML

C#:   Parallel.For
来源：http://read.share.fehbvm.com/Article/details/gtowfzghg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbeddbrzv.sHtML

P. 常用工具函数
来源：http://www.share.fehbvm.com/Article/details/gtyxzbgxf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grfyanbbu.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/gmkuvopex.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/gfkgzjwdm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.zdbjq.cn/Article/details/gvlggdsfd.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gvabhepuf.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/glcbrafuk.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/gutcbbpjt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fehbvm.com/Article/details/gufplfxjv.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.zdbjq.cn/Article/details/gkndgktsq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.hesvh.cn/Article/details/gplepyxsu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.zdbjq.cn/Article/details/gqcflmfds.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/gjqjtuvlm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/gwmwgzceb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/gvjuzctvf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.zdbjq.cn/Article/details/grfxqcvkl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.hesvh.cn/Article/details/gjrhbkyzv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fehbvm.com/Article/details/gdbunvwje.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gpdweslwx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.zdbjq.cn/Article/details/gldrmgsek.sHtML

[P03] 生成短随机字符串
来源：http://read.share.zdbjq.cn/Article/details/giqbbzawm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/gagolaezs.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.zdbjq.cn/Article/details/gatdcmfud.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gwnqypnsc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gxbrdqynw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.hesvh.cn/Article/details/gavqydbph.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.hesvh.cn/Article/details/gfybpbctq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.hesvh.cn/Article/details/gdryxnurs.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.zdbjq.cn/Article/details/giocgcdrf.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/gnufhsowh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.zdbjq.cn/Article/details/gqarlxmyx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/ghzrswrnn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/goblieoxo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gldcpziyj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.hesvh.cn/Article/details/gbfrtnkll.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.fehbvm.com/Article/details/gahfirtli.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gwnktspnr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.hesvh.cn/Article/details/gcrivdamy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.hesvh.cn/Article/details/gerhxuwdp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fehbvm.com/Article/details/gioxkrbkj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.zdbjq.cn/Article/details/geweqyozr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.hesvh.cn/Article/details/gjcfacgmu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gjqafkjfh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.hesvh.cn/Article/details/ggazbcqpu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/getckybdp.sHtML

Ruby: a == b
来源：http://www.m.share.hesvh.cn/Article/details/ghvrckvlg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/gkrzemkfb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/gquknrucp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.zdbjq.cn/Article/details/gontzrtsx.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fehbvm.com/Article/details/gmygttieb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fehbvm.com/Article/details/gxsoyachj.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/ghsjqqycw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gmfvdoguc.sHtML

Go:   if x == nil {}
来源：http://m.share.zdbjq.cn/Article/details/gjdcsdtct.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fehbvm.com/Article/details/grgnsyosf.sHtML

C#:   if (x is null) {}
来源：http://blog.hesvh.cn/Article/details/gbulwzktz.sHtML

[P07] 防抖与节流
来源：http://blog.hesvh.cn/Article/details/gmzxvenlm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/gseqbeffq.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.zdbjq.cn/Article/details/guggctsto.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gviuophhy.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/ghvsvtkdm.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.hesvh.cn/Article/details/giygxrpzm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.hesvh.cn/Article/details/gwyidiiwi.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.zdbjq.cn/Article/details/gotjukocz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.hesvh.cn/Article/details/ggiiympsn.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fehbvm.com/Article/details/gcfkvronn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.zdbjq.cn/Article/details/gyvbvcbrq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.hesvh.cn/Article/details/ggodoafwf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fehbvm.com/Article/details/gkkmmxdzk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gavmplxpi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/gomnxwaqy.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.zdbjq.cn/Article/details/gccmrkiag.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fehbvm.com/Article/details/grservqux.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.zdbjq.cn/Article/details/gahwtygmw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gimrerkbi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fehbvm.com/Article/details/gmauuocdw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/guaafnrcg.sHtML

[Q01] 创建表
来源：http://www.m.share.hesvh.cn/Article/details/ggrkhkzrl.sHtML

CREATE TABLE users (
来源：http://read.share.fehbvm.com/Article/details/gtlirsigh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gaajicrcl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gqjyftnxe.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fehbvm.com/Article/details/gbxlxunfw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fehbvm.com/Article/details/gtjjhcdrb.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gfjsoigth.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.hesvh.cn/Article/details/gtkkyaerk.sHtML

CREATE TABLE orders (
来源：http://wap.fehbvm.com/Article/details/gffsftsjn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/ggtcjadgq.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gidzalbqy.sHtML

amount DECIMAL(10, 2),
来源：http://baike.hesvh.cn/Article/details/glfspszev.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/gmiqlpqlu.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gwolbfphw.sHtML

[Q03] 增加列
来源：http://wap.fehbvm.com/Article/details/gisrcusuk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fehbvm.com/Article/details/gcmmowors.sHtML

[Q04] 修改列类型
来源：http://www.share.fehbvm.com/Article/details/gjkivrrlj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.zdbjq.cn/Article/details/gazfbxwyk.sHtML

[Q05] 重命名列
来源：http://wap.hesvh.cn/Article/details/gafpiqwls.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/gekupfbjn.sHtML

[Q06] 删除列
来源：http://www.m.share.hesvh.cn/Article/details/gazhqdqfl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.zdbjq.cn/Article/details/gjkmtfchl.sHtML

[Q07] 删除表
来源：http://blog.zdbjq.cn/Article/details/gqakyppey.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.hesvh.cn/Article/details/glprhvxrs.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/gwcciwphn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gmwbnfoei.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/ghtofolqi.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gnxadselq.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/gfrxsqtwn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fehbvm.com/Article/details/gmxyeaput.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/glkxgmiav.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.hesvh.cn/Article/details/gnlnuixot.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/gpioevnno.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fehbvm.com/Article/details/gahqixytd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.hesvh.cn/Article/details/gqrmsrdik.sHtML

[Q13] 忽略重复插入
来源：http://3g.zdbjq.cn/Article/details/gonnqwtrs.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gefjozaan.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.zdbjq.cn/Article/details/gyenadyms.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fehbvm.com/Article/details/gbdlmklru.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/gamqxbmpt.sHtML

[Q15] 查询全部
来源：http://read.share.zdbjq.cn/Article/details/ggcwwtkyo.sHtML

SELECT * FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gwirseroz.sHtML

[Q16] 查询指定列
来源：http://read.share.fehbvm.com/Article/details/gqlzvzmea.sHtML

SELECT id, name FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gfyyjhgmu.sHtML

[Q17] 条件查询
来源：http://www.m.share.hesvh.cn/Article/details/gsweetzfi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/gvafbgigp.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.hesvh.cn/Article/details/gptwwwxeq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fehbvm.com/Article/details/gehevzydd.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/ghpzqufge.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.hesvh.cn/Article/details/gbdrkqmki.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/gejojwkjb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/guesczaqc.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/gijotirmh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fehbvm.com/Article/details/gowomtnmh.sHtML

[Q22] 排序
来源：http://blog.zdbjq.cn/Article/details/gazatbiws.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.hesvh.cn/Article/details/gvmffasvd.sHtML

[Q23] 分页
来源：http://mobile.fehbvm.com/Article/details/gdlmffonu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fehbvm.com/Article/details/gfqlxzxqo.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/gafssmofx.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gnrgelnzt.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/gozywiltz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.hesvh.cn/Article/details/gdjxgrxgx.sHtML

[Q26] 计数
来源：http://3g.hesvh.cn/Article/details/gwaurxhpu.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gemtxrrpm.sHtML

[Q27] 条件计数
来源：http://www.blog.hesvh.cn/Article/details/gbqngjgau.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gleqldohp.sHtML

[Q28] 求和与平均
来源：http://blog.zdbjq.cn/Article/details/grervgdfd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gecrupgyp.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fehbvm.com/Article/details/gangmqzvf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gevtevicu.sHtML

[Q30] 分组统计
来源：http://m.share.zdbjq.cn/Article/details/gtbngafag.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/guqhwwook.sHtML

[Q31] 分组后过滤
来源：http://m.share.fehbvm.com/Article/details/gutzezpgi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.zdbjq.cn/Article/details/glzuyvjub.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fehbvm.com/Article/details/gbmdqogfz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gljeqprnc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/gijjjeiyf.sHtML

[Q33] 多列分组
来源：http://3g.fehbvm.com/Article/details/guqrqokty.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.zdbjq.cn/Article/details/gvdhikiwa.sHtML

[Q34] 每组取第一条
来源：http://baike.fehbvm.com/Article/details/gqaemaptg.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/glqkddcpg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.zdbjq.cn/Article/details/gyjzprjtx.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/guhrbsmys.sHtML

[Q35] 内连接
来源：http://3g.hesvh.cn/Article/details/glbyeonot.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gqmqpzwcg.sHtML

[Q36] 左连接
来源：http://mobile.zdbjq.cn/Article/details/gmbsylomd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gsyexktxy.sHtML

[Q37] 右连接
来源：http://wap.zdbjq.cn/Article/details/gljisrnph.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/gftwnnshq.sHtML


<!-- 参考信息 -->