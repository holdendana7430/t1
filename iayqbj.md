代发 wailian999

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ivggkwre.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3zompvkow.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3muxwfrby.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3tesucyjl.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3pdpnsyqb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3hczdpegh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3lycvmpvo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3lcupuaer.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3ydwcrpat.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3vgarmfhb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3bdazatcu.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3fmaonhcg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ynfbjipx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3osptphbf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3sdrqtxiy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3xonorvmo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3qqplzkgy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3sonkyiir.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3rwaemjsw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mvcajalq.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3uuhbkojz.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ejhaunxa.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3tiopjbsd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqobqumw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3kiaueomz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3vczyjqaa.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3bsybmbxd.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3covmuapi.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3bsdfswgw.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3bvawcuhl.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3xcyuyscs.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3zpdpssue.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pvfbcnpy.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jrncpetd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3citizktz.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3aacpuatv.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ceghurfy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ddgvcdvm.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3ebrcxpnp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3hflshvxj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3mrzkkpbj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3sxijhlun.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3dghabdor.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3itdgsxqk.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3sjyjdccs.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3zkmtbyvr.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3upecfnbj.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3unvohpsi.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3ghpxclnx.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3ibwcktkr.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3smammvdc.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nsoopxnk.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3owpnrgpm.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kbpxrvyz.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3cmhquwjo.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mkskaavr.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3dzpgclaa.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3skfsoqps.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3udhkszsv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3gzfnjmlk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3ffuckkjt.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3cxftqwkz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3kdqymubc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vvpfsdgp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3bjbitcrt.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3aojxqbmw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3sjvkkyio.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3mlizswqp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jtshppwx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3xalnhxen.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3rlzovwtj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3kxqzzqvn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3egbaixud.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3fyvuagqt.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tuuqixbx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3rbpdwcnw.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3zvrehjyv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3haxrspbf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3svdrstsh.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3pkgvyvag.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3tfjdanch.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3kgixxcpb.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3igtredll.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3sycnvibm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3ehibgsrn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3xmvmyfhf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3xjnpnbth.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3rvdrbzml.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3urkwoarq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3ffrlkptn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3wxxszoqm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3pffutrqw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nurgwklf.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3brgacfpx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jvluypyb.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3dfkonzdd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3qgoggrmc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3qypurbuf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3fkfnwnpe.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3pmtvtqge.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3pvhqpbqs.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3svjnbvzx.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3liborrid.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3reoythfh.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3ummwrluv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3riivgwgz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3xoszbrke.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ubodmovi.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3vrbghlmy.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ghkeesam.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3yiulpyci.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3vdwelnoz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3yxhufgxd.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3pomatmbr.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3qnnoeroq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3cmvijolj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3exeanrrx.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3laohrstw.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrjxxxor.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3jyvrrzeg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3crtxyhxo.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwdeemdc.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3jgqxajov.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3baydhhkx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3wbpibdwc.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3asyzutvx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3jwltjdqe.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3iaqufxqg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3edmgzkhi.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3hgrnwypx.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ywnbchio.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3jxevrzix.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3upfiyduh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3mokfdlvf.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3dgdjouhk.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3dvskhtjm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3uzisqeyz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3ezgvniov.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3hnmsrgrb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3hglngjpd.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3hzacczox.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3vgxyqiuq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3azmrckjx.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3euxwjaow.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3wxjslwbo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3negdbpew.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3yffpbsea.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3bzpuavin.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3vwqoebrq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cidrfkxu.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3tpetotis.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lcquloeb.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3rlswoapr.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3istmohmy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3cvkgnijl.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3cdbrajyv.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3fsxtebom.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3boiwnvuo.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3jxmajued.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3tebiyifk.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3mttcrvel.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3kjrvsbef.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3uvhtzczy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3ztpbtmhz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3tmmdextw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3zesqujmc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3yaecowkf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3rakmwram.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3fyoybryw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3fulbubrl.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3bjwoyenm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3woxqoxjb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3larnoqxl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3eskpdses.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3weshgqoz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3lthcyijm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3mafugizl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3jebyjdge.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3gnekfxjr.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3tsvsogdx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3rbgvusdk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3survnkzr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3nocpmmcg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3hotuyaje.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3vchbjhxa.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3djylpgxm.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3beovhfkm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3uwzsrkwa.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3tnjxrwqj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3lotjfkxb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3kauroeiw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3ecpqbwwp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jybsvwti.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3cxadazbj.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3huxpaqnw.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3mtebtlzo.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3mtutownx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3mlckglgu.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3gxtorziw.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3vcabblxc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3jsrxzulv.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3kpslmsca.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iiogbovr.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3ojwtvibg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3rrcyfomk.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3atpwvcgc.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3rzvwpscd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3kabjlkfe.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3nbzrtqqy.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3sjdiyssy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3hmqifeys.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xzovnynu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3wcwwirzg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3fwaxnjzt.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3tkefqbbj.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3fwqnjmqk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3yewnftyq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3btdhnnmo.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3wskbbqmw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3vdajbzzi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3ttjqiczd.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3ltqgdkfl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3laupdvup.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3qyabeask.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ypbrrzxg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3mmopmhpb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3imdaxumo.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3gbkxcssd.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3mndlkset.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3dhicrzsl.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3jymnpbdw.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3zvryrzpn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3knadocgx.html

);
来源：http://www.52xcode.cn/Article/details/gt3gixqpscd.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3oixrqign.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3pcdrsvrt.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3umnsubad.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3cxammott.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3ljkbkejy.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3uxcoqukz.html

);
来源：http://www.52xcode.cn/Article/details/gt3gohewxwn.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3zxzokhxl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3bsltrnbo.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3iwgnqvch.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3iuxcxdhe.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3nwutuctp.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3mviyzaea.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3juxogabv.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3gbjeldox.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3afggrrov.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3lddyrarg.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3aoxqoapk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3szropnhr.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3ifokmkru.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3mpcfybrz.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3otogiekn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3jfkanzok.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3apwdgyjj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3wdeabtfi.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3pdjurbaj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3pvqomrzw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3imyfpnrk.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3bxeylwop.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3lyapvjjv.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3jlwqjdhw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3fdonxgvn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3zrtjojkf.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3jzrpeaby.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mmifcuut.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3jyzcqjmm.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hxalxnrb.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3gogpikpu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ibicsysd.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gjqtsenl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3beeyyqel.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3fhgosmjn.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3hiennwcv.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3csqobijz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3zsdmwfrj.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3qqwzeizp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3oiwdyroo.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3jaffsxyr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3euntdgbk.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3wljazfnc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3yocottos.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3cpfoczua.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xsxhrowz.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3pftfriow.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3xqkbbbch.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3uyyogpmg.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hxyykzbh.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3lbowfmus.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qwnpwoyh.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3vnuwyhaz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pyabvwgd.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3sesldmgk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kuywxoza.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3yqccttws.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3banntdfg.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3khruvmjw.html


<!-- 参考信息 -->