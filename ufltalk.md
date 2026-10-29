代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.hesvh.cn/Article/details/gntrghkkf.sHtML

JS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gajxeklly.sHtML

TS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gcrwpjdfb.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/grpuwdnet.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fehbvm.com/Article/details/gzenmjynp.sHtML

Ruby: warn "err"
来源：http://m.share.zdbjq.cn/Article/details/gkrwcesem.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.hesvh.cn/Article/details/gsrfhzaks.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/goxwrljyu.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/gyjqhdfax.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.zdbjq.cn/Article/details/gnegjeesn.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gphehnpeg.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gloerkjqf.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gernzstye.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/ghkvyzhdq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.zdbjq.cn/Article/details/gipscwnsv.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/gwwkssfxa.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.zdbjq.cn/Article/details/gvvvpahcj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/gonwaslrz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.zdbjq.cn/Article/details/gikxjqkzf.sHtML

JS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/guxtkwubp.sHtML

TS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gxotwtwsj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/ggfdbjxvo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/gdpcdbtaa.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/gtxrnebxp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/goranbmpo.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvfiinnlr.sHtML

N. 数据结构与算法
来源：http://m.share.fehbvm.com/Article/details/gzchjyuzq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqnrpebhc.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.zdbjq.cn/Article/details/gwdxjivfk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gyvgjemsr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.hesvh.cn/Article/details/gajzqqlct.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/ghrzgmenq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gglghteqn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gpmuaahmn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gyduszuch.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/gofmxvbno.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gyqweniup.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/grghppdcx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gubzjsllw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fehbvm.com/Article/details/giileysxw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gpeuuvhnb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gpvsacdku.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/ghkxxpnjw.sHtML

Go:   slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gkagdbqdx.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gupkqlktu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.hesvh.cn/Article/details/gtfpvuiwo.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.zdbjq.cn/Article/details/gtywswfbz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/gavxofflc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/gpdrafbsh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gfbsdbotn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/glurtsxyg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fehbvm.com/Article/details/ggwmiqayp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gedidikmi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/gfszixhdx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.hesvh.cn/Article/details/gfgqrkbtx.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/gpwgjhots.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gmyibyvtk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/glzdhjeoz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gicvcbwgz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gyatkruib.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gjiteiecy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.hesvh.cn/Article/details/gwferbura.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/giuxacpjc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/glnciesrh.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/gfvdnltie.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gfpkpqnmk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/gklzmhxrt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gdxyibrus.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gygwlxgec.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fehbvm.com/Article/details/grbwqxhya.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/gnlwjqscz.sHtML

Ruby: a.gcd(b)
来源：http://3g.zdbjq.cn/Article/details/gvfvsobdg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/ggppcdewu.sHtML

[N06] 判断回文字符串
来源：http://read.share.hesvh.cn/Article/details/gbuioxmpb.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gevtqrlcb.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gjzkcadkq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gidjcaiig.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/glmhmvzcj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.zdbjq.cn/Article/details/gmsfwndyc.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/gopwvafup.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gjgkhczbw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/grhvlvpfp.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/gbszylvut.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/gyqamjoxi.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.hesvh.cn/Article/details/gegsjmrna.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/gexogaqyz.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fehbvm.com/Article/details/gbctxlzni.sHtML

Java: // 手写 HashMap
来源：http://www.share.fehbvm.com/Article/details/giihjheuw.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/gzsjbocjc.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gqxsbssot.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fehbvm.com/Article/details/gammelnbs.sHtML

[N08] 生成全排列
来源：http://m.share.fehbvm.com/Article/details/gbrqnaljw.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.zdbjq.cn/Article/details/gfzwdgmwi.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.hesvh.cn/Article/details/grwecnpeg.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gughqmmbo.sHtML

TS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gfayratka.sHtML

Java: // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gonbkzbyv.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gchcrwwtg.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.hesvh.cn/Article/details/gwpjmgbtv.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gcfqmmdfp.sHtML

