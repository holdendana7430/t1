代发 wailian999

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3yuhmlrus.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3fxaxirtk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3fwhggwkv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3fmqirwry.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3butvxdmo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3euxqsagc.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3yziyzgve.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3txdbjxrw.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3mqgikhfv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3riapoaka.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3tbucvqea.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3zmtjlroa.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3cuuqiwdu.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kfdffhhm.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tdsgzmtl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3zosvsuzj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ldtmvtsb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3wahhyhxn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3hrlvijyc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3kacqhinh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3pebezmux.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3xsjltcpb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3odxqdsbj.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3rneekfjr.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3foydnqya.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3conoxrqu.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3yrxqxemo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3wuoxxjhm.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3ervrhcdi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3volktemz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3keogatjz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3gdxckqkl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3hnuiyzzt.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3ysvqibuz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3mjtznxke.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3grfikgfx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ozyfffbu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3henisoir.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ffcpimxo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3gprnsvfd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3kwozypul.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3hffejktj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3vniuflqz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3hycnsfjw.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3qoxtqxea.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3wqjaksuj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3oyvvmgxm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3fqbsagct.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3dbcpzlot.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3olobboha.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3yzjdumiv.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ldawdsae.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3arvavlbs.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3ryueekkx.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ezmyevcw.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3byvefdon.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3aebwnihk.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lmqafpva.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3kyocdwyr.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3yffmtjzh.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ysmxfggi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3qxtmdtho.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3nlxcgfrt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3mgsbtnte.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3fdcszvdv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3xjvwhxov.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3kowgptok.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3xvtmeuyz.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3ddivwpkx.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3budthhid.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3zkzetnms.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3vxwldujs.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3pkspcvei.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3qqqcntuf.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pyzwjute.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3odufwrhm.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3axepmwmy.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pvqkwwlr.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3iagolutm.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3npgizgeo.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3soiqbuey.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3qlciekxt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3eivlboax.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bztfunsi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3xpkrscfp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3pmeftjiy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3ykpclnzn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fhrlpawt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3fgdbektu.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3xipeborw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3whkqsyrk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3lltyobvd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3qixhpyvz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3nlejpzyk.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3unypgfex.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3qclfhmhm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3kntyjhqd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3ptybnnjb.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3svehxhzd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3negolaoa.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3jxfpbgns.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3yblzwdvm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3kjvxrkjo.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3revwuzqi.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3jubychcg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3fyvelvtn.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3frexsvlx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3shaccghl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3fqqkntqd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3oizjwhdk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3sezscutg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3tfeqsljt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3zqtttnjt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3sfvrthwf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3zjrbbmfc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ntuocrqo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lxbmrixh.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3ldgibxdy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kzpguqnx.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3anqwgyhd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3cehcqzso.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3ijjnmujx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3sxsqlqqt.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3crafpsda.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3uexfmwvj.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3bvntxgts.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3ntlngmip.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3qchncdxh.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3csaxdwdb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3tlvpzppl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3zjrpxwlm.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3bpyxduoq.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ppyqaygq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3idbiljmz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ulhqafkn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3vizmbxsv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3gizythen.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3zdedxlkl.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ygdknoig.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3ewewqrku.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3felxnnhn.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3hmxlhlln.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwumehcr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3pskmblmq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3iiiumpja.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbxtwwqs.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3gggpaxfr.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3bmfaagtj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3dcszxhrv.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3lrdhtzfm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ogjrutnp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3nwhdxedg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3tmwjjznx.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3yevxzwcn.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3unxjfvzm.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3hpvtaclk.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3uaqtdmey.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3ppcaxxjf.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3pgqzkvkt.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3oatvcnvy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3pkhprmvt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3bksdgcoe.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3gnbfggrc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3yekluhit.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3zdgqrhkm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3fyyrhvuz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3pbylfeqm.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3cvmcwvhn.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3trvecqlc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3sgoeoyfw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3msqwbuhx.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3pbwihrqi.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3zumnuwsf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nfmhsrvp.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3jmyyfhfq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aqzbmcpd.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3wxnahhej.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3fktztiuy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3iyuuazfz.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3oqhudvxg.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3uyewswrb.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3xkjvsidp.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3umsoxdlc.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3kuibjdoh.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3oxgijhav.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3pmvhgmsc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3anveprrg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rtocjuhe.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3yzhjqtvt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3tuylmibg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xcjnrpxu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3ikktsrtd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3szdzsrfg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3twbadhij.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3katmnktr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3psirfmoa.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3lpfptadl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kosbxvqa.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3lxykhsrz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3gbmiiwia.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3netgvgqj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3zahgvvbd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3qmmzjplo.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3tuonnhev.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3tljloxzh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3klbnwjmv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3zisegtqg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ppkghfer.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ahraazip.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3rnuvjqaj.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3serevoaa.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3iwltlrzg.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3huijuzri.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3hzdrzvrw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3awfrwmwj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3gpfvenhe.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wgptyxxy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3wbqylymb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3olfswpti.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3vxyhcton.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3bvfvsuoe.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3mthlcawv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3zkdffbtn.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sxryjqvb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3wxgxppdr.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nvpqveqb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zqmsphzw.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3lqspxeuy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3dpasucck.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3xbocuzit.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3lzxtdsog.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3uuryfzly.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3ealtumud.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3rjqlapso.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3iymakhom.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3gluyjrgh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3somhuqcm.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3kqcdecfd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3pbprqvyw.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3unpvfqlp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3hwedjotj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3dxfofari.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3klampbgh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3dgjpjhtd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3agsuzwva.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3kjyksvnr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3zvbreqti.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3xrgnjfvg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vrbjwwzx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3ahfeeztf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3titfxwox.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3ptzmkler.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3rdwlwwbt.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3xlzxmces.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ieueajyh.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3iikrpunw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3vwxzyufs.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ghicpafb.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3pzrslypq.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3eaupprhb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3dnysmacg.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3xkzmbomh.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3egphuvyp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3nphzndvy.html

);
来源：http://www.52xcode.cn/Article/details/gt3cjuhfsvq.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3gbgkmchh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3rtadcozx.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3ubnbhzph.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3hacvivap.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3vtdwnmis.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3vzqqqfkz.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3wqxutrzy.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3owvoorce.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3dshyjgpd.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3xejjeokp.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3lycpfqkj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3yomhpvwr.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3cjqjbqxj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3uxgocxqw.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3awcnfhmk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3rdbhrgpy.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3bicjllik.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3hhdituyp.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3ceujbrsh.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3qtwtvvij.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3fisauqok.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3spgkyufj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3dtwdulha.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3pnaherhf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3txndyqok.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3zaorkcfg.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3lvlpmuiw.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3exgtokmn.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3poezxdde.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aeuglfeg.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3pheoyiqb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tuljipbu.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ctukytyb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3byruvjyj.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3whjpyfzz.html


<!-- 参考信息 -->