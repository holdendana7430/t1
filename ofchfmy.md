代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fanxiaobao.xyz/Article/details/ghjtauvxr.sHtML

Ruby: warn "err"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxlmzvfd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fanxiaobao.xyz/Article/details/gtuchqzeg.sHtML

[M07] 判断是否为主入口
来源：http://baike.fanxiaobao.xyz/Article/details/gahqwheqn.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fanxiaobao.xyz/Article/details/gpstkymle.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fanxiaobao.xyz/Article/details/gngibbauz.sHtML

JS:   require.main === module
来源：http://wap.fanxiaobao.xyz/Article/details/gikiegomt.sHtML

TS:   require.main === module
来源：http://www.share.fanxiaobao.xyz/Article/details/gqunlqijq.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbyyfytn.sHtML

Go:   func main()
来源：http://mobile.fanxiaobao.xyz/Article/details/gokkqompo.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbfoscem.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fanxiaobao.xyz/Article/details/grmwscvwq.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.fanxiaobao.xyz/Article/details/gjcblebde.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fanxiaobao.xyz/Article/details/gcvxnnboy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihihawcw.sHtML

JS:   process.platform;  process.version
来源：http://blog.fanxiaobao.xyz/Article/details/gzyfcpiid.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdovynmf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fanxiaobao.xyz/Article/details/gzyuxwliq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fanxiaobao.xyz/Article/details/gixgmmszu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fanxiaobao.xyz/Article/details/gmtjmvfjx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgnmrirf.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gximdystp.sHtML

N. 数据结构与算法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvoiwqhry.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrgujtbr.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fanxiaobao.xyz/Article/details/gwpustkhc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpalujuyo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnoscble.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fanxiaobao.xyz/Article/details/gezoabwdu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fanxiaobao.xyz/Article/details/gnozorhca.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzngqpzhj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlrdmosh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqxsloeu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmrxgpkj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyovwzsb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fanxiaobao.xyz/Article/details/gxjaundip.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxxmvyte.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcknolkt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvvewzcx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdvqbnbp.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gtwzdueip.sHtML

Ruby: arr.sort
来源：http://m.share.fanxiaobao.xyz/Article/details/gugbiltzx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fanxiaobao.xyz/Article/details/geppuhsmu.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkxumyld.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fanxiaobao.xyz/Article/details/gxywwrbgb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fanxiaobao.xyz/Article/details/gqakhfwvx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fanxiaobao.xyz/Article/details/gzwsmonwm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfaeyjba.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxlxqgsa.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fanxiaobao.xyz/Article/details/gnobjlqki.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fanxiaobao.xyz/Article/details/gcwgxmkui.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fanxiaobao.xyz/Article/details/gaftnimvj.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fanxiaobao.xyz/Article/details/garpjchia.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcgdzxwi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fanxiaobao.xyz/Article/details/gdmioirgk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyysnybya.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fanxiaobao.xyz/Article/details/grfhfdywi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsaahjlt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fanxiaobao.xyz/Article/details/gydmbvcrb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gxvxhrrib.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fanxiaobao.xyz/Article/details/ghpldrhst.sHtML

[N05] 最大公约数
来源：http://blog.fanxiaobao.xyz/Article/details/gwiicdvox.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fanxiaobao.xyz/Article/details/glwsaqprf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fanxiaobao.xyz/Article/details/glazsgfkd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fanxiaobao.xyz/Article/details/gcbjyudcp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakmaeblo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gneiohkcu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpskkfprw.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gloiclbgh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fanxiaobao.xyz/Article/details/gykgycwmq.sHtML

[N06] 判断回文字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqebhvvs.sHtML

