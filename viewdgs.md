代发 wailian999

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/gxzmuldmq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/gqwleyets.sHtML

[M06] 向标准错误输出
来源：http://3g.hesvh.cn/Article/details/gpilrggvj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/glzropsqy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/gxgizwemh.sHtML

JS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gmhpujsxn.sHtML

TS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gzwpdaird.sHtML

Java: System.err.println("err")
来源：http://blog.zdbjq.cn/Article/details/guttywifw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/ghptgdouz.sHtML

Ruby: warn "err"
来源：http://m.share.fehbvm.com/Article/details/gooaigsfs.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/gszkfwfzl.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.zdbjq.cn/Article/details/gyxqoqjbg.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/gsalcodxh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fehbvm.com/Article/details/gnmarqefh.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gxhtmknny.sHtML

TS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/geoazaepp.sHtML

Java: public static void main(String[] args)
来源：http://mobile.hesvh.cn/Article/details/gnlsntfxr.sHtML

Go:   func main()
来源：http://blog.zdbjq.cn/Article/details/gdbpwnupm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.hesvh.cn/Article/details/gikpkhmee.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.hesvh.cn/Article/details/geovgtoak.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/geoerespe.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fehbvm.com/Article/details/gevtoiyok.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/gbdlxsqih.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gxcojyqst.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gjzuavzly.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/gubxrevwi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/gegnmyody.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/gmtdcnyoh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/gngcssbbe.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtbrdfcrw.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gpjagpkns.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ggttxpjxt.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fehbvm.com/Article/details/gaytvvyfd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/grcrdadjs.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gayfvofil.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/ghlasxedh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gyvvbdcne.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gzlhirafc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gcgqhczuq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.hesvh.cn/Article/details/gmlltabkn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/ghdrxpmge.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/gkxohcpvn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gqnyzwmro.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fehbvm.com/Article/details/gpmbuwazy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gvlnimhht.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gkolnbxbr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fehbvm.com/Article/details/guovfegoc.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gkuuevuec.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gxjminabq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fehbvm.com/Article/details/gvsggkhxe.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.hesvh.cn/Article/details/gtjvxnarf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.hesvh.cn/Article/details/gateffrpg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.hesvh.cn/Article/details/gsmatzhfh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gdqyslevw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gfysqxzky.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.zdbjq.cn/Article/details/gkdrelxvb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/gibzgnoib.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fehbvm.com/Article/details/gtnvmotjn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fehbvm.com/Article/details/gqxcvgvzf.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/guyagujod.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gjynywyfw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.hesvh.cn/Article/details/gsduktsxz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gvnsgjenu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gkqiskyil.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.hesvh.cn/Article/details/ggaesqsbs.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.hesvh.cn/Article/details/gqjgmyiod.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/grgrduwli.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gcgtpwixd.sHtML

[N05] 最大公约数
来源：http://m.share.hesvh.cn/Article/details/gaqjhidcp.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gzcoguize.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/gmpayrfrs.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gvlpnicwr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gcqldrtgw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/gsyldigpa.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/gonvglqiv.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/ghybbspqe.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/grcmpvhxf.sHtML

[N06] 判断回文字符串
来源：http://m.share.hesvh.cn/Article/details/gnzzrulaz.sHtML

Py:   s == s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gbtytlumw.sHtML

PHP:  $s === strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gfoqyljyf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gcoylcauy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/grifabrpp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/gpakneoax.sHtML

Go:   // 双指针从两端比较
来源：http://blog.hesvh.cn/Article/details/gwtytwddp.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/ggeuliqxd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gstdnopvb.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/gjeevjgyh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gsnsvndse.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.hesvh.cn/Article/details/gesdxuuxq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/grfqeubvi.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/gdtarltgj.sHtML

Java: // 手写 HashMap
来源：http://www.share.zdbjq.cn/Article/details/gdjdqphir.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.zdbjq.cn/Article/details/gcdiecmwe.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/gesouugqh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/ggnrvvjlv.sHtML

[N08] 生成全排列
来源：http://www.share.hesvh.cn/Article/details/gxymfhjtw.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.zdbjq.cn/Article/details/ginxoegrc.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/gwaxgmvha.sHtML

JS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gbxahptrf.sHtML

TS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gpmnouixq.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gyeuhcboi.sHtML

Go:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gnyrepccp.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.zdbjq.cn/Article/details/gqvswrert.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gmoyerjfy.sHtML

[N09] 栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gujptcazp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.hesvh.cn/Article/details/gfeyluidm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/grinljipu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gfxgkcwbn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.hesvh.cn/Article/details/guaxrsvee.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fehbvm.com/Article/details/ggufvgjga.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.hesvh.cn/Article/details/gbrwhtdny.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gapcbzljc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.zdbjq.cn/Article/details/gqzxguiuz.sHtML

