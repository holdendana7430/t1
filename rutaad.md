代发 wailian999

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3dcsuctek.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3qlyctyow.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3sqeegaxs.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3vhpzfwxc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3vjgyshjn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3exxljqls.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3rmaomeij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3linbkpsk.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3hswmffqf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vuclbefv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3bgahqmgw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3krstgook.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3yhagfzmo.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dkldqpce.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3liyiyikx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3axvvpheb.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3szbzseqa.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3rppwxgdm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ogqlopgv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3cbebmrov.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3jgymenrq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3tlmrvkzo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3euctnzml.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3gqduqymb.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ktsqtsyr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3tocsqxvl.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3fptaumlt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3fxsrfaub.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3buohxcyr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ctmyhlpb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3pqdudqbz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3luokwgna.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3jeujcamk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3bcefdlkr.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3whegzjqa.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3dpioufbo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lkhrcwkh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ojodezbl.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3redmxkea.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dzxpjrwt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3nfptjjdn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3ertfszph.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3cnnywssn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3uihwyfje.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3tjonlfiy.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3faxkzfji.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3wnumsejn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhwfavim.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtobgvmt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3lpzpmafh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3dgcjdips.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3ryphiqna.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3jnbjzvtd.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3zzziqdwx.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3fhpxuxgb.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qqztzqys.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vulviekh.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3rgnpiltd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3fqcgavew.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3blggswuy.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3gwojmvqi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ahnoivpw.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3jkvtcxxy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3jhmhfcxj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3gcwaxiqd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3skgqtinp.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3drhvbmvv.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3dftnwdxf.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3eszbwprs.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3gofkoygo.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3rfwibdjq.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3nkcjmoya.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3udnphxfm.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3xlgdomql.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wgszzdfy.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rliwbhqp.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wbyqieax.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jdvhkoxi.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3afpnrtuu.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zmaughna.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3zzomlvsa.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3prtzotoc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3jthdufxy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3pebkanhk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3ppifwtcr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3papqdbte.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3yvlglldv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3gymicbwp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3uzjrsqhz.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3jsttbten.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3nzrugspc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3sbynqwcs.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3vsylnwcg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3cnxjntza.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3bqtgdglq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3gbtkmuxa.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3wvykszcy.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3tunyqasi.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jnauxypx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3mwnjfimh.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3irlhefpl.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ksmfcrwy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3osvmmjmu.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3lhyfpgbu.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3keaqubgw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3smggfwne.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3dmgbojtj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3sibntlld.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3rgoacenr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3utdnplmu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3oqfbuezg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3iwggbbqp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3lrkhtzen.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3hwuvqhyl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3vgujhvdo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3hnbvzxcy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cyiruqdm.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3aaxqunnw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uanhpvsd.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3tijlclat.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3sisoevcs.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3fqdfmedh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3qvaizrni.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3whjiumbo.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3bqsghbsm.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3fngobhnn.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3oytlhhde.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3xhbbkjue.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3ykbfhefe.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3ddlvbybl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3ogizhest.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3qrlwrnsu.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3jmptjyvp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3qdimleps.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3nbzswydg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3brsdpvfg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3mgkzqkwg.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3xoffnqku.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3lbplqbky.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3vcokcgkc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3gdgeciut.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3kawrqyrj.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3jdtezqeh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3gzfpxidh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3pscqyzzq.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gfvaddie.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3lvjlwlgd.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3ccwbhrgf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3letyctuv.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3qfwjmmvd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bknqwrhc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3mytmcdut.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3pxqfnscp.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3knmjuafx.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3mvxbozby.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3ilzibbjc.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3jmgumdpn.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3okwbjaci.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ldhbcggw.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3jfhugagl.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3bmoygarh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3csbiceoy.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3hkianyhm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3urhcwzjv.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3qwxgyzgf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3oxjapmwp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3viteiqxx.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3xthsnbny.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3vzhddmwm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3ahrrexnb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3zsouyiko.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3effolrgc.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3ohtpopof.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nbwklpwg.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3shhfhxxs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zvnionfq.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3qqerpdqc.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3eivykonk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3ktbdrnfe.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3vewtnlxt.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3jpihqffb.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3cejeeplz.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3zgpllczc.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3xqelyuvq.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3lkjweifd.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3yvwzfsda.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3ttldqtwc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jogymojq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ovlgvfir.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3fpzwyowa.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3woxsmcob.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3holrknlu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3pidrdwuo.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3cgpwpqja.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3cpsufmae.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3joqvdepg.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3xydnewxf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3whoqblcs.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gopfxuql.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3cxbyknni.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3tvmfjkax.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3hzwbcubx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3tflupbhj.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3uzlmbati.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3wwglqxpd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3emsfzyed.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3cnczvyxz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ulorjcwq.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3gatnjgeq.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3cpqyuhyd.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3znphuxan.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3kaafdfeb.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3aqzgljkt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3akjxoupj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3bgheobzz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3isqqvnpo.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3jwnocibo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3tggclaoz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3afkpsalg.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3yaunpfyg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3dptccijh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3hyychely.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3afvbyawp.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3drgjlivq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3gdlrndaj.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3xigeqets.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3dakwxcrq.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3zoonomzg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3tehugvdx.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zvlkakws.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3veajkpnq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3nmcybtru.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3isrjjmor.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3rmvmzzfm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3wwulcywq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3soximytd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3ybduoygd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3yinigqdr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3qgogkfnn.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3gffvvwcx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3viafemah.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3sjqcimsc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3ojyzbssj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3zakgvzeh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3oovvpnri.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3eaypxasy.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3rdumehty.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3lstcksxq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tqacdcsd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3nvdfltxn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wdslinai.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3rsuqlvjz.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3yfyvrgbo.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3wpecdkqg.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ulotvyek.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3comoddan.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3hrjkfitt.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3zgmqriih.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3dqfwbxzw.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3szfhszpr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3lbjrpaap.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3fkldrwfz.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3opvdvqti.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3udqxnjgu.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3jwujrmzf.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3ovuxxvmp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3tcvlwfvg.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3bntocztc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3wypbbmxo.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3guqscace.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3sxvfiinv.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3vqswbcpc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3mcqlzjzf.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3bvlwwtev.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fizygaki.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3osjnszkk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3bdmqtdis.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3krdjyomg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ccdykdwb.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3eilqheoe.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3zbdwgrpp.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3tssrnzbm.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3qonhlwfa.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3drdywydh.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3zhjskfgm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3gtxbknly.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3yusxteve.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3gklvibbi.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3mrqcifdy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3zkizxumq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3qbltwxan.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3aypqalpb.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3askomfzn.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3vrdczfii.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3stchwpqk.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3ggpguirg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ijzqserw.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3hlgydlyc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3qusfeesu.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3qimqhbgy.html


<!-- 参考信息 -->