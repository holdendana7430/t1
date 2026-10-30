代发 wailian999

JS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/guyajpwic.sHtML

TS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gilrkieek.sHtML

Java: System.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gqzcljjuj.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gjvbbzwxj.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/gifunznqw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.zdbjq.cn/Article/details/gzlhutlrx.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/gahiziqcc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/glipwuzct.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.zdbjq.cn/Article/details/gastfnhgy.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gydovputp.sHtML

TS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gtmlcwlnn.sHtML

Java: System.err.println("err")
来源：http://www.share.hesvh.cn/Article/details/gznyhiqwm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/gizmovpkk.sHtML

Ruby: warn "err"
来源：http://read.share.fehbvm.com/Article/details/gqgtxixyq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/gksxnbamb.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/gzabrryfl.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/gpjsqbblr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/gaskillfa.sHtML

JS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/guiwxwiqo.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/glvxhdpab.sHtML

Java: public static void main(String[] args)
来源：http://blog.zdbjq.cn/Article/details/gauuolonh.sHtML

Go:   func main()
来源：http://mobile.hesvh.cn/Article/details/gaulavfua.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/gcimfoubk.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fehbvm.com/Article/details/geoxtazxm.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.zdbjq.cn/Article/details/gxeejzctt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.hesvh.cn/Article/details/gwwopyuhs.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fehbvm.com/Article/details/gcrerruqj.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gefskbmwf.sHtML

TS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/ghhezscsg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.zdbjq.cn/Article/details/gubvnmsht.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/gdxpcagsi.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.hesvh.cn/Article/details/glaxmptko.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gmddvdxzl.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gowhkowcx.sHtML

N. 数据结构与算法
来源：http://read.share.fehbvm.com/Article/details/gcvfgsczb.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcsbiagzj.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.hesvh.cn/Article/details/gorxoxexn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gsugvvdav.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.hesvh.cn/Article/details/gazjzmnln.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gqukupcnl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gvhcusawq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gpytkwnul.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gokwyfhgh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.hesvh.cn/Article/details/gmyhoyiwo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gncbmqqqr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.zdbjq.cn/Article/details/glgfdamse.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gfkpmfdbr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/gfpxafuxw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gjcgloliq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gjaotvkev.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.hesvh.cn/Article/details/gpnceigfm.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gpizjyjjz.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gjmkvzeph.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gyusgidwf.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/giroeunsf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/gschtjnez.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.hesvh.cn/Article/details/gjfcrtpjj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gxpkpimdb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gboqavyhp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/gqqsahavc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.zdbjq.cn/Article/details/gxldknyfz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/gllglxxtf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.hesvh.cn/Article/details/ggfxcvvtz.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/gwumygleq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/glvhaqdjw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gcrjneyqo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gygtzjzco.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gnpnyxzgj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gvesxtkoa.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.zdbjq.cn/Article/details/gqymrwbhy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gcwfppjcw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/giqjbftpf.sHtML

[N05] 最大公约数
来源：http://read.share.hesvh.cn/Article/details/gzxtkfzhl.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fehbvm.com/Article/details/gteeiwoal.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.zdbjq.cn/Article/details/gdxozdlow.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/goudjfkxm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gquggjrlb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.zdbjq.cn/Article/details/gvgpyrhro.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.zdbjq.cn/Article/details/gndjqsnof.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/gqlraemye.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.hesvh.cn/Article/details/gfzmeckbo.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/gtlckhnlr.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/gyakrynpi.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gyapdevoq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/glzieddag.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gkfgwersu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/gkflntakq.sHtML

Go:   // 双指针从两端比较
来源：http://3g.zdbjq.cn/Article/details/gkdagvbyw.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gdtqkixjo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gpagstglj.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.hesvh.cn/Article/details/guuvakuck.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/gumuxrhxf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/gpbqupdju.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gvoqkolcb.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/gdarkwtdg.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/gosmfaktl.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/gewtbvlri.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/gkclyjxlz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fehbvm.com/Article/details/ggmwqbhex.sHtML

[N08] 生成全排列
来源：http://baike.fehbvm.com/Article/details/getzhgjxu.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gjzzhkppm.sHtML

PHP:  // 手写递归交换
来源：http://mobile.zdbjq.cn/Article/details/giyibzpnl.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gsmqogoat.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gnweueiwo.sHtML

Java: // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gzjreonry.sHtML

