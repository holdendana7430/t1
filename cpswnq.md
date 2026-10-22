代发 wailian999

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2essrvnjq.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2fbotfglb.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2jrtzhwjy.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2huhvcyif.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2bjyeuxdr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2vzgimomm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2imfsiicr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2thtdipbk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2lwovvqdg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yagoxebf.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2qelosymy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2scgpltdb.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2idycfxoh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2sguplqkk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2szvnzlzs.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2imkgvtnz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2jjqqlusp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wgwopmjd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nvoowpym.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2pbyxyver.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vvvmptlt.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2sivmpzfv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2hcmfrfni.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2deqidczh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2grehgmyp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2koikmxpc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2pkvdprvv.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rkdhyfqr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2qivbxnwu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ktaxsrsm.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2eqtnkrzi.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2ptkdfzmh.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2qlhfhqio.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2zeiofgwf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2dqfiylrj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2ezjuqmnr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2ymumacop.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2zusmvtwu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2uyvjlzzm.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2wefqgixs.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gbdygppa.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2xskoltaw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fykimdgi.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zlhijcup.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2tvvxuelr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2eunlysoo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2adhokkaz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cuvrnedh.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2hedcmkei.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2epqabxus.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2oadkneou.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2wfuweyrk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2yrjesevo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2yovirkna.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2ushmwecz.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2vufvxplr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2rldrbyet.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2mctajegz.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2fgufmkcm.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2udkyitvm.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2dejidlgd.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wobaspcf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2anpgvuav.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2nwkmydym.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hwzofxpx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2hpiaokxl.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2sguldlja.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2wurphoau.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2yjombkdq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2sipbdjnb.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2xfnghtjt.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2uticokoa.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2ijjqpdbh.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2aargsvbe.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2jmihkrxd.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2tmflfdvt.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zepcufli.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2rbmpnien.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2bellhwqx.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2dxxsfhqn.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wzeovnwt.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jnbavwff.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2xlhpejkl.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2oazwnedv.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2tqazcwnl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2pbnyxxrl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ozdojvnm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2dsamlsqp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2whiullqa.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2aiszylmn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2xwxhbztq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2hgqhtbfw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2izuhjoup.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2povyavxg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2igjjfuqk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2gkipigpy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2anxckncj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2lpjyddpn.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2qhlreenc.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2xxrsqbni.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2ivobhcrk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2aojbzftb.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tbrgepoi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2druzwobs.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2kyyfmgcg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2radqbhsb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2pqqvxcva.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2idqyttsp.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zpboytuc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2gbsxxkom.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2yxrndunr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2pyuhfmbf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2aifmqtbl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2vffgasmk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2wadnaune.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2gjmlbien.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2yfgbhabp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2axwrmlop.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2fagtzlyt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2swrzcayl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2babqvrzd.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2tcmwwqfi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qboofmqk.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2lscziymj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2qsrffhqo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2vzwadjap.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2vqzioblq.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2bbndboac.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2xehxcvkn.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2rzizpdbo.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2dgbflbfo.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2jtprkdzg.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2djsmviyl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2yeohhqca.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2suwjpnqp.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2yakawych.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2euidpleo.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2jsnuxmng.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2kbkqbesb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2woxdgrnf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2jaguumzq.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2kcjstymd.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2ormotusp.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2rwhcqujn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2zuivphny.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2vczcfore.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2deqohxrd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2rbwmyrlz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2deptpucq.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2hzinelck.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2tsbadsug.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2shrqweyj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2gwkbhbvi.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2twvhyywk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2svgfquze.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2knaufguq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2azzhyenk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2wnnijhfx.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2wgamvldl.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2ustmfrzq.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2snclsvmp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2okohzshw.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ddvulvxg.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2cgshaoys.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2dlohfdni.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2bkjyhxfn.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2gttglher.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2pmbiumzf.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2mvpmlzbs.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2lbpvzetn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2nburgkys.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2bsqmmwan.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2nzmybisc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2hfbckind.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2bhkwxugv.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2pzanlszk.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2jttrdejm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zglwtxfe.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2qxvatpge.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ppmlvrit.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2pmrsxegi.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2trapfzgs.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2hdzfxmfu.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2gpsykqfb.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2rpvnpawi.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2yanmnfnw.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2wkuwotgm.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2zpftxtzd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2fdrshjmj.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2ibvsiwng.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2mlupoiqm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2kgzdncdl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2ttuoaroq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2bwjkhpgg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2wyvyvfvl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2mmiggwzq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zcrakgdy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2lcybjxuf.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2ktbcxqls.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2zjbecwyc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2gcrfobzt.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2gdeftbbn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2knkhxubx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rqehosnh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2trbtghis.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2vlrwisvx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2ebkigvus.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2ykgftfvs.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2hsmtliap.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vzbeytll.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2jcwffhdq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2cqfovsio.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2lenidcwq.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2vfbxcdog.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2ygyxbsuc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2jvmjztfd.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2fzmxmpeh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2cpguhjeg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2yqtyikda.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2wkajudcb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ofqgimdz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2egphsvao.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2adefynja.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2oqbaeokw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2qvlkjakq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2deoktebg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2qyyrbinx.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2olrnmlwp.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2pltgsldk.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2itioqwdt.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2bzudaclg.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2jsnvdtqa.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2abibwziw.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2ebefsuyv.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2clzsvsor.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2uxxlnsyu.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2jqybqkib.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mmxvydfp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ftgoltig.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2prpchvno.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2hmoiakfw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2rlbyewgt.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2nsddjuqv.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2taazrnys.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2vnexthnx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2xvsxjsvv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2otfzvtpd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ihbqjbxp.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2evryaqdx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2qcxywuiq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2cfyiolfu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2kvxmyrdh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gumbhxhc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2xeyammtu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bukfpdvd.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2tsgsgryr.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2zjxdhafl.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2txwtbrgz.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2kezlvxjz.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2poyegfgh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2wnytrwjh.html

);
来源：http://www.52xcode.cn/Article/details/gt2xnmcibyr.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2fyhipxoy.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2howevbhm.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ueseafyz.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2fxpaustc.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2ygtzldkn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2uvengkgs.html

);
来源：http://www.52xcode.cn/Article/details/gt2ryedwljk.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2zhkkqhph.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2antfffex.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2kzvfrvft.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2njaaushi.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2wslcrlcv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2btkgmilg.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2nkkvzwer.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2msgqnzac.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2kngpqvys.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2ofotxfrp.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2llqrladp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2qjpfjhwt.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2zdzdvipg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ctiwtmnu.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2mztnxkye.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2cieqozin.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2munapwmp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xtcnukev.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2mbtrvnjr.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2pztcajcg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2kyoolhwb.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2togbythg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2qkgvtugl.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2fmravify.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2pojtacti.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2apxafaae.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2hbqmxnkv.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2exbgkepe.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2kznjbvfi.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bncbfitm.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2yxgdlujv.html


<!-- 参考信息 -->