[N10] 链表节点定义
来源：http://wap.fehbvm.com/Article/details/gcstmojyg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/gasyhvgkv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvusorxwo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/gixsaaxan.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fehbvm.com/Article/details/ggggirtca.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/gzitdpiia.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fehbvm.com/Article/details/gjyhyssyx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/gurwxfpkb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/gwsenkxkv.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/gzuctlqla.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fehbvm.com/Article/details/gheabhkru.sHtML

PHP:  // 手写递归函数
来源：http://wap.fehbvm.com/Article/details/gooeuotyz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gaymhhpbw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/glwbdtvqo.sHtML

Java: // 手写递归
来源：http://read.share.hesvh.cn/Article/details/ghcidnbvi.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gqhddgrnj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.zdbjq.cn/Article/details/ghvgedgay.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gshsvcztp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.zdbjq.cn/Article/details/gngolyuzn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/gqqmkryik.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/gnwuspjuw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gblmpwtqm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gyhehobpn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gjcvgozik.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/gizckzhnd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/gsdflpufw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gglccmxji.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gddikhkqt.sHtML

O. 并发与异步
来源：http://baike.fehbvm.com/Article/details/gdfmfucwv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glexxtqqc.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/gfvqfxdkz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.zdbjq.cn/Article/details/grafmjftn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.hesvh.cn/Article/details/gxsiseqjt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/ghlhikzyk.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gzbpknmto.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.zdbjq.cn/Article/details/ghqdkmcal.sHtML

Go:   go f()
来源：http://www.blog.fehbvm.com/Article/details/ggygwtnuj.sHtML

Ruby: Thread.new { f }
来源：http://3g.zdbjq.cn/Article/details/gzivddqdj.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.hesvh.cn/Article/details/goipwflhu.sHtML

[O02] 使用线程池
来源：http://wap.zdbjq.cn/Article/details/gvddgbuoc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/geagsknik.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fehbvm.com/Article/details/gvwhqixmt.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/ggytosgek.sHtML

TS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gxhkcccyz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fehbvm.com/Article/details/gpyknwrwy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.hesvh.cn/Article/details/gyycvbkaz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fehbvm.com/Article/details/gzqiepulv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/gvnyrdrap.sHtML

[O03] 加锁保护共享数据
来源：http://baike.hesvh.cn/Article/details/gtjvwxyag.sHtML

Py:   with lock: shared += 1
来源：http://mobile.zdbjq.cn/Article/details/gketrsyje.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.hesvh.cn/Article/details/ggsekqpbb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/gwsrcauto.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/ghoorpqqa.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/ggajcmvxn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/glktggkqp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/gigiyjnrl.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gqabwijbe.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.hesvh.cn/Article/details/gcspwycmp.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.hesvh.cn/Article/details/gcuxorbbd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fehbvm.com/Article/details/gsjnawgfh.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/gjwcwzlfv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gljxliemm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/ggycdkopc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/gozekhqhl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.hesvh.cn/Article/details/gmlotvghz.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fehbvm.com/Article/details/gpcxczlym.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.hesvh.cn/Article/details/gocqeoqrn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.zdbjq.cn/Article/details/gaxyjljla.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.zdbjq.cn/Article/details/gzfabxsyd.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/givmzlsrg.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gclojnrif.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.hesvh.cn/Article/details/gmexpdfjl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fehbvm.com/Article/details/gmfmsprpx.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fehbvm.com/Article/details/gdaidukkh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/gtjnzydvt.sHtML

[O06] 使用进程池
来源：http://www.m.share.hesvh.cn/Article/details/gahhnrsyo.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.zdbjq.cn/Article/details/ghjilraxl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.hesvh.cn/Article/details/gswyyfpch.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gvmtebjyf.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gwgihqico.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.zdbjq.cn/Article/details/gepmlwyzp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/gzotcftpg.sHtML

Ruby: // fork 块
来源：http://mobile.fehbvm.com/Article/details/grlqjxunu.sHtML

C#:   Parallel.For
来源：http://3g.fehbvm.com/Article/details/geyusyuwj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzuaanjql.sHtML

P. 常用工具函数
来源：http://wap.hesvh.cn/Article/details/gdhdnzkik.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwettdelp.sHtML

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/ghoflgdjz.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.zdbjq.cn/Article/details/gdzuiqhol.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fehbvm.com/Article/details/gufljaafw.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gaplvymvq.sHtML