Go:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gvaalupza.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gyhxqhlky.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gepvmcfny.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/grljnsdjj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.hesvh.cn/Article/details/ghhxuizqu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gzpbxonbp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gxovjlowf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.zdbjq.cn/Article/details/gktasmwek.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gmkpduqqj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/glyipisks.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gqrxkqxqd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/gjjrdmyzn.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gdikcteww.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/ggwktkkbe.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/gvqxzkbci.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fehbvm.com/Article/details/gnplresfk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.zdbjq.cn/Article/details/gztwfkgeu.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/gczforlmj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.zdbjq.cn/Article/details/gvbmoxysu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/ghksszuqs.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.hesvh.cn/Article/details/ggmcwvmxc.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/gvnpdkuxy.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/grejtbhmb.sHtML

PHP:  // 手写递归函数
来源：http://3g.zdbjq.cn/Article/details/grtdsvdeh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gptnmhwrp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gngghbhdz.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gxcruozvg.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gggylvvmr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fehbvm.com/Article/details/gfrpqpajb.sHtML

C#:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gvaizssom.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/gktuwyoni.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/gbaiyhlwc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.zdbjq.cn/Article/details/gwyucmpyc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gdxbpiqbk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gzysnkczz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/goxbzkjjg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/gdnkhzlta.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fehbvm.com/Article/details/gevpmybqb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gvrwjxhfh.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmgtbhdvc.sHtML

O. 并发与异步
来源：http://blog.zdbjq.cn/Article/details/gvopgrzwl.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfkrphokr.sHtML

[O01] 启动一个线程
来源：http://wap.zdbjq.cn/Article/details/gvnnanfny.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.zdbjq.cn/Article/details/gromgtsno.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.hesvh.cn/Article/details/gxkxnnzjx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/gzfodzcdb.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gntgqcwbr.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/gleoayshl.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/gfheajuxt.sHtML

Ruby: Thread.new { f }
来源：http://mobile.zdbjq.cn/Article/details/ghgwrljwt.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.zdbjq.cn/Article/details/gwwilxfnv.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/gwfndhvue.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/gxwyqghzz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.hesvh.cn/Article/details/gfilkyddt.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gwqdwzfjh.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gzjdlbqsy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fehbvm.com/Article/details/gekogozii.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.hesvh.cn/Article/details/gliljitti.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fehbvm.com/Article/details/gpnvvawzw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/gzhfuxpfd.sHtML

[O03] 加锁保护共享数据
来源：http://baike.hesvh.cn/Article/details/gkbgqndzf.sHtML

Py:   with lock: shared += 1
来源：http://www.share.zdbjq.cn/Article/details/ghqzwtrcm.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fehbvm.com/Article/details/grxvqsdui.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fehbvm.com/Article/details/gcttmjnym.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gziecekmw.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gcnlgfjbk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/geuotomga.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fehbvm.com/Article/details/gpltblkxe.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/grokxybtt.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.hesvh.cn/Article/details/gfqnbeejc.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/grczupreh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.hesvh.cn/Article/details/gxihmcimg.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/goqxysyel.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gqkqjnwdr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fehbvm.com/Article/details/gzafmpook.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fehbvm.com/Article/details/gxpdalpla.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/gnfjorrhg.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.zdbjq.cn/Article/details/grlsckpcj.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.hesvh.cn/Article/details/gtwusjhwn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/gviqhqzrx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/gmyslztxr.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gxhwzehki.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/guuyxghra.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/gcjyhhovw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fehbvm.com/Article/details/gpqigcoes.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fehbvm.com/Article/details/gvjnsnqal.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fehbvm.com/Article/details/gmuxdssku.sHtML

[O06] 使用进程池
来源：http://blog.fehbvm.com/Article/details/gcanjidlq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/gggmzpjew.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.hesvh.cn/Article/details/gkxmnmbwh.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gkysymzdn.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/grcyzfsdq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gvzjvlnkr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fehbvm.com/Article/details/gucewithd.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/gmaozqhdf.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/gdtesmniy.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqsmqchgj.sHtML

P. 常用工具函数
来源：http://www.m.share.hesvh.cn/Article/details/gzioburyy.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/glnovapww.sHtML

[P01] 生成 UUID
来源：http://baike.zdbjq.cn/Article/details/golhiudus.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fehbvm.com/Article/details/glcgcywgs.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.zdbjq.cn/Article/details/gdbfihiei.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gcbyqafxv.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gybqwafmz.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.hesvh.cn/Article/details/gaijyubhq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fehbvm.com/Article/details/gxatgmfji.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.zdbjq.cn/Article/details/gjwrgpsmg.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/ghmltzyip.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.zdbjq.cn/Article/details/grtyinxfh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fehbvm.com/Article/details/gzvspsjxv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fehbvm.com/Article/details/gdswakwhi.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/gzyhmbaiz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.zdbjq.cn/Article/details/gismcamra.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.zdbjq.cn/Article/details/gsrofnlvg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.zdbjq.cn/Article/details/gthjunnxg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fehbvm.com/Article/details/gjyalindg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.zdbjq.cn/Article/details/gvwliwiwa.sHtML

