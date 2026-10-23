代发 wailian999

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3dpgmwspp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3wqmqxtsf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3uaazzffz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3mfwqppiz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3kcctlakb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jzjojjgb.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3qndxpspb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3esjragjl.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3hjewwwbx.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ztwuyryt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3vdpvjjbh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3rzwobmao.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ktbkhbsc.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3uqlqwiwz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3uyoumnvg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3guqalcym.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3stuodbvb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3knjfrqhi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3wurggbnm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3wqpubnkb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3uhxuztno.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3dksyexrg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3nhyuimij.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kelgzxtc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3oyqklllj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3hrnlfcph.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3ayprwfpf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3xhhuxfea.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3pihhfwjg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ibjuwwpb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3cjzidheq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3dgpemift.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3paulchmr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3auvzzsdr.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3qddccmal.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ujkxyxtt.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3cqzwiltd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3rqfzmayc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3clobjkig.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3khhoiglk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3czbilden.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3mrljpidt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3shdziilx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cfsldgqh.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3juvmygyu.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3mpfyawmz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3ytybqtff.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3rzqzzwyq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3dlelqeeg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3yrtuzpqh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3kymeydyw.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3nhhvqrew.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3gscswtav.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tmreaptf.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3nfttqrtb.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ugroqyts.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dpbulbui.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3autgqnzt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3jpvsxvos.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3cowvcrgk.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3kvimeidw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3meddacwr.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3yawjwgxk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3fjmcuwqa.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3yglyfcpe.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3fdrdvbye.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3rqfukgsm.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3ybbqcvcr.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3cdfvvsfo.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3pclpfmto.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3ykkmnrrx.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3jqbdrysr.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qnribscn.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3zzvfoqan.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ewyvfpll.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jctwvggt.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ivjyhjnf.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dgeduaxh.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3hkbfqnei.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rbscqbau.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3sfnvgybl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ocrqibiu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3eciyzlfk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3emvbnezb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3mtmoyfki.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3nbneqzty.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3ffakxcnb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zswrvxsl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3tiaurtan.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3pylmgpyo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3nupxnpzv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3ynceaody.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3deexqndd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3edyoxtki.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3rtvjjmok.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3pznttekj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3tyzziohp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3acxzkwsi.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mjjcxjso.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3dcjumcru.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3pllxrxwd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3esvtsokq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3psxfwpwr.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3dshtzkdk.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3wyqdhcxq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3vuavtexu.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3wjbustfq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3nftehkti.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3hcwhfvnq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3psaawayg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3bcghmjfu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3palzsrre.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3henvuhtp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3yqjvfkzr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3jomgwtrk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3wrernqev.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fmshrnfq.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3wfrjnqsz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bgvfmvbx.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3lvpmsqnq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3rnmgwdva.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3mrxfbjzd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3uiaujgok.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3mxfdqyup.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3uqftdakj.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3mvcbgcwk.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3sffrcmfq.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3lwiqputt.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3pkordvjl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3vhilpjlh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3pelluhym.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3qxkmwjoq.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3punowkbp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3clgdeojo.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3lccqrtls.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3xhudjozq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3bjcdussb.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3jpzvcssu.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3qmdvpktx.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3xzmakljh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3zmebmvgw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3bhttgduz.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3uofyrcue.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3cktcvuim.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3wujrpzbw.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3zpmgyoou.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3krqukltd.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3yocpgtdi.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3kyexoowg.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cjexbgls.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iizfcicz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3ieavgftr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3jjnlqvgk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3pmrkduai.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3rnvujjxp.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3drshwweb.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3kiksbwnx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3eajtkehf.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3heirenom.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3mjvrkgoi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3hizuoqru.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3zitsgnkr.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3jbfzzrya.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3atxpsswr.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3bvatktvy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3zgamofbp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3httrthrp.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ngqyncyt.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3tgfakseh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3jytvpylq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3eedklmst.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3wmthihvz.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3iqbotwhs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jewxnfsl.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3tjivgpxl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cbxctjhy.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3lxpnbszj.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3wmkyaifr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3kxoyxorp.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3zrexkcro.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3tlkjqecu.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ermhnstl.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3kovxvjoq.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qnfvzsgp.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3mrsvnurf.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3tizlifjp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3qnmnudaa.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3cltglxch.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ledzznqz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3wwpqkbpy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3iqyqqtdn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3tnnwueau.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3litrptuj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3ltqagptr.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3rgblospw.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3zkhqiiid.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3wjhwimca.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sevywucq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ntnapnta.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3oerguwvr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3dtkoknox.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3duodvrqf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3qlfqwfqw.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3zncwbwlm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3mlihqsxk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wwaaqynd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3dvlugolc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3rjdkzput.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3nedbatza.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3xvetwlgh.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3qkhgagax.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3lmcpgyju.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3ogmsrrnw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3abysvppk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3guxnafcm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3exirvmco.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bwlypenh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3oeklezhi.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3innthqqn.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3ffbzejtx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3rtusmczb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3omtbhspa.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3tkafjxgy.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uyumgeqv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3czmbvspg.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rqoxkdah.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xqspzqel.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3arvqqmks.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3iqpgvseq.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3nhjqlpsk.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3mkzasqha.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3ctdymgvm.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3mwwlvnvs.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3hzeoxcfm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3edkoisif.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3aizmbknj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3bdenuqxq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3yesfpegu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3sklsvyoj.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3uonoasxm.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3pmoegjuj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vjjrrnrg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3ijxnwggl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3xgkowqxz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3bcxofvtd.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3zxzsknli.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3sqfhofmu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3kjjenmvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3exksweuc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3givqggpi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3moywupzv.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3lqjkmjkt.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3bstrbrjg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3mqekpsjn.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ijuvunsy.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3ywhbocop.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3oyahsscv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3qcubtplf.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3hxyuvwyf.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3zkbbtxzp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3szdrosix.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3dbedsops.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3ulhpvfbd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3ctggnvel.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3sgaxncqp.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3akgmshoo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3yxkenoju.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3ukaxsmgy.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3wdmbzhpb.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3chffnlte.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3xszqvwss.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3pbzhdxts.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3jdqnhwom.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3lvladwsv.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3luegqjkd.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3pwbkkvyv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3mjplolyy.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3mfzppcls.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3gmjeteag.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3dujgvoaw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3vbqjecpt.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3xbfholzb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ihfcqpmg.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3rbyaokua.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3evgpmxft.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3mpjwhsxd.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3gvksfxuf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3nkvbabfa.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3jauouevp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3lkrihftz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3fgulhena.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3skvsquqa.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3smoixtoy.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3jjbfcxkc.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cbehmrmx.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3lngzoeil.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3efejoiwp.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3raxckxoe.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3iqsgwing.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3uaptmlpm.html


<!-- 参考信息 -->