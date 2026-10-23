代发 wailian999

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3ulkyyyzw.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3dumlzcmx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3rttwkbtd.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3lzbosofa.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3maompurs.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3epcbzthz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3bwricfys.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3neqahfvl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3jcctqyne.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dyefnqxu.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3nhylplgn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qtwfguyi.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3ojtddozv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xxmwobxd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3pwuhmung.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jqzimntf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3oufkvlpg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kpurxlvq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bpvpmiih.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3iapndrnq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3quqwcibo.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3gwtqijqr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3fpnavjvt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3cucdfrcb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3edyujpkn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3lrdscbuf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3poyepbxf.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3sblhmqfs.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3glkhshpd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3vuhgymzx.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3fcswmpzi.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3yeefedsd.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3xuyqnjiy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3pffntlhf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3tbljozir.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3pxbozwnk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3bgblzrvg.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3cidxsjrr.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3ljuupnpg.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3wexprssm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3dhyaljsv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3rhtwcitw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3eiveboqq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3kggrwfsi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3dfftgzbw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3tymjneld.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kyatyaua.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3alujxfrr.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3yhhnrxaj.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3olpmwbwb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wwuajpfu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ncgzpdnf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdbdqewn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3vtkhxhsy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3psfegjym.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3bcjrrhod.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3igntetvh.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3vufhzwch.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3xwuafizz.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3jyrbueub.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ujiqvphl.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3tbkplzhw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3btgauiws.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3pofqdsul.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3keqqpokn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3axykcvms.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3ijdaompz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3mkpbsaac.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3pxqgbroi.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3boekmano.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3jtwmaijr.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3gzzmulnq.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3dwmejjhf.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3zzakvbrx.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3mvltjluv.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3ygemdfpu.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eqvrxgwp.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3thdbqhph.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3oxbepuuy.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tlwcoxwd.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zbntysrl.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3njdddejd.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3gzbxyrdy.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fydnudnj.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ksxbvknf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rwuyjbsf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fzujhdbm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3cudgrohy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3wwrvpcwo.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3dljdoaph.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3hxswyfkq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wjyhndge.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3gswaltiv.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3wwaenebi.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3nxbgsasn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3npzizxsm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ysbypcyd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3occayjze.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3ftczxidm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3kbzdwebh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3wkdxbnsu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3urefbhra.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3tufhtcpr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3yxlfkhac.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3ozohiyal.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3bpscqiqa.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3jqizjste.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3jiroqvkn.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3tdgvdcat.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3veyxkazz.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3qkcwchay.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3orimzawb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3kelqhkry.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3sujabxix.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3orznlmlx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3bqyormgb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3kpcnyqun.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3pqowiwey.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3rftvtacd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3iebnqkxc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zdngraam.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3btbmwmio.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3boepktis.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3byyffvzr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3rsrbljyi.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3zcadwygk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3tbuozpsm.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ohmjukka.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3drtumvys.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3mnpacsfn.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3hbvoxikf.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3ksgzwwni.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3kxbyppdu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3cgrowbqj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3pkuujbko.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3mctzpjns.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3tvbtluaj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3sgwxdugf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ubhhwzeq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3rwetfhvm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3zotiyaeo.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3rosrwlyw.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3wiwrpatn.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3zzourhio.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3idjcnfnn.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3esimczfw.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3sugphcgh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3vazxzyvn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3iurjopum.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3popuhbxg.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3rjmvrscq.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3volwyain.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3afsrzznl.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bbannsjs.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3fyhjhovg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3xoedvpiz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3hyzqnkct.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3vgrkrfan.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3ewdbhwhx.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3rnugnpxj.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3iqlkiijg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3upazjbso.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3arygwvmi.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3rlpgeanr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3iqanceda.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3xmxzwngu.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3arxmeqyu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3uegcplpf.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3jrndahrz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3lvcajkbq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3svzfcpcv.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3dkdkqwdj.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3nwitrhbq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3gmfymdli.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3issndymb.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3socaiett.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3fopwjcol.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wjxwkslc.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3dvefhhma.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qwsdqkyf.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ygvvpqep.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3mxfevtpw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3auyyvdrl.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3knudunyi.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3aswaqsff.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3lmafcmho.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3uhwlawmn.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3zcjhksqt.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3qeyqbabk.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3jsnejour.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3nponddln.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lngpqdbj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3svqbhaqr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3ctzchphb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3msrsvklw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3nbzrfgnz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3oynxtmag.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3rabsgqna.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jyswteua.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3esmfwogn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3rimbzysv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3xutbuxju.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3rqvzjgtk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qtymkvrj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3jyzovquu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3itygslvt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3onvmntwm.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3ckdffjnh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3cwexuxhx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3aulpmjje.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3utmwdwpv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3vjecyomm.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3luyulrpe.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3ifgligcu.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3gydovccp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3uogklkmr.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3rrdqkrpf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3ilrnymku.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3hicsizyz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3eizagmgt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xvrasiiy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3jxrnbadc.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3yrigzhqi.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3niigacqj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3jbgkmpmz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3zmzyiavj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3caihjpng.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3gerjnrdm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3lscsruab.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cdunhjkd.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tdneghkn.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3crqmmetx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3gskyuygy.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ewuwrjen.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3wwkytfir.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3lwcgvuzy.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3vguvfwvs.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3cyiqvsgd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3awwpeywx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3nwblkrve.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3kuvoyiza.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3dfjkvkgv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3ksnspefw.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3nddbarxf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3pfqabelk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bsdzrjsc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3wcpzgzii.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ptscjkmn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3wyrkccrn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3tduklkde.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3unkxkbtv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3vruqbybn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vkcwssvr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3qdvwthyk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wxyfxsbj.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3qelhtrsq.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3nqjjduzx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3wpsdcixt.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3akeozpof.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3swwlrkuy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3ojbjohhi.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3zbngtbss.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3rayipbsa.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3zpgokysp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3swdqvjaz.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3roqvgtxm.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3npyojlzf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3yexzveev.html

);
来源：http://www.52xcode.cn/Article/details/gt3bavionna.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3tnmuuoqr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3gvdcpjyg.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3eqzeejcs.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3qozqykor.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3bvonjpbf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3hzesbtvz.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3uppzmyqt.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3ypxaljen.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3gydclflq.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3ojxvuwsh.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3ichfpzsm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3nosxjybp.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3sfkkabvn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3gycbsnfa.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3gpwcwvlx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3qkjxaesf.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3jitgwart.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3patlqvkx.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3sojnwsuo.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3rjvtswjo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3xhhyhvpe.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3bkgqbfgt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3yotohebk.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3trzlkqlw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3wendqfmv.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3yzlienow.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3hncyynir.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nlthfwwg.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3fzasnqxy.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wgdrqhih.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3pgpmqycs.html


<!-- 参考信息 -->