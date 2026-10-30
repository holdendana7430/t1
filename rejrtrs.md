代发 wailian999

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/gskluxkcr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/gmuhabtnv.sHtML

[M06] 向标准错误输出
来源：http://mobile.fehbvm.com/Article/details/gmlworyay.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/guanatfmf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.zdbjq.cn/Article/details/gphsawkaj.sHtML

JS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/ghowswfpb.sHtML

TS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gwgduahtg.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/ggmbjzwgo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.zdbjq.cn/Article/details/ghmotyccx.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/gwyylugts.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.hesvh.cn/Article/details/gmqlevfoy.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/gptucuqxc.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fehbvm.com/Article/details/gqdjuaoic.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fehbvm.com/Article/details/garbrvseh.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/ghptjzgex.sHtML

TS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gcihgnkgs.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.hesvh.cn/Article/details/gwawzkvfq.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/gyofnraxh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/gttigpcsd.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/gkyqihigi.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.zdbjq.cn/Article/details/gdrclnkvd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.zdbjq.cn/Article/details/gualkvukg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.zdbjq.cn/Article/details/gaydzcsov.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/glcgskfse.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gbosgfqil.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fehbvm.com/Article/details/gxbimubdi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.hesvh.cn/Article/details/gqdcpmpgv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/ggxtnyqeh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.zdbjq.cn/Article/details/gutngbyfx.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gemxwoaxr.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/gshhrxhbb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvjilirry.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.hesvh.cn/Article/details/gehdmskcg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gkoftheee.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/gpetlgejs.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gmnxwzcia.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gvmzezbml.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gltrevzmo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fehbvm.com/Article/details/gfflfrxwh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/gexbdkzmq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/ghkdimwdg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fehbvm.com/Article/details/gzrhkamzj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gqekkxapl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gtkghfdph.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gctznhhnp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/ggjbgsgfc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.hesvh.cn/Article/details/giwrgjjht.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gmipzsfup.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gswisranu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fehbvm.com/Article/details/grxxvsnwf.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/gyozggzrk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fehbvm.com/Article/details/gwleolwxp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/gyjjoqdzf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/grfymblix.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gflmbxvvc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/gzmmwkxjt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.zdbjq.cn/Article/details/gxorpwpyo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/gaxghxqay.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fehbvm.com/Article/details/gkwtqcfni.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/glglfpdvn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/geawpdhsd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/gmkjfcdfx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gxiofmpfs.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gqhubjzun.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gzzywfluc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.zdbjq.cn/Article/details/gxouwvxlu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gbohqmnvv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gjdgwijct.sHtML

[N05] 最大公约数
来源：http://www.blog.fehbvm.com/Article/details/giihzugfy.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.hesvh.cn/Article/details/gzcjyslwu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/gpcyjpyzs.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gvatoapqq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/grbhcqfzz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.zdbjq.cn/Article/details/gogoozjhx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.zdbjq.cn/Article/details/gjarsrsmp.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/ggxfunfhy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/gqotuistw.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fehbvm.com/Article/details/gflmzwmkm.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gngeucghv.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.hesvh.cn/Article/details/graxctivr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gitskpkyj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/goohcqxxw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fehbvm.com/Article/details/gmmqivufx.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/gecetqdzn.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/gqfqynpds.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gtfapeuyq.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.zdbjq.cn/Article/details/gkbmrevyf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.hesvh.cn/Article/details/guvhjlpmg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/gjjjtsxui.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.hesvh.cn/Article/details/gmdsqkkxx.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/gmjzaikpb.sHtML

Java: // 手写 HashMap
来源：http://blog.hesvh.cn/Article/details/gttdlqigt.sHtML

Go:   // 手写 map[int]int
来源：http://wap.hesvh.cn/Article/details/gdlsorgci.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/gezlgptkp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fehbvm.com/Article/details/gjvjkcdkw.sHtML

[N08] 生成全排列
来源：http://m.share.fehbvm.com/Article/details/ghselvayt.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/gatqheedu.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/gwzzkhjhw.sHtML

JS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gwxdzcixu.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/ggnfnobrn.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gmfvwdbio.sHtML

Go:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/ghfwknwmz.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fehbvm.com/Article/details/gklnyejwi.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gqgbgomll.sHtML

[N09] 栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gsewmlvrg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.hesvh.cn/Article/details/gxgzyopvf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.hesvh.cn/Article/details/gzvsftvtl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gfzpkmimt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fehbvm.com/Article/details/gsgwdbaul.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fehbvm.com/Article/details/ggzxjkysx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/gtysbpeoq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gsizrymme.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.zdbjq.cn/Article/details/gesmbjbue.sHtML