Py:   s == s[::-1]
来源：http://www.share.fanxiaobao.xyz/Article/details/grbpgjdyc.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fanxiaobao.xyz/Article/details/gdjflbxyh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fanxiaobao.xyz/Article/details/gdkhfelov.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnrowhbp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdwhjycs.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fanxiaobao.xyz/Article/details/geqztujhz.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrbiovnj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngkpxano.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilwbvczj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fanxiaobao.xyz/Article/details/gnghzpivb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgrbgllj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fanxiaobao.xyz/Article/details/grvejqkxs.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fanxiaobao.xyz/Article/details/goljqfbzb.sHtML

Java: // 手写 HashMap
来源：http://read.share.fanxiaobao.xyz/Article/details/gycstzrsb.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvksynbvg.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrlpxfcj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrjwgntv.sHtML

[N08] 生成全排列
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqzikltq.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gerhjmjqw.sHtML

PHP:  // 手写递归交换
来源：http://3g.fanxiaobao.xyz/Article/details/gsvgtfapo.sHtML

JS:   // 手写回溯递归
来源：http://blog.fanxiaobao.xyz/Article/details/gvkdubgyu.sHtML

TS:   // 手写回溯递归
来源：http://blog.fanxiaobao.xyz/Article/details/gjpkoioli.sHtML

Java: // 手写回溯递归
来源：http://baike.fanxiaobao.xyz/Article/details/gkjzwzodb.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtmwwaiv.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmvrpkez.sHtML

C#:   // 手写回溯递归
来源：http://baike.fanxiaobao.xyz/Article/details/gkioiwgpe.sHtML

[N09] 栈与队列
来源：http://wap.fanxiaobao.xyz/Article/details/gprfpgthx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrunwaki.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkozpxkb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fanxiaobao.xyz/Article/details/gexmzyprh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwpzfqve.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gofuvfxxs.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fanxiaobao.xyz/Article/details/gbyhquizr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fanxiaobao.xyz/Article/details/glotadcld.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fanxiaobao.xyz/Article/details/glxfpchsl.sHtML

[N10] 链表节点定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhynnsmy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fanxiaobao.xyz/Article/details/gteabiegy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmgigjia.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gewebiqdx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgweqcmr.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkuxfjpwt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqtvatmd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fanxiaobao.xyz/Article/details/gfclecjmf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptwzbigl.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcgsimir.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fanxiaobao.xyz/Article/details/gijybtlno.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/greyrtoel.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fanxiaobao.xyz/Article/details/gzndcjdqu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fanxiaobao.xyz/Article/details/gmvrrlrpz.sHtML

Java: // 手写递归
来源：http://wap.fanxiaobao.xyz/Article/details/giymmujbp.sHtML

Go:   // 手写递归
来源：http://www.share.fanxiaobao.xyz/Article/details/glwptoarb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlgsvhav.sHtML

C#:   // 手写递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitzvglof.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzjstuih.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fanxiaobao.xyz/Article/details/gqryisvcm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsgwgnik.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fanxiaobao.xyz/Article/details/gdguapjjx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fanxiaobao.xyz/Article/details/gocscjoqg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fanxiaobao.xyz/Article/details/glxxjhkjf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnnpeqvl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gefseurfq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gnppimjip.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdeuqxljr.sHtML

O. 并发与异步
来源：http://3g.fanxiaobao.xyz/Article/details/gaybnzhtz.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gdliimkhr.sHtML

[O01] 启动一个线程
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggifuatxj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtmkkjwo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhgwmcwk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecvjjzva.sHtML

TS:   // 同 JS
来源：http://3g.fanxiaobao.xyz/Article/details/gitljwzsm.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrvgqxmn.sHtML

Go:   go f()
来源：http://m.share.fanxiaobao.xyz/Article/details/graqmzyxa.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fanxiaobao.xyz/Article/details/gufcwfwsk.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fanxiaobao.xyz/Article/details/glppkebsb.sHtML

