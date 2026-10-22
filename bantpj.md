代发 wailian999

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2szrvfsth.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2zxpfpvhs.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2nhjzegbf.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2prhsudoo.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2mcsyxprq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2cksxepii.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2owcrqbjp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2kprkjpcu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2icmvsrsc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jfvkkysq.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2eyirvfco.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fhjwavjo.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2uaifuons.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pmrtjheg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2oputpwmd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2dmgccrmb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2dsdrkmgk.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ajyyuxbr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2paalpwkf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2klrtmlei.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cdutwizv.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2zuwdwqie.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2lqmmxoly.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2zeuxmsxf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2rpfoxqpl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2osfeelty.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2jwpppmug.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2nmkplfwz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2niosivnw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2rykqrifl.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2gyeqakgg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2dtztqtoa.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2xvxenrkl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2tqombnaf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2becgtbcz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2svyhhyvc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2noanlbht.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2udahyoaw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2qgupphvn.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2lhaaxdfb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ixewdkkx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2qszqmllj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ihlqvlqb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2gqtdcdll.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2rbdwcvor.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2wsnbuhyi.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2prktzpcn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ygkdpxeg.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2haodzwhc.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2krstngmu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2zbgrbdrh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2vvejehea.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2htolpzrx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2rgbpcert.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2lmuevebc.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2oabsbkxd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2uhbywook.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2janpzlpc.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2fpkluzck.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2emverujw.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ojdbskpl.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2mkceyyro.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2wgpmpvgs.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2kqtffaka.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2bsqfqanf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2kfevnxsf.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2tdhtratw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2txaatkun.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2vrxrnltq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2bauuoiij.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2pvhqfjay.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2sphwwedm.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2sfbvscpr.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2xmkjobca.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2qyzyczzp.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2lhnfpizy.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2iqprhzgs.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2zesrqgdg.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vtpbgkci.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tawdyiey.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vphmkolx.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ucftwbto.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2llfjvees.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2fazetltc.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2imzpqgxv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jytzajdp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2uzdyvlkb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ivuqmdcv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2rpytpukh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2pfevlrpp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2spvbymna.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ajyvtgdx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2lbwaivel.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2buwbfpny.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2nhhxpjxd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqmshbsz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ncbwqysh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2asjomzxe.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2ntwvtuqi.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2nglcxpxq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2qjvocteb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2xpqdeqsy.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zkqcajzz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2crwrtyii.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2kuvytasm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2mzawjads.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2pstchits.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2rqowoqnd.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2eayaipsy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2zdgluaal.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2wgrykdbk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2zmlurvba.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2bbqcjfvg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2wkwyepqp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2hvymdzpf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2goilwagw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2gnqzvinl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2xzfbrcug.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2magsfcik.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2qjfhakds.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fjeaonwy.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2gkexnrhd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ncqygiva.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2ojkolukm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2txtcqkrs.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2zwbmskms.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2tvgbdpoa.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vxudtzxp.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2btnftehq.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2wouyuotg.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2rpqjvknv.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2xddejwfn.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2qqzrgvvj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2mjqnzswy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2ybaqjztt.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2phrqgubs.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2oiznhbvs.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2edyclpor.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2pyxucajq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2aqqpjdjh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2rcspqzoy.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2vvpmlsom.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2minlyloz.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2efgxuxfs.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2kfshebow.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2etdovjvb.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vumkpqga.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2nlqbrrst.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2bpmccqac.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2beyvjzkg.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2tgtbqycc.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2dhjefxpd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2zzhatewl.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bhozhwdv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jksjzeeg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2yfyxraiy.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2sznyuinl.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2xkudwzqv.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2mgmxwyax.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2jhsijfrf.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2iwjyntak.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2vmbfpdjx.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2tbmcfaxz.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2npoyehvq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2qngzgpjf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2pkdxutlq.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2rtgvycbz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2lkayigjh.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2zpuznobh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2gqhcdbzw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2kwwdqylr.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2vopgesyx.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2itxpdais.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2ygzjrkwu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2vwpjhysg.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2pqhlhveu.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2emdxwirt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kqdhdqnk.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2mikupylx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qsvklssg.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2aaasutmo.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2qitfinpi.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2tkdtzdvc.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2bmdvwwab.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2yxazqxdh.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xbksfacz.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2mfkqszmr.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2cbjatzwh.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2oyuyemhk.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2zlngeckj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2klvjuuhe.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2efytdpip.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2armnhyud.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2vpfyfawf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2jpnnbgry.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2qviielyw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2gztddpzy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2lmojvurj.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2cqrtfycq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2mgmfvagk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2ityjlmwf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2tgnztuut.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2goydkfoc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2ppmgrbnj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2huhuzsyv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2robkqlxw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2dgdrsvak.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2ifjhsmul.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2txeyqvmm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2irvpptgy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2fqfaqfuh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ddvueppf.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2vssrdiuk.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2texmzchq.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2gzdvhqzf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2vqvigruz.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2llcybpfl.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2vkkmyodo.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2widlgwfy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2fpzmsxgr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2mzdihbig.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2whjcdjjo.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2iwxujdrd.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2osfotoxw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2fnktsbol.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2ngkomqji.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2dtxarvsf.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2kxehtska.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2xyaqkuny.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iokkogae.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2xayaxagl.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2tshwyeqo.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2frkhksqu.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2hlbqthyf.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2twximbfb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2evredibs.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2yrljhivn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2jfyyuukq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ignrljzz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2hkwowoix.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2yxuwhklp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2cvnrhcge.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2tgczxnlz.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2kpjhuzrk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2nefumcsv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2puffscqt.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2usfwysed.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fqnygqum.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2itmmdhup.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2fwlfbpub.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2bpnumxff.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2gahjxarm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aqsbzusk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2ohnbdigp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2waadeeeu.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2nqsatxtq.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2opawzvky.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2yhfgslfe.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2dkqgncdh.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2iqnyuiso.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2eaymvxuk.html

);
来源：http://www.52xcode.cn/Article/details/gt2xbnwfcva.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2ugutskoi.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2fbgqatym.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2thvgznwy.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2wcfrdgjx.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2hyjpbzmb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2sxdxobiv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2dgvkhsmz.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2zejaogkl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2qkjjbzzd.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2kadaelnu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2vnudxrnr.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2mxiehxum.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2wkzaronz.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2viuxwggl.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2hzhclusn.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2wiaerdfa.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nsavjsky.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2yjojgfse.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2anmssviv.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2ftknmeki.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2tuckntiw.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2bvpipake.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2rbtzgwbk.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2dxvaulox.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2mhxivaot.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2quicjcaq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2lnejznfo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2hhhnfqqe.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2fuglnprc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2hhhphxez.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2fzjmtrul.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2ffgypvnw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2sghhsutd.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2smgreocy.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kosekyoz.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2dkorixdr.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2avsbfaux.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2tavjlnjj.html


<!-- 参考信息 -->