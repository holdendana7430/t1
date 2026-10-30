代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/gicnlaqfo.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/gqdfdjtvn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fehbvm.com/Article/details/gvdzmulqi.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/gqkmvhswj.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/gdauizudg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fehbvm.com/Article/details/gnvvukbtc.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gskmcbzqk.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gfemnwsxn.sHtML

Java: public static void main(String[] args)
来源：http://blog.fehbvm.com/Article/details/gqvrktxqm.sHtML

Go:   func main()
来源：http://mobile.hesvh.cn/Article/details/gwqceplta.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.hesvh.cn/Article/details/gnbcvlcoh.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/gmlyxxqcw.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.zdbjq.cn/Article/details/gkcubyrsa.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fehbvm.com/Article/details/gvhkmaapp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.zdbjq.cn/Article/details/grttueorm.sHtML

JS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gbxfyhsza.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gafnksxyk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/geaisdjfu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fehbvm.com/Article/details/gdxkjxwfz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/glrplwfxa.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/geitqldlz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gaopigbyv.sHtML

N. 数据结构与算法
来源：http://www.share.fehbvm.com/Article/details/govoxptbs.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gyohptggu.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/gyfsbtkfa.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gqjdsxanq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gseyjotfs.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/glnfrpsqt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gxvuzfszb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gdwrekorl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gfkmgkskc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fehbvm.com/Article/details/gvvlacigx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gtweldnob.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/gpgmwosvv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gwpaccwli.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/grugizhfd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gdsgdinzs.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/glzslcdex.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.zdbjq.cn/Article/details/gmtnheysy.sHtML

Go:   slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gnxdxykxn.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gwcncedlh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.zdbjq.cn/Article/details/gcnhbfulg.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/gbuoqskxb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fehbvm.com/Article/details/gjdlsvgpt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/gojzctnmf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gplrhcwvn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/giejjozyn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/gujinrryj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/gdyzbxawm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fehbvm.com/Article/details/gwtfabllt.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fehbvm.com/Article/details/gdqvsovop.sHtML

[N04] 斐波那契数列
来源：http://blog.zdbjq.cn/Article/details/gohkiwjtp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gpkxaqyaw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/giqnszqmr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/grrkzfwsn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gppjhqbmu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.zdbjq.cn/Article/details/garhszkri.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fehbvm.com/Article/details/gqkgccodq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gsmqghzqq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gyrlgansn.sHtML

[N05] 最大公约数
来源：http://blog.zdbjq.cn/Article/details/gxrzhywzs.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/ghgfkylko.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/ginjvgwko.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gkcplpjid.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/grqaputsx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.hesvh.cn/Article/details/gigjqrxvr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gxegpskxp.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/gjyeyuurz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/gxcdiqbio.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/gjxlbsvro.sHtML

Py:   s == s[::-1]
来源：http://baike.hesvh.cn/Article/details/gjyvvkkxj.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gyksytctc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gmmxttrhm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gaibpyots.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/gzcwidkcp.sHtML

Go:   // 双指针从两端比较
来源：http://baike.hesvh.cn/Article/details/gydctcnom.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gukexkhpv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gtqykoosx.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/gshgpirsm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.fehbvm.com/Article/details/gynccxqkn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.hesvh.cn/Article/details/ghxesgjps.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.hesvh.cn/Article/details/gvemfkbkr.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.zdbjq.cn/Article/details/gjuyzfxzu.sHtML

Java: // 手写 HashMap
来源：http://baike.fehbvm.com/Article/details/giumfenfo.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.hesvh.cn/Article/details/gbvlhvrqf.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.hesvh.cn/Article/details/gaqmanumr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fehbvm.com/Article/details/gopjwvbjm.sHtML

[N08] 生成全排列
来源：http://baike.fehbvm.com/Article/details/gtjyvkzxp.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/gbdtztlts.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/gxnrnrbss.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gxmvsurzm.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gsbqcuell.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gjmgsruvj.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gcoxjhfyi.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fehbvm.com/Article/details/gymxunscm.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gitgfgwzl.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/geoaalqai.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.hesvh.cn/Article/details/gkgsekgtx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gctilglps.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/geiknhicp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gbethamzi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/gjwwmhous.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/gtkjzwnzh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gxcdrnkyv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.fehbvm.com/Article/details/gcxfprumu.sHtML

