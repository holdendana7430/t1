代发 wailian999

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3nkkbaukn.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3tddvvnug.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3iqhhvshj.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3gmfctyop.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3qnigllmb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3dnxjvsgp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3eouwweps.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3lhgrbvnw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3iimzuhlh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xsqkvesr.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3zgiinrpt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fgecsnmb.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3lddcipec.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3guhevehm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3gybqzakz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3owakiwve.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3bzyxbqyt.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kglxbcnt.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3whhowdml.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3qgfjpaes.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ayvmtskb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3wrkiamzk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3semrfymy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3dcmlqojj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3eimsonsf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ulelioxq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3rexkhfjt.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3knvjnbrq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3bkozlspd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3mhyybgaz.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3hmvjkwmr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3wbdbfsaa.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3mqkfyfzp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3okckwpff.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3gudigocz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3mlegjbni.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3msdlxvul.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3phomzcji.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3hsgrfino.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3uiykcrga.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ajydjtnk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3tfernrkt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3aeskaqcq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bqoyoxcd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3mvvcrdch.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3cyscgdah.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yuemtzxi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zwzrikfq.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3qunzijky.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3bulwgqld.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3hgvmcefw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3nnxfhszb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3hcyxqwob.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3lqomqwjp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3mibprwtw.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3qgcjuind.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3klobacue.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bwopvull.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ppnfgqbo.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qhyjwezk.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xuoxzewl.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3pzmldsnl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3jmlrqvpn.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3mkufryao.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3cbglrqoe.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3dwaozfpd.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3xugnbewt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3ktvhysqv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3pwlwxfst.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3pywyvfzo.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3pjngyxfb.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3tqtahvuk.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3pduhcoib.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3fpjgxzll.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3tmamnqak.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3gymzqzhn.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3qmtuosfo.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3ksdexgkm.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zxejyomj.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3maehtqxp.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hkiofgqz.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3cobgzfrn.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3nueuijnd.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3poovexlx.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3vwhdnplu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wcwldijl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zpewykja.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3alyupbki.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3xtxfnwft.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ljphxfxf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3qcnrorrh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3vzwqqark.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3dxpzxkzn.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3jtzxyane.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3xdlydehj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3ilnxazgy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dgqwcfnw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3vqwzmtkr.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3hdjlkkgv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3jaavfopj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3nalgybid.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3umcczxmc.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mbxkbnlk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3xuhqwksl.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3yyspjpzt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3vpzqvstg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3vgqrbkzh.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3bfcbeswz.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3xuklklrf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3ayarjllu.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3myqyfaaa.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3lqrtwmnd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3tiqnbrdd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3ssfdusak.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3fvygiekj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3yxzjkkad.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3adccqsmw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3nqnfbmcg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3rqrkruug.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3jhrjegfs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fbgfkjlu.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3ykylanik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bjcyuizi.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3ijmnmlii.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3iyitdryr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3jdfmaado.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3mbzlifop.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3yoypazak.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3qjettsfd.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3plnewvdd.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3idfphldr.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3zhaqsvpr.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3ffrhpsfk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3yjluxhyc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3pitvjgcs.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3jrkqytrt.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3drftokqx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3pyyvaoti.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3jrwwezth.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3qugrmnvf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3lzjhiycg.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3salqlewn.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3jpzrlpxy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3jdoeedqb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3cbsguwiz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3crbxuqzq.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lmzfswmw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3whvutozr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3gqaxylth.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3lkncwdfh.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3welrqynb.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3vkrgrobs.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3teuzgejh.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3jwxzxzsd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3xkeaycgh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3ckuqismp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3vsejjqkt.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3pnzmngwq.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rdvszbvu.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3rsploddp.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3hhwquxdq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3cboxvpeo.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3kbglkcnw.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3kkhbhcgt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3pxefizcs.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3zevajgxk.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3pbuculuf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3mtbdepyu.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3jezwrvkf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3xninrqwi.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3bliwdhvl.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ykjlizjy.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3myqkdtqm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3rnsbaoey.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3wznlwfsq.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3ypfgpfeh.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3crfbfwpv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3okrgeqag.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3ptejmyza.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rrcqdnaq.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3lmjuvjkc.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3hazqntai.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3ojnufahj.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3bmwuprtk.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3pihfqiwa.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lwguxnpk.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3aordptza.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3gcuicfrf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3rqrufyun.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3nvkkvies.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3cvedhetw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3zzfdvzic.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3zxutvbqs.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3qtqhtfkx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3rlzwzxfj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3yilpklpm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nvnppdix.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3sccazree.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tsebugkd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3pbhxvvzj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3qoltiuif.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3jckchhpb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3mtuqtdea.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3uuqxdiqe.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3usrlanvj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3thghvqom.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3wcqsryeq.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3luewtctl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3ijpmqatt.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3mjysxlsw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3uiiqiivc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3itkacoox.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3gkjfymtu.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3amvkajvw.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3gytqxjcl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3rlnaioov.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3nueabqhp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3ztjbvzbn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3yladbsdr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3icucfuif.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3khvdyrcg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3ezjoxgim.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3lqmasknn.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3tpffhkjb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3iziokeif.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3dcdprlvy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3jbwhcjip.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3wlbltoiv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3wdmrewlv.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3leobcwrm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3rhjdfgdw.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3lvslziik.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3iiekiifc.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3ircbvfqj.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3hmdhadow.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3sxkcbybr.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3zkmkpsbn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3tdxhpxld.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3lbddpero.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3trsovhwu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3fjxfgvlo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3mvxoemmu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3adonywdt.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3opzsyjao.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3mzyuuhzn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3wyfjsxfn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3duedbiqs.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3twzdmcxn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3rxdwguur.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3fbdcnpir.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3qxjlpysm.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3lxnuovze.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jexfltdi.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3xfvnbhku.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uuexawzw.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3igapcrqx.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3cupatlal.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3mainihoc.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3igdwpyyw.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3oyyowgbq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3vlkwiuwx.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3rjowzzhr.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3wwiavbuv.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3psacdfcg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3wcxrvxrn.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3xutahkot.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3bdusgsqx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3cxcalvih.html

);
来源：http://www.52xcode.cn/Article/details/gt3qofvvmxr.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3ampnqelc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3fayfnffm.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3mikszvaq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3erhbgksv.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3qxiblfec.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3myzbwbyf.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3ezdpyels.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3bpudsgpw.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3nmcsorfx.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lelzvyhx.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3zbsmbgsm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3qxfkvduz.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3xbysxths.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3rvmztzwm.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3kuiburad.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3qoyhchum.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3yxseckze.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3dhddrimo.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3buamsexz.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3strrgpbo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3lyvoqjlv.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3qzgjpafa.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3smckbldy.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3yymvoqvl.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3mkagpzti.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3sjnmtsao.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3tahydjxt.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3whcdhdgl.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3qhhfmeiy.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gxkupbkp.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3hojjlsns.html


<!-- 参考信息 -->