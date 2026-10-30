代发 wailian999

Py:   if __name__ == "__main__":
来源：http://m.share.hesvh.cn/Article/details/gpjfwtczt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fehbvm.com/Article/details/gxtuxyovc.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gejvthrtw.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gizupddeo.sHtML

Java: public static void main(String[] args)
来源：http://wap.fehbvm.com/Article/details/gizqqtqxa.sHtML

Go:   func main()
来源：http://mobile.hesvh.cn/Article/details/gurzdyozo.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/gvtglsxap.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/ghjxyhnvt.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gptkfcmdd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.zdbjq.cn/Article/details/gikfzmtpb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.zdbjq.cn/Article/details/gieyrifff.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gnljyxzdt.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gyvupxssh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.hesvh.cn/Article/details/gixxonqmi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.hesvh.cn/Article/details/grygbhlqi.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.zdbjq.cn/Article/details/gnqittazm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fehbvm.com/Article/details/gdjvkdcxs.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/giawzczsa.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gfdfbypmx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gojacnhyr.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/ggnmvkkxm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gnerppeec.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gfsslubyp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gklcodkks.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gbqbfflah.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gzvunhjhi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.fehbvm.com/Article/details/gkxyxbdbu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/gkrosutad.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/guikkccwt.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.zdbjq.cn/Article/details/gmyqozcwi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gknwdqiaq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.zdbjq.cn/Article/details/gkflihfpr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/goovrmfut.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gdeqzzzed.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/gbghrjdnf.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gsjylzgvm.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gvthfglps.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/gponbxxqk.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/gymfjoroh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/gswsmwdhq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/gvecbchzl.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gytrayeou.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gbxalamxq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fehbvm.com/Article/details/gyiibvbaf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/gxnsmzzet.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.zdbjq.cn/Article/details/gdcczfgad.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/grpzmiprq.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/gzdwehhyx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gndmhpgfh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gitudavhs.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gvyuzfwcf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gnbkwrupq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gtahjhnwm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.zdbjq.cn/Article/details/gfaykxbwj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gsrmsaubl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gwpzhmtxk.sHtML

[N05] 最大公约数
来源：http://www.m.share.fehbvm.com/Article/details/goohfedhp.sHtML

Py:   math.gcd(a, b)
来源：http://blog.hesvh.cn/Article/details/gurnavofl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/gepdrrehy.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/guvewnbfp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfzvipumr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fehbvm.com/Article/details/gpaelpaqa.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.hesvh.cn/Article/details/gqwvlkzns.sHtML

Ruby: a.gcd(b)
来源：http://m.share.zdbjq.cn/Article/details/gjizqqgum.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.zdbjq.cn/Article/details/gvxokondx.sHtML

[N06] 判断回文字符串
来源：http://www.blog.hesvh.cn/Article/details/gvbrqcdhx.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gwlnlayjc.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gumsmsdeo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gpeqebeoc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gwdqopmkp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/gjnbmwcxm.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.zdbjq.cn/Article/details/gabzcoyfu.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/gaxgskfyw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/glpyfpdcj.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/gteaouptt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.zdbjq.cn/Article/details/gdgyskruo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.zdbjq.cn/Article/details/gcyogqnor.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.zdbjq.cn/Article/details/gtpfstfpc.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/ghcdkevds.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/guopubhry.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.zdbjq.cn/Article/details/gyfjuoezx.sHtML

Ruby: // 手写 Hash
来源：http://www.share.zdbjq.cn/Article/details/gyerrujtr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/giexqyzoo.sHtML

[N08] 生成全排列
来源：http://3g.fehbvm.com/Article/details/gxhsgqtpy.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gkiksuhon.sHtML

PHP:  // 手写递归交换
来源：http://m.share.hesvh.cn/Article/details/gfgkcwoiy.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gzawuthtx.sHtML

TS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/glwfjjerm.sHtML

Java: // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gvgjvyaiw.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gnzojkgfr.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fehbvm.com/Article/details/gpglmdkll.sHtML

C#:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gcdhsnfur.sHtML

[N09] 栈与队列
来源：http://blog.hesvh.cn/Article/details/ghnsierks.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.zdbjq.cn/Article/details/gnytdvmcy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gifdzpece.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gvtqzbfjs.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/gmdkuymbt.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fehbvm.com/Article/details/gpqtkmpwk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.zdbjq.cn/Article/details/grcjwbcyv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gbntofeaq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fehbvm.com/Article/details/guqptvpjn.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gksrbjmwp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.hesvh.cn/Article/details/gkzlihpgb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.hesvh.cn/Article/details/gzohzdafm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.zdbjq.cn/Article/details/gucecngrl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/gwnvyskwt.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fehbvm.com/Article/details/gkgegmmtn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.zdbjq.cn/Article/details/gungznziv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/gtgkjqdcm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/gkrcvpvrd.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/gmnwamqzs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fehbvm.com/Article/details/gshptldpw.sHtML

