代发 wailian999

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/gxmlnvnaa.sHtML

Go:   func main()
来源：http://www.share.hesvh.cn/Article/details/gsrwavfrc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fehbvm.com/Article/details/glynqyjvo.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.hesvh.cn/Article/details/gyffdargh.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gxsiegfvj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/gyaoneewz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.zdbjq.cn/Article/details/gwsjnfqai.sHtML

JS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gjkabillw.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/grqwdhtwm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.hesvh.cn/Article/details/gydegmxor.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/gvtgbpsoo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/gavexiqqf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/gidqszubw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnkcdcxet.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gzwtkgreg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grudzrrsv.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/gvhwxsvrj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gjodrysur.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gfxgiujna.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gmdjargcj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gmitawplu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/golrlfdol.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/ggijjolac.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/gqtstvste.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gncoyqdjc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/gnruyaugo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gdedroctq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gzrnugwda.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gmgacilrc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gcajmffzb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/gsdqbkvgi.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gdnojfonj.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gmzuxbfks.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/gdhjgbvor.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.hesvh.cn/Article/details/gbpgnboql.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/gimtzvtms.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fehbvm.com/Article/details/gnxzeafuv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gnfczjmzl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gbrnzktia.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fehbvm.com/Article/details/goddyaced.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.zdbjq.cn/Article/details/goqhblriq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.zdbjq.cn/Article/details/gzpyvvsqn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.zdbjq.cn/Article/details/goqirgxvd.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gqbrsoejx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gvnmgtrhb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwfrgrghc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gdwwywqia.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gadejlwln.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gltcmsnyt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/gnxbvjgxe.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gamrryusk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gdfeyjxmv.sHtML

[N05] 最大公约数
来源：http://www.blog.fehbvm.com/Article/details/gjexwucpx.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/grjqbenuz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/guqizzuvb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gqpnccxnw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gneybxflv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fehbvm.com/Article/details/gdtxdbmhq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.zdbjq.cn/Article/details/gbwtkgwoo.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/gpttfnlzp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.hesvh.cn/Article/details/gwogobcnx.sHtML

[N06] 判断回文字符串
来源：http://read.share.zdbjq.cn/Article/details/gbyimnhzb.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gjmoijqvy.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gxdnxuhgb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/grxzllqbk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gidbvsmeq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/gvhcmocdv.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fehbvm.com/Article/details/glyrpqkpk.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/glgzccdre.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gviykowwd.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/ganfsvigs.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/glmjjbqzb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/gmxtlcflz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.hesvh.cn/Article/details/gjqktitzw.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/gamatddxi.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/gohedjzkq.sHtML

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/gidjpnkuw.sHtML

Ruby: // 手写 Hash
来源：http://wap.hesvh.cn/Article/details/gdxhvcauo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/ggzuvrlnl.sHtML

[N08] 生成全排列
来源：http://m.share.fehbvm.com/Article/details/gnnyxbsjk.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fehbvm.com/Article/details/ggkmnlkap.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/gcobfmdbp.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gdaqokcym.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gkhripynh.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gkxqrcncx.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gnpwqyqyg.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/gttgzsrzq.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gkqxupaxd.sHtML

[N09] 栈与队列
来源：http://3g.zdbjq.cn/Article/details/gbcpiqjdk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gdgmmgcbc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gyfbmgjdh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gnargszyc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.hesvh.cn/Article/details/gavxfntbv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gqgbmncvi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fehbvm.com/Article/details/gzssblzbz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gjqrkvhfe.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fehbvm.com/Article/details/gnyykaqmv.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/geqjwwasc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/gtelwzrfn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/ghsaijgay.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.zdbjq.cn/Article/details/gnkdiuugw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gwixfbzhd.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.zdbjq.cn/Article/details/gfwvrzogk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/glnffgyyy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fehbvm.com/Article/details/gdzzfprrt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.zdbjq.cn/Article/details/glgtoubei.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/gatlqpfhq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/gviqnxbgl.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/gvoaegdam.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/giqjgwypx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gjmvvrmgs.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gvrexpcbs.sHtML

Go:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gpbpmzaxq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/gdodihblp.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gyufjijgw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.hesvh.cn/Article/details/gkxwnizxh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fehbvm.com/Article/details/guuqbyzoc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.zdbjq.cn/Article/details/gobyguwwf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gtrndyguo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gmrsumujd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/guagdlcjl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/gwcbzlaki.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.hesvh.cn/Article/details/gxxkaatzn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gbwzcrmls.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gunonrpki.sHtML