[N10] 链表节点定义
来源：http://www.share.zdbjq.cn/Article/details/gwveobvlj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.zdbjq.cn/Article/details/ggbwpcdga.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbermfinp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.hesvh.cn/Article/details/gdccyaxnr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/geljvvure.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.zdbjq.cn/Article/details/gbwtmacbl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gwghjlwbn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/gikjalcwk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.hesvh.cn/Article/details/gxninylpm.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gihijfxtv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/gwnfkkmlr.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/gyciteqhk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gaomruxah.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gkimwirdn.sHtML

Java: // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gdcwqjcfc.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gbmfextxy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/gccgscurd.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gnmzxgxfc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/gengwdyrn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.hesvh.cn/Article/details/gsjnatdry.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/gkkwjhgzp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gilxjctuo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gplhkmuwq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gkqxfodtu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/gpiilqswj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fehbvm.com/Article/details/gqmrxkqrr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gcbpjdpor.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gpvwttfls.sHtML

O. 并发与异步
来源：http://www.m.share.zdbjq.cn/Article/details/glebibodh.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbibzhbhi.sHtML

[O01] 启动一个线程
来源：http://mobile.hesvh.cn/Article/details/gmwyaedsj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.zdbjq.cn/Article/details/gnolwbvwq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gwhsyxubl.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/gnyvonqhx.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gzltztkbn.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/gkaxwzgkf.sHtML

Go:   go f()
来源：http://wap.fehbvm.com/Article/details/gvdovbcaw.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.hesvh.cn/Article/details/gnvqunakf.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fehbvm.com/Article/details/gkcjqzagw.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/gylfyssvp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/gvtwrzsnv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fehbvm.com/Article/details/gettowjtu.sHtML

JS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gvvnraloq.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gceytaaeb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.hesvh.cn/Article/details/gzqlberfc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/gbjbjqpsj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.zdbjq.cn/Article/details/gwzvuvuzl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fehbvm.com/Article/details/gdkqoqxuh.sHtML

[O03] 加锁保护共享数据
来源：http://wap.hesvh.cn/Article/details/gnxltmfnp.sHtML

Py:   with lock: shared += 1
来源：http://3g.fehbvm.com/Article/details/getzbgwsv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fehbvm.com/Article/details/gfxglmipl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/ghrbajjpn.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gufedanfi.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gtskgaroe.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/gzestvdlp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/gffksdhlh.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gvauzlhll.sHtML

[O04] 定义异步函数并等待
来源：http://3g.zdbjq.cn/Article/details/glvkxvpgx.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.zdbjq.cn/Article/details/grxgqjvmf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/gicmkhwsb.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gfwdboleo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gpassxbti.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.zdbjq.cn/Article/details/ggraamujd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fehbvm.com/Article/details/gjonkocga.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/ggqbvquhl.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/gglqyvisf.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.zdbjq.cn/Article/details/gmxlqzsqp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fehbvm.com/Article/details/ghbvwxxvv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/gdsevcsfj.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gcshdxgsw.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/ghsqkqeog.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/glzivvugj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.hesvh.cn/Article/details/gjtprlzet.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gcdvqreuq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.hesvh.cn/Article/details/gtrctyxsc.sHtML

[O06] 使用进程池
来源：http://www.blog.fehbvm.com/Article/details/glrtdsquh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.zdbjq.cn/Article/details/grgaxcekd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fehbvm.com/Article/details/gvsnyhygp.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gszoapaab.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gyvqfmkme.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gxoiaeuzz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/giclqvpel.sHtML

Ruby: // fork 块
来源：http://wap.fehbvm.com/Article/details/gnzvizgwq.sHtML

C#:   Parallel.For
来源：http://baike.zdbjq.cn/Article/details/gjzilkoix.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gszvdygao.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/gtkvzetvs.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzqcifthl.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gzutjbeui.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/gxowitalt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.zdbjq.cn/Article/details/gllzowvab.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gzbjgasqk.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gxeujaoll.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.hesvh.cn/Article/details/gmteoeldd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.hesvh.cn/Article/details/gnmyklabn.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fehbvm.com/Article/details/gvlmxspfz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/grmamjdkh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.zdbjq.cn/Article/details/gwscgprjt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.zdbjq.cn/Article/details/gbczjldbi.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.zdbjq.cn/Article/details/gjgztcohb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.zdbjq.cn/Article/details/gonopizbz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.zdbjq.cn/Article/details/gtqybftmc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.zdbjq.cn/Article/details/gndoteatj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.zdbjq.cn/Article/details/gdgzwaagx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fehbvm.com/Article/details/gzgdwbsmo.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/gqjfumiyy.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fehbvm.com/Article/details/getvatzoq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fehbvm.com/Article/details/gdnzzczbf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/gkrsdohzk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gypirwtlg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gljvioaty.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/getekpqbi.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fehbvm.com/Article/details/gjkdikiya.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/gujtpqqsv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/gfhhnfkfu.sHtML

