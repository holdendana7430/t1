代发 wailian999

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2hvwqgaft.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2nvixuerw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2fxyfvyeb.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2uwlzbuhm.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2cttqplhh.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2yexcjfss.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2qkltfxgl.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2veccgkhy.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2wzlkbpil.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2wtwdkyoa.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2itlagdep.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2aeblnedq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2isptjwzn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rfqjzqxv.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2jqmifnej.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ouxdwgzx.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2pnwdnvuo.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tzwywqpq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ijtkrtiz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ngkqloae.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2myxvyjmz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2eiuolcdh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ospqooby.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2utedgllz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2liruhiww.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2hmfgqfyd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2mzvllljy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2xdfgamfa.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2emgyejfj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2jygeedxi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2hmjvlklt.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2phlctjpz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2gymjxoeq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2ragsfgqr.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2xkzhkyao.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2utexllpr.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2fatnbivy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2wuyqmnay.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2cnttbmat.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2gnggdsvn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2wkliqoyz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2itkwwnps.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2vtyfjnfn.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2wirpnlma.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hpnegdge.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2mtyjnueh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2bpkwjnbh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bhxlnubw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2yrfdkudr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2mvtdjiby.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fqibbufp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cftwjpfd.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2bmldrfnb.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ecqnegji.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2gdhfmxbx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vrwuyqnr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2qbwkzydt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2hmkrnzqe.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2ttcexwxu.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zcrdvjsf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2rtenkcpa.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kpdzcyqf.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2cyjswbpd.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2hsadkneu.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2oyehvxjt.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tkykgjlr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2xseuuwol.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2zjaowfhy.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jgylbvho.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2driowbeg.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2noazgpnv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2wcdpirmg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2jnpoeibj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2wgaxuous.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2qjzmjxkf.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2nhlksolo.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2bxrdqiid.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2ehexkssh.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2gednytpp.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2qlrgujsb.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2udpxgcyj.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2txcfwexp.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zrbfejoc.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2aadtmhot.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xtsgaepw.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zfxdwayx.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2yulvelub.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ezuadfxp.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2bcbrugno.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2yndaxzzq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2gwprudyr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qwueizia.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2dgopcqbb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2javjqoiq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2joguejrd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2iqlreujk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2qhpwsryb.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2pfuxwyth.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2houbirjr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2twkuicnk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2idffwumv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2dvpegsgf.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2argjbisj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2fvvaoltw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2zohizpbb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2gomalrnu.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2prbawutu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2tjeiptkx.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2tkvbmzmo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ycioyiyu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2lcwncofj.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zymlbdwe.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2wgwxhqor.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2rxhershc.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zkapnalc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2crpvyvtv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2jpfigezi.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2souyfskm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2xzgkhjrr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2pwpjxcdm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2xaxpheci.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2gtkwetsa.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2cpisehok.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ecqciubz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ppxldtnr.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2ehcscyvk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xyjbvrhm.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2cogudofy.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2fxkzdaih.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2hgpzpusw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2lpuwehpt.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2pfdwqlna.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2bgyxcizp.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2xtqjpcyv.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2hzfxbnvt.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2xtkbfrma.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2npgciomz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2hcdgczrf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2xmqnapjs.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2iasgfite.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2thcdxwhr.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2ljkgwyxa.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2hqwbzrze.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2fwwajcgy.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2rqzbhcon.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2evljhsal.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2lbkjxodq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2utsmhbgt.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2urvnqozb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vxyonpsy.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2wymbgtnr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2ikpjufby.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2gqdcwozj.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tptopiex.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2eenvfxpi.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2cdfycdnr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2estrndbh.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2orvrjtmi.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2oereatnn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2xlwgfthy.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2ppqkyqlj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2sbumfjtf.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2cstmfaxe.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2jyygydhk.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2wbmjyodz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2wpulylrj.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2snvclsle.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2cdxeijrw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2kpkofork.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2tdcwegrj.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2rvqydkvl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2qsclotrb.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2qsjiidke.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2btlhvopk.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2efbovfkh.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2tlxdiloo.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2gyiqlqzf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2fllqmidr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2tzumixjx.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2gmkodvsz.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2jeuyoasm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2laaankiy.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2pepwxgiu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xaweucfr.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2olptsfvg.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2hifxyfhb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2alfczama.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2vmuqyxgr.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2yulakyus.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2twlptlqw.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2echoxdog.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2rglwgmll.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ocmtuaed.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2eaksbrct.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2vdjfpxxe.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2uvbngvzb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2twlgevph.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2ldyuhwmh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ohaqmxgm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2vbwvvwdd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2irtvaaom.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2fcnyrjhm.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yxevfosg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2hmzybbjv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2uindthgq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ukfkfhyt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2fxypzsyu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2csvosmje.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2heobqtfk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2rtmqkzlh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2ivubijbq.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2zcfybbzd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2ezmcwkiq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2avwiupba.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ttaybqrh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2fakvdulv.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2cfcybdmz.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2wzsuenlz.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2loksgvsw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2rrrabtul.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2wzwookmo.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2bypfojoh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2ujupdrrc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2facinejd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2guukapjm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2crvotolu.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2alnwiflw.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2nrfmabsz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2glnofjkc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2gyzabydq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2yfbltfjj.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xuifxaum.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2wuqyndwd.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2yookixuc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2btdkddif.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2pxstktii.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2wzfpincm.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kykmvajw.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2nolbcdqo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2sjeneklr.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2xxprpyys.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2jxnnbrdn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ibmkdrhp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2xlzeszjg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2kweltrlt.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2gqryvqiu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2mxbefxne.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2cnnnxwpm.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2dprddxfw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2eybliiij.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2daeszmxu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2igglpkjt.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2dyiarysy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2nzagyvtg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2quravmmu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2ikeplbps.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cmkchqjh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2sedyouzs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2itkiubup.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2uklqrwxj.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2vprklubv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2czowrnez.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2jtkpvtph.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2bstjwiwv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2wnxuullr.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2qytprpbo.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2elbasduw.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2ezxzadle.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2syvgjpsk.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2qaknrxew.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2jxzkvkjc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2zfjkeiks.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2jdjfnxiy.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2pshfaovl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2niwaxiub.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2xubgfdtb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2qxvexxxo.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2koqdgqbv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2rwfrvpii.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2etnjkczg.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2yiyuyhll.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2kswwxpup.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2banjjjjp.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2ujdnnyjt.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2gzltotgk.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2hdhmodlc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2jgnoahmn.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2uwqeuwqn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ootbekzh.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2pggqfgal.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2qjiofvnf.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2pfydgzjx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2jvssrvjx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2qdrwwsts.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2uykfwelz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2vvreulph.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2sdzetmab.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2kkhtgyac.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2pwswekei.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2xnlnucjp.html


<!-- 参考信息 -->