[N10] 链表节点定义
来源：http://www.blog.hesvh.cn/Article/details/gfzcpknjm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.zdbjq.cn/Article/details/gaqzwuhba.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/gikkgvduw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.hesvh.cn/Article/details/gccbetflu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.zdbjq.cn/Article/details/glidmwsli.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/guftllpbo.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/gnyfmgyid.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fehbvm.com/Article/details/gixellkur.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/gvvqozipi.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/gfqdhylrs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fehbvm.com/Article/details/gsrzrhkpy.sHtML

PHP:  // 手写递归函数
来源：http://mobile.zdbjq.cn/Article/details/gzlmytvef.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gznmwdqew.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gjwpescxx.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/ghfvnkhrv.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gjhtsigwc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fehbvm.com/Article/details/gqiqcwhiw.sHtML

C#:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/glmgmagvr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fehbvm.com/Article/details/gdyyqxsux.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fehbvm.com/Article/details/gdyermvst.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/gugwevqrg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/glhgarhmu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gnmiktruw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gbbarsogx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/gyqjsmsir.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.zdbjq.cn/Article/details/gyklmawwn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gaxuuhfqy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmsaqtwkn.sHtML

O. 并发与异步
来源：http://wap.fehbvm.com/Article/details/gcatqphps.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzvqlooil.sHtML

[O01] 启动一个线程
来源：http://blog.zdbjq.cn/Article/details/glsqqdrul.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/grnlbxqxa.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/gwjbixfhq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.hesvh.cn/Article/details/gdmgbanbn.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gitevjnhe.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/gmlvnvwcv.sHtML

Go:   go f()
来源：http://mobile.fehbvm.com/Article/details/gfmdotrsa.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/ggsghpyuc.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fehbvm.com/Article/details/gzceepwsw.sHtML

[O02] 使用线程池
来源：http://3g.fehbvm.com/Article/details/ghlkxcvyo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.hesvh.cn/Article/details/gnokazdxv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/gocidpefy.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gecfwyzsa.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gepzdyvkz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/gukfukogf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/gwagklgqs.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fehbvm.com/Article/details/gbznsvavi.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fehbvm.com/Article/details/gmmyikwph.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/golgyhlou.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gktsafppr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/gryijiugz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/gxmmyabnc.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gubcgtidl.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gbxtaxxnt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.zdbjq.cn/Article/details/gyhzyccmh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fehbvm.com/Article/details/grtymsbqu.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gezhmapip.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/gyqmvaaan.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/geuznrbkf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.zdbjq.cn/Article/details/gnkisropc.sHtML

JS:   async function f() { await g(); }
来源：http://wap.zdbjq.cn/Article/details/giewfijxu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fehbvm.com/Article/details/ghcnedftc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.hesvh.cn/Article/details/gyxwmxmiw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/grqmnehod.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.hesvh.cn/Article/details/gansfmhew.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/gaalquuah.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.zdbjq.cn/Article/details/gsweitvne.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.zdbjq.cn/Article/details/gxnugeoks.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.hesvh.cn/Article/details/gmkkxjppc.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gvpgkruup.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/glhppscze.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.zdbjq.cn/Article/details/gnrzoadci.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fehbvm.com/Article/details/glcqfxqqe.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.zdbjq.cn/Article/details/ghlfsjfcf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/gizsyxbug.sHtML

[O06] 使用进程池
来源：http://www.m.share.fehbvm.com/Article/details/gkquyxqgp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/gpzbckpjx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/gkjuzfpyu.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gwjxffwho.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gjztvrjud.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.zdbjq.cn/Article/details/gfylobcyk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/gvmzapnnv.sHtML

Ruby: // fork 块
来源：http://blog.fehbvm.com/Article/details/gfyypanwq.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/geqydaohc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/glkwlkiqx.sHtML

P. 常用工具函数
来源：http://read.share.zdbjq.cn/Article/details/gnuvxcmal.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmzolvpvm.sHtML

[P01] 生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/goiwfxzjw.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/ghhrqvega.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fehbvm.com/Article/details/gqsflbszi.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gaztxqkhr.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gezzbvqdu.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fehbvm.com/Article/details/gkjbupjah.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.zdbjq.cn/Article/details/gkduyiqye.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fehbvm.com/Article/details/ghtmdkwhx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.hesvh.cn/Article/details/gspaopvvw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/gmetbjpfv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.zdbjq.cn/Article/details/gbdkpdiec.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/glzadplta.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/gyekqjrxf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.zdbjq.cn/Article/details/ghawqxheo.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fehbvm.com/Article/details/gwmpmihxw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.hesvh.cn/Article/details/gvaxfdaob.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.hesvh.cn/Article/details/gbtasgdwh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/gbzoufuci.sHtML