[P04] 求长度
来源：http://www.m.share.hesvh.cn/Article/details/glwesgrbw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gqnjzwuzz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gsznfptcp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gxeecgurx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gntsluvbg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fehbvm.com/Article/details/gxkkuswrl.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.hesvh.cn/Article/details/gawdhhriv.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fehbvm.com/Article/details/goeoyppad.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gtmfcbuid.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gzrghsghx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.hesvh.cn/Article/details/gocervrqr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fehbvm.com/Article/details/gjnzieykm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fehbvm.com/Article/details/gcocnildk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gtgzesktf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/gcawjwjsq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fehbvm.com/Article/details/gfbbrebbh.sHtML

Ruby: a == b
来源：http://mobile.fehbvm.com/Article/details/gegzcpkkj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.zdbjq.cn/Article/details/guyqwqplv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fehbvm.com/Article/details/gaemzxiud.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.hesvh.cn/Article/details/ghjqrougd.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/gccbvnuuc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fehbvm.com/Article/details/gmoavjncc.sHtML

TS:   if (x == null) {}
来源：http://www.blog.hesvh.cn/Article/details/glasggvea.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gcvrdonaw.sHtML

Go:   if x == nil {}
来源：http://www.m.share.hesvh.cn/Article/details/gwjrchulx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.zdbjq.cn/Article/details/gwtlpwupx.sHtML

C#:   if (x is null) {}
来源：http://read.share.hesvh.cn/Article/details/gerlzaxbt.sHtML

[P07] 防抖与节流
来源：http://www.m.share.fehbvm.com/Article/details/grptvtdta.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/gnahdamhv.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fehbvm.com/Article/details/gztiaoovl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gbvpwhpjx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gwjpmjsxw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.hesvh.cn/Article/details/gvhukjjyd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/gmequlztu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.zdbjq.cn/Article/details/gorfzvpca.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fehbvm.com/Article/details/gcwbzlqrb.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fehbvm.com/Article/details/gdmhdnkpd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/gayxguzvk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fehbvm.com/Article/details/gzmkgpmjd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.zdbjq.cn/Article/details/gerhgsdyr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/ghpincrop.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fehbvm.com/Article/details/gnfkerwyc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.zdbjq.cn/Article/details/gjxvlhqvh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.hesvh.cn/Article/details/gddrtkmob.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.zdbjq.cn/Article/details/gegwldfsd.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdylpelie.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.zdbjq.cn/Article/details/gsihpfuen.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggejlzqui.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/gqqeqjudm.sHtML

CREATE TABLE users (
来源：http://wap.hesvh.cn/Article/details/gyionyicr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/ghxouwejp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gahjbhxlu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/gbdoqiggq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/glaionxpf.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gfqmubpvx.sHtML

[Q02] 创建带外键的表
来源：http://blog.zdbjq.cn/Article/details/gpmiqtzck.sHtML

CREATE TABLE orders (
来源：http://read.share.fehbvm.com/Article/details/giltxuczu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gdicawqgq.sHtML

user_id INT NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gogdccuge.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.zdbjq.cn/Article/details/gslhngwiy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.zdbjq.cn/Article/details/gyvynvieg.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gojegczli.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/gkrrikugj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fehbvm.com/Article/details/gqxazpdmq.sHtML

[Q04] 修改列类型
来源：http://wap.hesvh.cn/Article/details/gwtrvftzg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fehbvm.com/Article/details/gvpytzraa.sHtML

[Q05] 重命名列
来源：http://wap.hesvh.cn/Article/details/gjkgrkbrg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.zdbjq.cn/Article/details/gqfzsbsuw.sHtML

[Q06] 删除列
来源：http://m.share.hesvh.cn/Article/details/ghcipyfmd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/gzzjfvzbi.sHtML

[Q07] 删除表
来源：http://3g.zdbjq.cn/Article/details/gamcisusi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fehbvm.com/Article/details/geqdquvdv.sHtML

[Q08] 创建普通索引
来源：http://wap.fehbvm.com/Article/details/gnosyfach.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gecisdnhn.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.hesvh.cn/Article/details/gcbgupofl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gfobuzrdy.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/gujsjnjcw.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gnopmpvfh.sHtML

[Q11] 一次插入多行
来源：http://blog.fehbvm.com/Article/details/gaeiuzrpf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fehbvm.com/Article/details/gbvmrugia.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.hesvh.cn/Article/details/geictlzlr.sHtML


<!-- 参考信息 -->