[O02] 使用线程池
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goglaribv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fanxiaobao.xyz/Article/details/ggtunuzts.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fanxiaobao.xyz/Article/details/gatdxbebe.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fanxiaobao.xyz/Article/details/gfvsgdyxo.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fanxiaobao.xyz/Article/details/gykkzdnyt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gtgvnbfaa.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjdtlanw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclzdixln.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdjckapw.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fanxiaobao.xyz/Article/details/gilkykqrk.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fanxiaobao.xyz/Article/details/guimpjvjd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fanxiaobao.xyz/Article/details/gqaxbtotc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fanxiaobao.xyz/Article/details/gkynnujte.sHtML

TS:   // 同 JS
来源：http://blog.fanxiaobao.xyz/Article/details/gphapwpcd.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fanxiaobao.xyz/Article/details/gyjtyhnjq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fanxiaobao.xyz/Article/details/grtdegkef.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkprjelpl.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnnimhdbw.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gnfgultas.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdhlowlc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fanxiaobao.xyz/Article/details/gxruapdpo.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gwrqilrzk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gsulkfxtw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fanxiaobao.xyz/Article/details/gampwediy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fanxiaobao.xyz/Article/details/gjkrsayrc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkcnzjip.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnmtmjei.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fanxiaobao.xyz/Article/details/guctbiaac.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsgqiuuu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fanxiaobao.xyz/Article/details/gkigrtcwm.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvcjedyh.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fanxiaobao.xyz/Article/details/gqsvupzqf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fanxiaobao.xyz/Article/details/giqpomupx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fanxiaobao.xyz/Article/details/gysbkshre.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fanxiaobao.xyz/Article/details/gmyyuxoaa.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcvguvan.sHtML

[O06] 使用进程池
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqgocucg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkcjdwtx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmnmqxjt.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvcuzgwh.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwlnasll.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fanxiaobao.xyz/Article/details/gkpcpjmmi.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fanxiaobao.xyz/Article/details/gzvtvanqh.sHtML

Ruby: // fork 块
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvznrjct.sHtML

C#:   Parallel.For
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkxsqefc.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gynmdfhsw.sHtML

P. 常用工具函数
来源：http://3g.fanxiaobao.xyz/Article/details/gckesjvut.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gzningodh.sHtML

[P01] 生成 UUID
来源：http://www.share.fanxiaobao.xyz/Article/details/gdaknmllx.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fanxiaobao.xyz/Article/details/gysnsbndz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzejjmed.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fanxiaobao.xyz/Article/details/gnkvfmpqa.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fanxiaobao.xyz/Article/details/gcdmhifao.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fanxiaobao.xyz/Article/details/grxxidffy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqbxqumo.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdqqmkgd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fanxiaobao.xyz/Article/details/gvagtndkd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxakamjp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbpcplwf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.fanxiaobao.xyz/Article/details/gehxnrwaj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fanxiaobao.xyz/Article/details/ggsoozhye.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fanxiaobao.xyz/Article/details/gicaowpsy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjimqwkbz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxgvruvr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgdcrwlj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvshlgvgo.sHtML

[P03] 生成短随机字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gbigdkzgb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fanxiaobao.xyz/Article/details/gkekepwye.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxopirrur.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyulzyox.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjrabkyn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fanxiaobao.xyz/Article/details/gpfyqmyeh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fanxiaobao.xyz/Article/details/gdinzluzz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fanxiaobao.xyz/Article/details/gmuneqwmz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fanxiaobao.xyz/Article/details/gubpymxkm.sHtML

[P04] 求长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gutkmibkq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fanxiaobao.xyz/Article/details/gyaelhdto.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fanxiaobao.xyz/Article/details/gxngxizde.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukgvkujy.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fanxiaobao.xyz/Article/details/ghsvwyauz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fanxiaobao.xyz/Article/details/gmqjrgrpr.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfiexmsmr.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpybuiieg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqyxtohk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpxwiyzn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fanxiaobao.xyz/Article/details/gzxcqiebv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfmvkywh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fanxiaobao.xyz/Article/details/goyklherb.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsyisvui.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwioaueo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrrxbzbq.sHtML