[N09] 栈与队列
来源：http://wap.fehbvm.com/Article/details/griddgvfc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/gcigesauw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gvtyzqqzm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gaacoipuz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fehbvm.com/Article/details/gctynjlsc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.hesvh.cn/Article/details/getlhscnj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fehbvm.com/Article/details/gryfechal.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gpxrshhtv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.zdbjq.cn/Article/details/gxqlykgpv.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/gtehovahe.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.zdbjq.cn/Article/details/gmzesezrg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.hesvh.cn/Article/details/gedmsmzpw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fehbvm.com/Article/details/gnaliouya.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/ggfaggwcr.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.zdbjq.cn/Article/details/gjayibljq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/gvlwsyyjs.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/girlgwhgu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fehbvm.com/Article/details/gdsuwnvyb.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/gwmlcamsd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.zdbjq.cn/Article/details/gmcxlvkgd.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fehbvm.com/Article/details/gsqvuchoz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gkgtiilzh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/grnnoinyx.sHtML

Java: // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gfgpqitby.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gapuvpris.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.hesvh.cn/Article/details/gnfitmfvx.sHtML

C#:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gevqqlquk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.zdbjq.cn/Article/details/gpqrhmxiy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fehbvm.com/Article/details/guomynuvm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/gfigkimlf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gjglowoyh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/ghcgjrwta.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gfvcgnfdn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.zdbjq.cn/Article/details/ghxtpslos.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/gtyjnpkor.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gddmomdav.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gffnowklo.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/gdhszgjdt.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gkmxolnhu.sHtML

[O01] 启动一个线程
来源：http://www.blog.fehbvm.com/Article/details/gtebcylec.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.hesvh.cn/Article/details/ggxvjlbvv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/glkotcvhs.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.hesvh.cn/Article/details/gwelosjox.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gzfhzpdpo.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.zdbjq.cn/Article/details/gpmmzoqot.sHtML

Go:   go f()
来源：http://blog.hesvh.cn/Article/details/gfpihbbyh.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/gneqreqcd.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fehbvm.com/Article/details/gcbbjdawi.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/ggorlmnfy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fehbvm.com/Article/details/gzxdqrucq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/gyrigsczj.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/glnuhmzge.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gzdihbwxg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fehbvm.com/Article/details/guxomnpqq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fehbvm.com/Article/details/gzzkffhde.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.zdbjq.cn/Article/details/gsshsuedk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fehbvm.com/Article/details/gwecqclqz.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fehbvm.com/Article/details/gbipwaexs.sHtML

Py:   with lock: shared += 1
来源：http://3g.fehbvm.com/Article/details/gvgxgnuif.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/gpdcvtlkb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.zdbjq.cn/Article/details/gghcocshs.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/glxmpjvah.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gxzuxrois.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.hesvh.cn/Article/details/gnfemsvgt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.zdbjq.cn/Article/details/gywuimyiu.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gylynbaye.sHtML

[O04] 定义异步函数并等待
来源：http://wap.hesvh.cn/Article/details/gwgfvjyfi.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/gdoisqysu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.zdbjq.cn/Article/details/geokoobnc.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gehdntwpn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/glfacugra.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/gqoqyudqy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.hesvh.cn/Article/details/gcqzrtoar.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.zdbjq.cn/Article/details/gucjikmpg.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.zdbjq.cn/Article/details/gwmvxphaa.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.zdbjq.cn/Article/details/gmggmywso.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fehbvm.com/Article/details/gjxmuljag.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.zdbjq.cn/Article/details/gkdnisfob.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/ghzykfuvm.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gvkxfzotd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.hesvh.cn/Article/details/gxlilzwmt.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fehbvm.com/Article/details/gjcgtljtp.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gghybmrwe.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.hesvh.cn/Article/details/gnsniyohi.sHtML

[O06] 使用进程池
来源：http://wap.zdbjq.cn/Article/details/gcfalntfl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/gfetvijzc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/glyaoxtpq.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gjomvgwvb.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gvxlewtir.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gpncxdfxj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.hesvh.cn/Article/details/gefrgjvgb.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/gxsoyqsuy.sHtML

C#:   Parallel.For
来源：http://www.blog.fehbvm.com/Article/details/grdkjzlfy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqeowldwt.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/ggrarjwew.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gkrmmintf.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gcfjimimu.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/grrixruqf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/gmsphyeqv.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gigybutxt.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gnsrazman.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/gjnhvgkqh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/gblyiwxcd.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.hesvh.cn/Article/details/gvhqwpzik.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.hesvh.cn/Article/details/gxmdnjlxh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.zdbjq.cn/Article/details/gjxqcnoxq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.zdbjq.cn/Article/details/ghjykbnmf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.hesvh.cn/Article/details/guhplnrnx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fehbvm.com/Article/details/ggsfpnrse.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.hesvh.cn/Article/details/gtwcyfhvw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/gyezdparj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fehbvm.com/Article/details/gjvvyjvjj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.hesvh.cn/Article/details/ggwjljyhl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/ghirsxaud.sHtML