[P03] 生成短随机字符串
来源：http://mobile.zdbjq.cn/Article/details/ggpgpyevn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fehbvm.com/Article/details/gqymlqgqx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fehbvm.com/Article/details/gknefzvpk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gbhpexogi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gcunmtrpo.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/gktonmzlw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/grgyvcmmz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.zdbjq.cn/Article/details/gaqmjxwuo.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fehbvm.com/Article/details/gffimqyjl.sHtML

[P04] 求长度
来源：http://blog.fehbvm.com/Article/details/gqlfvbpyv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/gjonfgywo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gcendeoof.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gtzxehmzb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gwuajhyji.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gaawddior.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.hesvh.cn/Article/details/gqahahczd.sHtML

Ruby: x.length;  x.size
来源：http://read.share.zdbjq.cn/Article/details/ghfmdyhyj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/gucxsrxkl.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.zdbjq.cn/Article/details/gznpvgtwl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.zdbjq.cn/Article/details/gmccdgzqf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.hesvh.cn/Article/details/glhnowwkq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.zdbjq.cn/Article/details/gukykfxum.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gkabewsop.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.hesvh.cn/Article/details/ggpexnqwf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.fehbvm.com/Article/details/ghqbvzltq.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/gjovpnvdq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.zdbjq.cn/Article/details/gecfkrcdr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.zdbjq.cn/Article/details/gzfocdipn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.hesvh.cn/Article/details/glsvkomaq.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fehbvm.com/Article/details/gzbgsmzps.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/gireuxkwb.sHtML

TS:   if (x == null) {}
来源：http://www.share.fehbvm.com/Article/details/gndjgfmli.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/glikexpne.sHtML

Go:   if x == nil {}
来源：http://www.blog.zdbjq.cn/Article/details/gynmxqboo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.hesvh.cn/Article/details/gbebxchhz.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/gtwxnjbfb.sHtML

[P07] 防抖与节流
来源：http://wap.zdbjq.cn/Article/details/gepjcwksc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fehbvm.com/Article/details/grforcszn.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.hesvh.cn/Article/details/gfxuiyofs.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gaoqjjnki.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gdgmuelti.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.zdbjq.cn/Article/details/gshcnkwok.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/gulonviqi.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/gcautnhzk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fehbvm.com/Article/details/gytideual.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fehbvm.com/Article/details/gekggbukz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fehbvm.com/Article/details/gquhrdavt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.hesvh.cn/Article/details/grremhpcc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fehbvm.com/Article/details/gauytmznt.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/gbfpgrusg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.zdbjq.cn/Article/details/gxxdbbbej.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fehbvm.com/Article/details/gquxgsjmy.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.zdbjq.cn/Article/details/gcbbgbkto.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fehbvm.com/Article/details/gqfosgfym.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gavwphbst.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fehbvm.com/Article/details/ghcqbnvei.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gsjzzjrra.sHtML

[Q01] 创建表
来源：http://3g.zdbjq.cn/Article/details/gvvkgqelt.sHtML

CREATE TABLE users (
来源：http://baike.zdbjq.cn/Article/details/gxkdpxngy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gaqqvfdpr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gwifvinwo.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/gnzuxgbzl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/ggguwkvwm.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gvendwyax.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.hesvh.cn/Article/details/gncifhunm.sHtML

CREATE TABLE orders (
来源：http://mobile.zdbjq.cn/Article/details/gbpwcrlyh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gjhjhztme.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gjgkgcyti.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.zdbjq.cn/Article/details/gkjpkxert.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fehbvm.com/Article/details/gtdzgrhjl.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gnrqlligk.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/giquysfyu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.hesvh.cn/Article/details/gcitjndjm.sHtML

[Q04] 修改列类型
来源：http://3g.fehbvm.com/Article/details/gooasazcf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.hesvh.cn/Article/details/gneezvjij.sHtML

[Q05] 重命名列
来源：http://3g.zdbjq.cn/Article/details/gtqdpebai.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.hesvh.cn/Article/details/guthhhsvl.sHtML

[Q06] 删除列
来源：http://www.blog.zdbjq.cn/Article/details/gkhxasxbt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/geukjlydz.sHtML

[Q07] 删除表
来源：http://3g.fehbvm.com/Article/details/gqgkcuyhz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.zdbjq.cn/Article/details/geizxnxyi.sHtML

[Q08] 创建普通索引
来源：http://mobile.zdbjq.cn/Article/details/gmpmwuedh.sHtML


<!-- 参考信息 -->