Ruby: a == b
来源：http://m.share.fanxiaobao.xyz/Article/details/grhqrjdth.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fanxiaobao.xyz/Article/details/gpvubqwti.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxbxczxs.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fanxiaobao.xyz/Article/details/gvyenlerm.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/giqtfnhnf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fanxiaobao.xyz/Article/details/gyuumfimx.sHtML

TS:   if (x == null) {}
来源：http://3g.fanxiaobao.xyz/Article/details/glsaawwfn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gwfqiadsc.sHtML

Go:   if x == nil {}
来源：http://baike.fanxiaobao.xyz/Article/details/gjygevmxg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fanxiaobao.xyz/Article/details/gqaqgugdy.sHtML

C#:   if (x is null) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gzyimuabc.sHtML

[P07] 防抖与节流
来源：http://baike.fanxiaobao.xyz/Article/details/gosgqttaw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbxusjcg.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtodkysd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwpwggjj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gpahngywr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqhqpnee.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fanxiaobao.xyz/Article/details/gqevlmmil.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fanxiaobao.xyz/Article/details/gdtmvvrdv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fanxiaobao.xyz/Article/details/glhtsppbx.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fanxiaobao.xyz/Article/details/glzaqqczs.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfclyejbc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghixjwckq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fanxiaobao.xyz/Article/details/gcrzyuqmj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fanxiaobao.xyz/Article/details/gzifvlgsh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.fanxiaobao.xyz/Article/details/gsgaweuhs.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fanxiaobao.xyz/Article/details/gndnshhow.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxbbylvu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fanxiaobao.xyz/Article/details/gyvrdetkf.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/grovrbdzo.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbptqgcw.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvssqdwug.sHtML

[Q01] 创建表
来源：http://baike.fanxiaobao.xyz/Article/details/grqcztefv.sHtML

CREATE TABLE users (
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdxygaok.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fanxiaobao.xyz/Article/details/gzxeymepr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhuittkn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fanxiaobao.xyz/Article/details/gmkxydpaa.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fanxiaobao.xyz/Article/details/gqkkdizva.sHtML

);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmypueen.sHtML

[Q02] 创建带外键的表
来源：http://3g.fanxiaobao.xyz/Article/details/gyovcwgmp.sHtML

CREATE TABLE orders (
来源：http://baike.fanxiaobao.xyz/Article/details/glncuwyxu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fanxiaobao.xyz/Article/details/gpoxdrgnk.sHtML

user_id INT NOT NULL,
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxaqxape.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fanxiaobao.xyz/Article/details/gpjbjwpxg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fanxiaobao.xyz/Article/details/gdlyvafqn.sHtML

);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtylrtcc.sHtML

[Q03] 增加列
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbehovke.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gamgjdqct.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsdosekx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fanxiaobao.xyz/Article/details/gyexdppnh.sHtML

[Q05] 重命名列
来源：http://blog.fanxiaobao.xyz/Article/details/gnrseuses.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fanxiaobao.xyz/Article/details/gtgbpgvnk.sHtML

[Q06] 删除列
来源：http://mobile.fanxiaobao.xyz/Article/details/gkobkzrqv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgvtffwl.sHtML

[Q07] 删除表
来源：http://m.share.fanxiaobao.xyz/Article/details/gswreytez.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecgdfbaa.sHtML

[Q08] 创建普通索引
来源：http://wap.fanxiaobao.xyz/Article/details/gctuizcss.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fanxiaobao.xyz/Article/details/goszvfeoh.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryvluivi.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fanxiaobao.xyz/Article/details/gytccdqut.sHtML

[Q10] 插入单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmghnsuhm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/gxihpyosp.sHtML

[Q11] 一次插入多行
来源：http://wap.fanxiaobao.xyz/Article/details/gkazlesws.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxqqpydz.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmnujmjf.sHtML


<!-- 参考信息 -->