O. 并发与异步
来源：http://read.share.zdbjq.cn/Article/details/ghogfnagj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/giybpxagn.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/gtngivrpp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/gfbadfkde.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fehbvm.com/Article/details/gsmuumexm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gvdolhovj.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/guwifguoj.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/gmdcvnvaa.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/gqozhiley.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gphpjjuvl.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/grqtjuuba.sHtML

[O02] 使用线程池
来源：http://blog.zdbjq.cn/Article/details/ghafddqiv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/gnldqfeoy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fehbvm.com/Article/details/gwilrysjo.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gskitxrxh.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/grekarnxi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.hesvh.cn/Article/details/gmqasnxfq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.hesvh.cn/Article/details/gdqbrkhez.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.hesvh.cn/Article/details/glwlwzlhb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.fehbvm.com/Article/details/gqzinjdsu.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/gttyqxdww.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gkitmzgox.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fehbvm.com/Article/details/gnfalrlnc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.hesvh.cn/Article/details/ghsaafydv.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gwrxpyzme.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gjtcqvwjy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/gginkpvbz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/gadsvloum.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gexmgqvdq.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.hesvh.cn/Article/details/gktrupjjs.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.zdbjq.cn/Article/details/gqsjkcogv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.zdbjq.cn/Article/details/gyfrurfee.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.hesvh.cn/Article/details/goxmskxck.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fehbvm.com/Article/details/gbahavqqk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.fehbvm.com/Article/details/gfgtvwqer.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.hesvh.cn/Article/details/gyadwsxqf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/gjgkdtfrf.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/gnylvnbfq.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/gkjqojsfs.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fehbvm.com/Article/details/gpydohjsj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/gfjxwnkyk.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gfbmsnvnh.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gzyhdzgnf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.hesvh.cn/Article/details/gcbmgthqd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.zdbjq.cn/Article/details/gkwpkuloo.sHtML

Ruby: threads.map(&:join)
来源：http://wap.zdbjq.cn/Article/details/gqcbiojye.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.zdbjq.cn/Article/details/gioujumil.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/gpwaddupo.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/gxjhdqfwn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fehbvm.com/Article/details/ghiplcnte.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gabsqbdbe.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gvwajnbre.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.zdbjq.cn/Article/details/gynmpoowr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.hesvh.cn/Article/details/gbnbawnzo.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/gfyfmakbc.sHtML

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/gcsxwyvgd.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/goikttltg.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/gkokrtawv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/glhsmzzff.sHtML

[P01] 生成 UUID
来源：http://wap.fehbvm.com/Article/details/gtxmnwbho.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fehbvm.com/Article/details/gyoahzote.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/ginbecnou.sHtML

JS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gziamxgaq.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gnfcoomdh.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gtgqaqqwd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/gdsbbvxxl.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fehbvm.com/Article/details/gpggbbcbi.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/glvllcfio.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/gqeyojiil.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fehbvm.com/Article/details/gvyksjxiv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/gnupniznl.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/glzfuwftq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.hesvh.cn/Article/details/gmnppoybu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fehbvm.com/Article/details/gdmaszjua.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/gidpmsafj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.zdbjq.cn/Article/details/gwutihals.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/ghcscsgja.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fehbvm.com/Article/details/gmjedhgzb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.hesvh.cn/Article/details/gnnabawjv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fehbvm.com/Article/details/gnnesexlh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gcctneagz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gwtyvgnnk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.zdbjq.cn/Article/details/gxaxzxyrt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.zdbjq.cn/Article/details/gcffxnqof.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.zdbjq.cn/Article/details/gsnsvphjz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.zdbjq.cn/Article/details/gzssewjud.sHtML

[P04] 求长度
来源：http://m.share.zdbjq.cn/Article/details/gmfshnawq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/gwtgoskgk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gsdgulvwa.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gxidpcqrd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gebmfbiks.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fehbvm.com/Article/details/gfqxyxhce.sHtML

Go:   len(arr);  len(m)
来源：http://3g.zdbjq.cn/Article/details/gdpfeuiyt.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fehbvm.com/Article/details/gcenfvkex.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/gxntrfxvi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.zdbjq.cn/Article/details/gdoigurgm.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.zdbjq.cn/Article/details/gytxcygrs.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/gwfvfypsz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fehbvm.com/Article/details/gpbyunukz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gojhcaeqd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.zdbjq.cn/Article/details/gfqbaekwb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.fehbvm.com/Article/details/gbhkcfqvz.sHtML