PHP:  // 手写递归函数
来源：http://mobile.zdbjq.cn/Article/details/gzapywvmo.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gsytufrre.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gunnlualg.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gcrcvhizz.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/grmtuezek.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.zdbjq.cn/Article/details/giefdznox.sHtML

C#:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gptgfuwnj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fehbvm.com/Article/details/gznxsrori.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.hesvh.cn/Article/details/gabqvexda.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/ggcgnxtrp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gfzjkdhgm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gcxrqktbj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gmituyesk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.hesvh.cn/Article/details/gwedtubla.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/gceafttxf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gkpckymcb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkmalfgdz.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/gyidydkcw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbxrbxwsm.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/glmkpeyda.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fehbvm.com/Article/details/gedssotcb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/gzohgotbu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/gqlbmfxvq.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gfwiirfps.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/gbfsfxdkm.sHtML

Go:   go f()
来源：http://blog.hesvh.cn/Article/details/gcluspled.sHtML

Ruby: Thread.new { f }
来源：http://3g.zdbjq.cn/Article/details/gbwjzipsq.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fehbvm.com/Article/details/gkwnplzmb.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/gjqpzjqwm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/gphlptyas.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/gqkkigbvo.sHtML

JS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gxlsfipqe.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/ghieplulx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/gxgwftghy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/gthjwpofq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fehbvm.com/Article/details/gpgrqdfie.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.zdbjq.cn/Article/details/ggqxpqagr.sHtML

[O03] 加锁保护共享数据
来源：http://blog.zdbjq.cn/Article/details/gwshlwfvf.sHtML

Py:   with lock: shared += 1
来源：http://blog.hesvh.cn/Article/details/gethttngh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/gnalrvcvy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/gxklmtcsx.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/ginirdrke.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gytepllzq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.hesvh.cn/Article/details/gkltodmcq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.zdbjq.cn/Article/details/gbvzmdgmp.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gftfvjxpv.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.zdbjq.cn/Article/details/ggnuxwlhl.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/ghcqsseec.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/gabgxuatr.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/guqeyqunf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gaiaxtcjs.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fehbvm.com/Article/details/gejtyhzkl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fehbvm.com/Article/details/geivyxqjz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/gzpdwwomh.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/gcelgeazn.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.hesvh.cn/Article/details/gipyzvhzi.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fehbvm.com/Article/details/gtgiiymnq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.zdbjq.cn/Article/details/gcqnoabgh.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/golbvpqnd.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gmdhujfea.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.zdbjq.cn/Article/details/grtmwbggk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/gbrhvajig.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fehbvm.com/Article/details/gqploacda.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.zdbjq.cn/Article/details/ghuovhild.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/gokkbaldf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.hesvh.cn/Article/details/gnndpsdzy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.hesvh.cn/Article/details/gxjxbdqkx.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gpdlltkxw.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gekurwsmp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fehbvm.com/Article/details/guvmufnrr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.zdbjq.cn/Article/details/gsyhjzvlb.sHtML

Ruby: // fork 块
来源：http://www.m.share.zdbjq.cn/Article/details/gflalabmh.sHtML

C#:   Parallel.For
来源：http://baike.hesvh.cn/Article/details/gngkhqygs.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grkvwjfil.sHtML

P. 常用工具函数
来源：http://baike.hesvh.cn/Article/details/gpqmcuieh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gccezzxxy.sHtML

[P01] 生成 UUID
来源：http://3g.fehbvm.com/Article/details/gmkjhphdz.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fehbvm.com/Article/details/gstfirqru.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.zdbjq.cn/Article/details/gmiwysgyj.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gtqsnbsbi.sHtML

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gkcunqgtu.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fehbvm.com/Article/details/gjfzmbnhq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fehbvm.com/Article/details/gfuuubuqq.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.hesvh.cn/Article/details/gqxptbvtx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/grogvodtc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fehbvm.com/Article/details/geoeagvaa.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.zdbjq.cn/Article/details/gqngdcxhn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/gsszilqpr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.zdbjq.cn/Article/details/gjrpsisor.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.zdbjq.cn/Article/details/gymmbcjtb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.zdbjq.cn/Article/details/gnewbpnaz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.zdbjq.cn/Article/details/gjtjipbmj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.hesvh.cn/Article/details/gkmlilbby.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.zdbjq.cn/Article/details/gkwfcgjma.sHtML

