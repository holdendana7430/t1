代发 wailian999

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2omnrorun.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2hsusksuv.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2yaxdfmoi.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2fpsmusvk.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2whrpyojn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2qxrtgzmm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2qtbtmftp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2xovcwcig.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2mvenmqrk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2wdyupvrh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2xutggcik.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2tuwrqfar.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tjwyljoy.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2bzefifxv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tgylpjsf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ehavavej.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2eftnypfx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2rfkxpfbo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ggrwlhur.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2rvtrsywo.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2utdwkmdy.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ulzhbixn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2ocdnrchy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2jxjbmfcr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2gdolcsij.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2dprkzhbq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2argciqzp.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xmarlgyd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2diwcwqox.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2fpyefaaw.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2eqmhrgua.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bmmmgzet.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rypytvkk.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2koxiegwj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2jwzfqkyw.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2vfbodhzn.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2clsnaeyt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2bjepngoc.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2hyqqylhv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2mgpructk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2plfjxjsz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2pvlblwzb.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2kvnmjcul.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2hwjdpmgt.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2pmtkhfmp.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2uqsdzwds.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2hyveggze.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2kchxakfd.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qmpxmfgw.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2npmzyxqa.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2yhjpgoic.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nxyllqtw.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ddlyhwky.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ehcpyryg.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2nkngswak.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2oszzdnuf.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2sqzofezb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2htasrnmz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2tlhfjsdf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rjfnyaya.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2knoqkmlx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ntjtcfnx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2jdadqhew.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2eemyxldj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2rjldgrsy.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2hqjbdwjy.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2bcizcfuh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2nkdglqzr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2lqebqhje.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2nhndhmas.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2ctmmogxk.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2qcuufhtz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2hdklvsuk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofmzinry.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2wwlbcmuh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ekakkxzq.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2hecryzzo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2pkfhbafm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2bjknrufv.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ndjhpfwp.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2vtyeipst.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2abmaluba.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2rduiceix.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2bsmnllro.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2hnrgudxw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2vltqumyq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2jsnzqdjs.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2anhzzgtr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2yxmubgyg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2fdryngdf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2npzocsjv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2oyhqpvdf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2plgauijv.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2kuenqqom.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dsdedxlk.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2gpugtydg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2lsiponfc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2mxvihwlw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2vcgxujkg.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2mrlbucbu.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2bplphazh.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2azipstuo.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2hdvaheci.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2euuuqogx.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mkgeivcf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2jhmwfdgo.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2ymiapmed.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2nocbzvvd.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2kmuawigs.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ifzsesvk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2svyyrtrw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2fixvzkwi.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2hyuwwhrj.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2cevzpczk.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2vxzmrttf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2jrocomsp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2kngveeyn.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2xsqethvb.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jgkbruyf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2ctqaoulu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2idlbwrci.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2kslayrmn.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2gfjgceag.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2adnipbbl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2czejvomp.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2bdxzjewa.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xtdredke.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2mtxitalc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2lvsafdfp.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2haxkbyyu.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2irpyvpdh.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2hkopdzft.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2zujifaeo.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2mrrwayft.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2sncfusnx.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2cvwildib.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2llzwxgkl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2qtxwnqgq.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2zmwxbbdw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2nyqysaff.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2rzhiilmc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2adswduei.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2vsmanxzr.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2knfelbmg.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2tmkotcgg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2ffwsusls.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2qyzhvwjc.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2nzuzjnwk.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2ulkbstcx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eysrrzyo.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2bfslqkyw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wmrllttz.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2splflasr.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2ladkwkir.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2nfrmvbsa.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2snsrhaft.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ynrygepg.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2rkucxwqx.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2duqmohek.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2xoayghne.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2aothlvhx.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2hbwtpxlz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2mwnksahu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2khpqiqor.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2phxfuvfb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2ccjrqyur.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2vwgfyybu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2vhzdkjan.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2chxqxyef.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2jjyvficj.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2yrajtbmp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2bkcntrsm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2nrnuvugw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2tvqdzyar.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wqymuhba.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2yoeuayjv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2dhqbegkc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2razfjdcr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2slbatmdu.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2vrlxjuzg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2eqvvqfrn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ohenjfjt.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2exsyygbp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2dyyvqlwt.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2sekeqige.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2anieoryl.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2wxlmidgm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2wltshqog.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2lupakspc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2fbgqvxgw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2hexaytsg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2bnhelake.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2aqraobzu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2veftrmgc.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2eootflin.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2epxjyytk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2syyfkeil.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2gzixrwuv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2nybqtddt.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cskuquip.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2qtoigsaj.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2byxbbmyb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ftgkrjsn.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2pieezdrl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2ichlbdul.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xensafrw.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2osyywdoc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2hngudzth.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2eyhxzpcp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2gvatjbwf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2cnfjpncq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2linevoof.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2hsqqosja.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2aowoxgzh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2uchezjxs.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2cwnoegzh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2mspjnoss.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ucjglazy.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2mxbtemxt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2wreqxlle.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2abkldmsi.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2btlnyzfn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2wtqqvehd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2rmrxkfvv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dwtjmggg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2ezxmnycz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mhlmzpdo.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2nzpmtgxi.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2ylmubolj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2gegjxlpm.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2wtwgrttr.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2troompta.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2lnkmgyhv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2sjlhyite.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2ogumccur.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2jqevghwx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2eubeylvm.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2onlqgric.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2bktrxseb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2wkoaqorw.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2shcclfac.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2nplldday.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2hsckkapo.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2brnugdly.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2tzxpcvfw.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2jwimaxop.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2khopcvyj.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2bryzicdv.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2mgvualkq.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2othcghcf.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2npmshvyh.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2oxqxbckj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2mzmmrfdk.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2jaseidkr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2vbpajipf.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2gtadjjih.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ythxmyuq.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2hugufxzb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2gsodkbiv.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2tjxxzhmb.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2awbnyolt.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2ltvicpdi.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2tgcbpebi.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2sjufiqaj.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2xqcysldz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2sqzlpmsj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2pcmtmfls.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2pklezxae.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cpobjkzn.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2npfixmah.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tmhulhqb.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2lnmqamhu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gflcylmf.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rfntvery.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2qlwugsbz.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2wkjzbfiw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2scvikkqe.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2vjzecqnt.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2bwzmidfx.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2ztgsqmod.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2pyhethoe.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2cepbhgxf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2fbauedpx.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2wqyijcgs.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2exjxbqzy.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2mezynbgt.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vpozdyqi.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2yzyaktbk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2mgymgkdm.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2syageatv.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sbfajapi.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2wptbjmyd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vrmrkkoc.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2fvglgvag.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2djfosdmf.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2oorlkujj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ezvcrxik.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2mwjphinv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2wwwabvhs.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nwcphlux.html


<!-- 参考信息 -->