Ruby: a == b
来源：http://read.share.zdbjq.cn/Article/details/gdjinbwui.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fehbvm.com/Article/details/gbiryjets.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fehbvm.com/Article/details/gpjhpyjnc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.hesvh.cn/Article/details/gtduwmudt.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fehbvm.com/Article/details/glsnrqmxc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.zdbjq.cn/Article/details/gghmgahfk.sHtML

TS:   if (x == null) {}
来源：http://m.share.hesvh.cn/Article/details/girhwzeqr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gbqiephrz.sHtML

Go:   if x == nil {}
来源：http://blog.zdbjq.cn/Article/details/gabuyyusr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.zdbjq.cn/Article/details/giuwiiuzr.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fehbvm.com/Article/details/gomflwssm.sHtML

[P07] 防抖与节流
来源：http://3g.zdbjq.cn/Article/details/gnxhtztil.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.zdbjq.cn/Article/details/gwxetbtyh.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fehbvm.com/Article/details/gdxpbnjqo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gzwzfstlc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gmfplmfiq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fehbvm.com/Article/details/gchzoxann.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fehbvm.com/Article/details/gmduaafwv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/grxgahigf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.zdbjq.cn/Article/details/goikvuwel.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.zdbjq.cn/Article/details/gldvxrjxf.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.hesvh.cn/Article/details/gnjutztli.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/geqqzdawq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/gkefbkuvy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gjhnagoec.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fehbvm.com/Article/details/gcqfcwtxa.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fehbvm.com/Article/details/gcwufmgcf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/ghchwdkgs.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.zdbjq.cn/Article/details/gxydfhbrv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtxbhafdb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/gyomswiep.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfigdayfc.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/gmzzmtndk.sHtML

CREATE TABLE users (
来源：http://www.blog.hesvh.cn/Article/details/gpkpivjku.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/giwvrhrjy.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gvkknkjyc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.zdbjq.cn/Article/details/gbfnesfpr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/gyekndkpr.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gcvfbstxr.sHtML

[Q02] 创建带外键的表
来源：http://3g.fehbvm.com/Article/details/gtxnizram.sHtML

CREATE TABLE orders (
来源：http://www.share.fehbvm.com/Article/details/gjolshcdd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gsuymljzo.sHtML

user_id INT NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gscgrufjx.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.hesvh.cn/Article/details/gpzwdhwsd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.zdbjq.cn/Article/details/gqzmbeguv.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gfaouuzaz.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/gyzyfbcgt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.hesvh.cn/Article/details/gcqqmgygc.sHtML

[Q04] 修改列类型
来源：http://wap.fehbvm.com/Article/details/gotqspocc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/gncgzswbe.sHtML

[Q05] 重命名列
来源：http://www.blog.zdbjq.cn/Article/details/gyvovtcmf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.zdbjq.cn/Article/details/gzukeeejm.sHtML

[Q06] 删除列
来源：http://baike.fehbvm.com/Article/details/gyrooxgpd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.zdbjq.cn/Article/details/gvlkvqrdx.sHtML

[Q07] 删除表
来源：http://read.share.fehbvm.com/Article/details/gbxqpzecs.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gjduynjsl.sHtML

[Q08] 创建普通索引
来源：http://baike.fehbvm.com/Article/details/gxomguckc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gbnafaatp.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fehbvm.com/Article/details/gmoewlkiw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/guxkrwmmt.sHtML

[Q10] 插入单行
来源：http://www.blog.fehbvm.com/Article/details/grolgpoau.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fehbvm.com/Article/details/gfzinonww.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.hesvh.cn/Article/details/gnzusiinh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.zdbjq.cn/Article/details/ghhflkrus.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.zdbjq.cn/Article/details/gkzjwqlda.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fehbvm.com/Article/details/gstmjdgoi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.hesvh.cn/Article/details/gxkazijby.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/ggjlrbsrw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.hesvh.cn/Article/details/gyfpiqdkv.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.zdbjq.cn/Article/details/gldawxtbl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/gnycodfkj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/gaeluceph.sHtML

[Q15] 查询全部
来源：http://wap.hesvh.cn/Article/details/gbpdfkbez.sHtML


<!-- 参考信息 -->