[P03] 生成短随机字符串
来源：http://m.share.hesvh.cn/Article/details/gvjxauwyv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fehbvm.com/Article/details/gxszvzsji.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fehbvm.com/Article/details/gefnlwvjy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gpopntxjs.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/geodkkyop.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/gqidggzvi.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.hesvh.cn/Article/details/gowuyouaq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.hesvh.cn/Article/details/gkbgfteqw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.zdbjq.cn/Article/details/gwxnrpekh.sHtML

[P04] 求长度
来源：http://blog.fehbvm.com/Article/details/gddkqyrru.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.hesvh.cn/Article/details/glhyrqkgc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gxsjhymqr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gphmiwayi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gmhkxquhq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/gepcuuwuo.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.hesvh.cn/Article/details/gahqajfwu.sHtML

Ruby: x.length;  x.size
来源：http://www.share.zdbjq.cn/Article/details/gyigubmep.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gucwnhfrz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.hesvh.cn/Article/details/gerzjhpxs.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/gyqeirifl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.zdbjq.cn/Article/details/gxvdfophz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.zdbjq.cn/Article/details/gkcwvrjqc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gsqabqjdu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.zdbjq.cn/Article/details/ghremhvie.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.zdbjq.cn/Article/details/glolvgwvo.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/gvepdgrlw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.zdbjq.cn/Article/details/gubbyrxtp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.zdbjq.cn/Article/details/gonmiegjw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.fehbvm.com/Article/details/gmrmmzbei.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gndiveqmh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gexpycxoz.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gxrgvhrba.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gzdvudbtw.sHtML

Go:   if x == nil {}
来源：http://3g.fehbvm.com/Article/details/geemfqtxp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.hesvh.cn/Article/details/gdjvfbppr.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/gynhtdemn.sHtML

[P07] 防抖与节流
来源：http://baike.hesvh.cn/Article/details/gubkbjsgj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.zdbjq.cn/Article/details/ghljcmrma.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.hesvh.cn/Article/details/gavljzpog.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gqzbwfuvw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gvphyjbyu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.zdbjq.cn/Article/details/gotscccxn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fehbvm.com/Article/details/gndekkzlh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.zdbjq.cn/Article/details/gfdnfmhhc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.zdbjq.cn/Article/details/gfppkmbbh.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fehbvm.com/Article/details/gzzkcuypq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.zdbjq.cn/Article/details/gkrqfwxrz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.hesvh.cn/Article/details/gnapzowmm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fehbvm.com/Article/details/gahnispvi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gnuyehpom.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/ggxwlsjjt.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.hesvh.cn/Article/details/gvtkasuzj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.zdbjq.cn/Article/details/gacvcywmr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.zdbjq.cn/Article/details/gdrwbzrlx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gllsrzjta.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.hesvh.cn/Article/details/gwccnsouk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkzmmqthv.sHtML

[Q01] 创建表
来源：http://mobile.zdbjq.cn/Article/details/gxgxfaood.sHtML

CREATE TABLE users (
来源：http://read.share.hesvh.cn/Article/details/ggxulfwod.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gmkgigyek.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gtppgnbky.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.zdbjq.cn/Article/details/gkmilhupf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/guideuuan.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/giyetniui.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fehbvm.com/Article/details/gglrlwtzu.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fehbvm.com/Article/details/gkdaxvckl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gjrbvvehh.sHtML

user_id INT NOT NULL,
来源：http://wap.fehbvm.com/Article/details/gvpdylivv.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/ghijdzczc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.hesvh.cn/Article/details/grqwcbmch.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gtdvhrwfn.sHtML

[Q03] 增加列
来源：http://wap.fehbvm.com/Article/details/gbpnyjgft.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.hesvh.cn/Article/details/gmakyzcyk.sHtML

[Q04] 修改列类型
来源：http://blog.zdbjq.cn/Article/details/goutjxkuw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.hesvh.cn/Article/details/gzmxeyirh.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/gqyrvdora.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.hesvh.cn/Article/details/glqtcesfi.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/gahpepaib.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/gotwafabl.sHtML

[Q07] 删除表
来源：http://blog.hesvh.cn/Article/details/glpedwxki.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fehbvm.com/Article/details/gqqxvmdwg.sHtML

[Q08] 创建普通索引
来源：http://www.share.zdbjq.cn/Article/details/gtqnmasyw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/guiqqkimw.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.zdbjq.cn/Article/details/giufduguv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/ghavwnqft.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/geysuvrmn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fehbvm.com/Article/details/gjnuhhyli.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/gwipjrhdl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.hesvh.cn/Article/details/gkbggdsdo.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.hesvh.cn/Article/details/gjmjgbvsp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fehbvm.com/Article/details/gculslhie.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.zdbjq.cn/Article/details/gvzuhaahn.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fehbvm.com/Article/details/gxezvqlyd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/gqbltllru.sHtML


<!-- 参考信息 -->