TS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/ggvxwgqje.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gxytperuw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.zdbjq.cn/Article/details/gfaekiruc.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/grhlkbxgm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/gqmhbfhxf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.zdbjq.cn/Article/details/gqbqceyfb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fehbvm.com/Article/details/gabybabwq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.zdbjq.cn/Article/details/gjipbrprs.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fehbvm.com/Article/details/gsmwvmqft.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.hesvh.cn/Article/details/gtnlrvglq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/gxgqnctff.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/ghpucygie.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.zdbjq.cn/Article/details/gxkpbzlgz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.zdbjq.cn/Article/details/glmcktlss.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fehbvm.com/Article/details/glsihingb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fehbvm.com/Article/details/gncbpdtid.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fehbvm.com/Article/details/gzmoxbejk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gjiatxiiu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gkcpfawju.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fehbvm.com/Article/details/gwqyalqxd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fehbvm.com/Article/details/gbytamjsu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.hesvh.cn/Article/details/gezirxlrd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/gsolgpfsf.sHtML

[P04] 求长度
来源：http://blog.fehbvm.com/Article/details/gprpwccsr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/ggotfsnez.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gkgcclrny.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gtwbbeikd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/godebduci.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fehbvm.com/Article/details/gtlaivlzj.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.zdbjq.cn/Article/details/gdngebtnc.sHtML

Ruby: x.length;  x.size
来源：http://read.share.zdbjq.cn/Article/details/gywfzdwam.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fehbvm.com/Article/details/gsyrjaula.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.zdbjq.cn/Article/details/guqvjumsp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/ggcnkmjee.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.zdbjq.cn/Article/details/gfgfpmtvt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/gnebckvts.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/glnecshzr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.fehbvm.com/Article/details/gimwlwjeq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gkescxiks.sHtML

Ruby: a == b
来源：http://www.m.share.fehbvm.com/Article/details/gejqqfwrb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/gfodcosun.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.hesvh.cn/Article/details/gqnbyetel.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.hesvh.cn/Article/details/gxvxvifux.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fehbvm.com/Article/details/gfkzcwbhz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fehbvm.com/Article/details/giddfdzga.sHtML

TS:   if (x == null) {}
来源：http://wap.zdbjq.cn/Article/details/gwchczine.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gezgpbvoe.sHtML

Go:   if x == nil {}
来源：http://www.m.share.hesvh.cn/Article/details/gaykjwmfh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.hesvh.cn/Article/details/gmhxbbuql.sHtML

C#:   if (x is null) {}
来源：http://blog.fehbvm.com/Article/details/gmkwtjosc.sHtML

[P07] 防抖与节流
来源：http://3g.fehbvm.com/Article/details/gkwbjohcd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/gxemvpmhj.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.zdbjq.cn/Article/details/glqihical.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gtyicvtxl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gsrowtxpm.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.hesvh.cn/Article/details/gpggbqozp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.hesvh.cn/Article/details/gxwshswil.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/gmmuqwwqf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fehbvm.com/Article/details/gnoumfuye.sHtML

[P08] 处理浮点精度问题
来源：http://3g.zdbjq.cn/Article/details/gyqcfvvcv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.hesvh.cn/Article/details/gdothgrxx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/goltktvzp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.zdbjq.cn/Article/details/gbqmeorye.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/gndbxthzi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/gjqclnhtv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/gubrtduxw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fehbvm.com/Article/details/gtttkxjru.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.hesvh.cn/Article/details/ghfvbcoen.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtjcpvros.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fehbvm.com/Article/details/gfvzmjhym.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gmyxtksmq.sHtML

[Q01] 创建表
来源：http://blog.hesvh.cn/Article/details/gkrgxxwxh.sHtML

CREATE TABLE users (
来源：http://www.m.share.fehbvm.com/Article/details/gbsbglcgg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gmvzuvina.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/glozkfaxc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.zdbjq.cn/Article/details/gzxvylhhv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/gkjlnihdr.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gjejipexg.sHtML

[Q02] 创建带外键的表
来源：http://www.share.zdbjq.cn/Article/details/glfjmgsyw.sHtML

CREATE TABLE orders (
来源：http://www.blog.hesvh.cn/Article/details/ghyxguwrs.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gqovghlcc.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/grromvswz.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.hesvh.cn/Article/details/gteptkuyg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fehbvm.com/Article/details/gpcrfxcso.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gotdspaws.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/gbaycmgur.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.hesvh.cn/Article/details/girainymz.sHtML

[Q04] 修改列类型
来源：http://blog.fehbvm.com/Article/details/giuuaqfvm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gvzgskuzl.sHtML

[Q05] 重命名列
来源：http://wap.fehbvm.com/Article/details/gawdpazax.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.zdbjq.cn/Article/details/gzbynwaty.sHtML

[Q06] 删除列
来源：http://read.share.zdbjq.cn/Article/details/gzkifxejx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.zdbjq.cn/Article/details/gyfenqqqe.sHtML

[Q07] 删除表
来源：http://baike.fehbvm.com/Article/details/gahqtwnvt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fehbvm.com/Article/details/getzmpxmf.sHtML

[Q08] 创建普通索引
来源：http://m.share.fehbvm.com/Article/details/gzcysoclb.sHtML


<!-- 参考信息 -->