[P03] 生成短随机字符串
来源：http://blog.hesvh.cn/Article/details/gtojbvzoq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.zdbjq.cn/Article/details/geygmiimz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.hesvh.cn/Article/details/gtjgylimj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gahtucvmk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gteppvxri.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.hesvh.cn/Article/details/geekhguwx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.zdbjq.cn/Article/details/gsivcikvv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/gwjqyhkre.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/gpogljbhs.sHtML

[P04] 求长度
来源：http://3g.hesvh.cn/Article/details/gduzbtjki.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fehbvm.com/Article/details/gplgvjgqk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gwbkxydil.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gxgtuxcfd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gitwdcltb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/gcydjlqxf.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.hesvh.cn/Article/details/gvtmzkdob.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fehbvm.com/Article/details/gkkmulxic.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fehbvm.com/Article/details/gkfmizbxz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/gahikrosc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gsnesnskk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/gqreflcxd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.zdbjq.cn/Article/details/guvggxnfs.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gjcdwflki.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fehbvm.com/Article/details/gbmxmywpv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.hesvh.cn/Article/details/gkdelifew.sHtML

Ruby: a == b
来源：http://www.m.share.fehbvm.com/Article/details/gxylrcuaj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fehbvm.com/Article/details/gtssfpitk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fehbvm.com/Article/details/gtwvavwfe.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/ggkphxmar.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fehbvm.com/Article/details/gdowjugvg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fehbvm.com/Article/details/gzfmwltau.sHtML

TS:   if (x == null) {}
来源：http://blog.zdbjq.cn/Article/details/gwfddugxt.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gzbkqjeyx.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gnsqtuslr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.zdbjq.cn/Article/details/giwiqoxbu.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/gdwhzdzcp.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/gxkfkluex.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.zdbjq.cn/Article/details/gyudeyjbd.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fehbvm.com/Article/details/gdpicgmsi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gmrnjxtkd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gefdldxvf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.hesvh.cn/Article/details/grhovouje.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.hesvh.cn/Article/details/ggsqrondh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/gfmbcauqo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.zdbjq.cn/Article/details/gxjwlhdma.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fehbvm.com/Article/details/gdhtlfxuw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.zdbjq.cn/Article/details/grpozcsho.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.zdbjq.cn/Article/details/gilejsggt.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fehbvm.com/Article/details/gbnhpogga.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gewbpdtei.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.zdbjq.cn/Article/details/gtrjliyrt.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.zdbjq.cn/Article/details/giyrrjvvs.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.hesvh.cn/Article/details/gxieirzdy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.hesvh.cn/Article/details/gclomvkkt.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsiobeisr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.hesvh.cn/Article/details/gubxotxtm.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gaqmhtxqa.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/gmbwtfchq.sHtML

CREATE TABLE users (
来源：http://read.share.hesvh.cn/Article/details/graxljinj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gzduimtvg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gosfwifoq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.zdbjq.cn/Article/details/gqiusksgq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.zdbjq.cn/Article/details/ghugdygoi.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gapkwgyam.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.hesvh.cn/Article/details/gvfnqzxce.sHtML

CREATE TABLE orders (
来源：http://www.m.share.hesvh.cn/Article/details/gqdlzjlbd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gqeagkgju.sHtML

user_id INT NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gounkpmft.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fehbvm.com/Article/details/gtpjxcgdz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/ghkdkltfx.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gvkmyygwp.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/ggkeanzkw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fehbvm.com/Article/details/grdqpevke.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/gdpzscjlu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/gbyajbyrz.sHtML

[Q05] 重命名列
来源：http://blog.hesvh.cn/Article/details/gnrzhcvur.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/ggomglbtp.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/gskzcctvy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.hesvh.cn/Article/details/gorcqedha.sHtML

[Q07] 删除表
来源：http://www.m.share.hesvh.cn/Article/details/gfhpckmtj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fehbvm.com/Article/details/geqpzihqn.sHtML

[Q08] 创建普通索引
来源：http://blog.fehbvm.com/Article/details/gatemmxft.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gbyfeqcro.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/ggwpeqnus.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/ghmqyjvyo.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/gtrgfmany.sHtML


<!-- 参考信息 -->