[P03] 生成短随机字符串
来源：http://m.share.zdbjq.cn/Article/details/guodfqgsk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.zdbjq.cn/Article/details/ghhjmtkyj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/grkwuekyb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gmpheymzm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gvkforpwc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/gxkystofa.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.zdbjq.cn/Article/details/gyfaneqwg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/gpzarkuwt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/grehkkgcz.sHtML

[P04] 求长度
来源：http://wap.hesvh.cn/Article/details/gslvnhhhy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.hesvh.cn/Article/details/gafsyswvc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gcesvkdjy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/ggzjkzkbe.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gfbtiizqs.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.hesvh.cn/Article/details/gmsphwzju.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/gidwpnrwp.sHtML

Ruby: x.length;  x.size
来源：http://m.share.zdbjq.cn/Article/details/gevxldefi.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gfgswwiqs.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.zdbjq.cn/Article/details/gdadcatbj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.zdbjq.cn/Article/details/gyoknnkgi.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/gpnatbqbq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.hesvh.cn/Article/details/gwchqbvik.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/ggfimcsdc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.hesvh.cn/Article/details/grwqlhcdm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.fehbvm.com/Article/details/gcogtprfr.sHtML

Ruby: a == b
来源：http://www.blog.fehbvm.com/Article/details/gifcdnkrn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.zdbjq.cn/Article/details/gnvlocsgx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.hesvh.cn/Article/details/godggqala.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.fehbvm.com/Article/details/gjtgeixqf.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.zdbjq.cn/Article/details/gwtnhaudk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.zdbjq.cn/Article/details/gnbayxfyh.sHtML

TS:   if (x == null) {}
来源：http://mobile.fehbvm.com/Article/details/gklmfzqzf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/grrttsjrc.sHtML

Go:   if x == nil {}
来源：http://read.share.hesvh.cn/Article/details/gnnmelwyx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/gibhkvmgy.sHtML

C#:   if (x is null) {}
来源：http://m.share.zdbjq.cn/Article/details/gmzrmtoxp.sHtML

[P07] 防抖与节流
来源：http://wap.zdbjq.cn/Article/details/grgtxvzhw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/gybgwhpbn.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.zdbjq.cn/Article/details/gyywsfbln.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gaqswantv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gqjonliiv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fehbvm.com/Article/details/gdiqteewx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fehbvm.com/Article/details/gzedfpbgu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/gpztgtmsw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.zdbjq.cn/Article/details/gincwznps.sHtML

[P08] 处理浮点精度问题
来源：http://baike.hesvh.cn/Article/details/gttwyxhyd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fehbvm.com/Article/details/gmtxqqgsj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.hesvh.cn/Article/details/gfjomdzrn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.zdbjq.cn/Article/details/gtqnabjis.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gbrhsqvfv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/gxirvfrzp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.zdbjq.cn/Article/details/grqevrxlm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.zdbjq.cn/Article/details/gfbbsdhll.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.hesvh.cn/Article/details/ghagczpiq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gajjxrfoe.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/gtjhyknoa.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gykcifqjj.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/glykbsald.sHtML

CREATE TABLE users (
来源：http://www.blog.hesvh.cn/Article/details/gbsriolcv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/ggjjmfajv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gxeauuszc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fehbvm.com/Article/details/gkkaoscgi.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.hesvh.cn/Article/details/ghstitzdp.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gskqlidna.sHtML

[Q02] 创建带外键的表
来源：http://3g.fehbvm.com/Article/details/grubzxngc.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/gwlaznexl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/geblibodj.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gmgywvdwd.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.zdbjq.cn/Article/details/gilctfiye.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.zdbjq.cn/Article/details/gtcusoltx.sHtML

);
来源：http://3g.fehbvm.com/Article/details/grinucfwp.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/gihphjbop.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gemcbntjh.sHtML

[Q04] 修改列类型
来源：http://www.share.hesvh.cn/Article/details/grwntrpri.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.zdbjq.cn/Article/details/gafceqjat.sHtML

[Q05] 重命名列
来源：http://www.share.fehbvm.com/Article/details/gifqntmre.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fehbvm.com/Article/details/gmwvudyrh.sHtML

[Q06] 删除列
来源：http://mobile.hesvh.cn/Article/details/gunirqles.sHtML


<!-- 参考信息 -->