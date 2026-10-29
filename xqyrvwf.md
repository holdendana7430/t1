代发 wailian999

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gofuhkhqk.sHtML

TS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gmtarcpfm.sHtML

Java: System.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/giqhsmugx.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/grrevlqgz.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/gbhmxdccv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.zdbjq.cn/Article/details/gukeduypi.sHtML

[M06] 向标准错误输出
来源：http://3g.hesvh.cn/Article/details/giuqgbmks.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gqdpgcnsh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.hesvh.cn/Article/details/gaknksybg.sHtML

JS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gicaxzeee.sHtML

TS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gkehdierz.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/gqomkdyrz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fehbvm.com/Article/details/gyqkuorhb.sHtML

Ruby: warn "err"
来源：http://mobile.zdbjq.cn/Article/details/gkxwjsoan.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.hesvh.cn/Article/details/gsijrkdwr.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/gwuvjjvux.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/gubsyjaza.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.hesvh.cn/Article/details/gsmvgwcjz.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gpkvgiesg.sHtML

TS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gfjgphuvz.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gwuancsoi.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/grffpetzh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/ggiuvmjag.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gqrczghno.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.hesvh.cn/Article/details/gvbxvytgs.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/gfsmpqxgv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fehbvm.com/Article/details/gwgcclhla.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gpdedzvhp.sHtML

TS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gvrsutunr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fehbvm.com/Article/details/gsssfrqjf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/gezzieact.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/gyihssseg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/glhakpomn.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/guugjpypp.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/gueffznhj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjyusslog.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/gqzpgideh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gxivaldvm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.hesvh.cn/Article/details/gzjwvdkcb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gtpsrtoxd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gvooymkys.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gcdwktewe.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gxnrqszpj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.zdbjq.cn/Article/details/grbivewtq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gjhjszesb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/gfyewlyts.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gparcqhyx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.hesvh.cn/Article/details/gtfrqsgxz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gwvmpilsz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gkselyyhi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gcyyabfve.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gavfnexca.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/galgsgmwm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fehbvm.com/Article/details/gqkjiqnhe.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/gvoiejynn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/gnfqunicf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.zdbjq.cn/Article/details/gwzgrtadd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/goffnglej.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gmxffidje.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fehbvm.com/Article/details/gpgpbnqzw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fehbvm.com/Article/details/gehtdzgst.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.zdbjq.cn/Article/details/gakshfvrz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/gzdgcovqe.sHtML

[N04] 斐波那契数列
来源：http://wap.zdbjq.cn/Article/details/gwmnhpxdo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gqdnzkqjj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fehbvm.com/Article/details/gvxrnhzuh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gtolwhidj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gfvrpnhpj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gmuoadlsn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/gighcsswl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gpajpplyl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/grrdrrudp.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/glcclnuzy.sHtML

Py:   math.gcd(a, b)
来源：http://blog.zdbjq.cn/Article/details/gcmqwbron.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fehbvm.com/Article/details/gucngwmqb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gagmoftsh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gkfbgeeev.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/gjnelefhk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/gstzfweox.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fehbvm.com/Article/details/ggcdrfxdy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fehbvm.com/Article/details/gshhhpqle.sHtML

[N06] 判断回文字符串
来源：http://www.share.fehbvm.com/Article/details/ggmgeihvh.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gtelybrzb.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gqeebrday.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gnsvppkph.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gbkjhfatu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fehbvm.com/Article/details/geuxxwrvr.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/ggttjodxt.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/gzjpkovud.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/ghczkjnla.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.hesvh.cn/Article/details/gyluwwdlb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.hesvh.cn/Article/details/gjztxkcdo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/ggsixsmam.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/gcropeely.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/ghfpqlybr.sHtML

Java: // 手写 HashMap
来源：http://www.blog.hesvh.cn/Article/details/govpxjwdv.sHtML

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/griamdinf.sHtML

Ruby: // 手写 Hash
来源：http://blog.hesvh.cn/Article/details/gbumpudcj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/ggvxnsdzb.sHtML

[N08] 生成全排列
来源：http://read.share.fehbvm.com/Article/details/ghygkqlrl.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gdkfjfklr.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/gfljpjavw.sHtML

JS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/ggmrylksi.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gpivnvred.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gftrmsiaj.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gnjzdijqc.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.hesvh.cn/Article/details/gugqvlzgh.sHtML

C#:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gmqwwmbir.sHtML

[N09] 栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gdlmolawg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gvevbtjzi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/gwvwcselm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gsldndqtb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/gmmldqihb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gtxnxtpzc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.zdbjq.cn/Article/details/gcfeqdyzs.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gqordlumn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/ggejxppgp.sHtML

[N10] 链表节点定义
来源：http://mobile.zdbjq.cn/Article/details/gcjfxxree.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fehbvm.com/Article/details/gradyxrtu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/gadjzjosz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.hesvh.cn/Article/details/gbikyzfpo.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fehbvm.com/Article/details/gwrjxtmyw.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gwxqtylai.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.zdbjq.cn/Article/details/gpajcgwdz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.zdbjq.cn/Article/details/gkvvuvnxg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/gsqqosbnw.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.hesvh.cn/Article/details/gnpqvpuyi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fehbvm.com/Article/details/gjvgavbfg.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fehbvm.com/Article/details/gtxubzdji.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gfyuwyhta.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gcupypohi.sHtML

Java: // 手写递归
来源：http://baike.hesvh.cn/Article/details/gcbkauiwu.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/ggfhdeybi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fehbvm.com/Article/details/gezqevsqp.sHtML

C#:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/ghcfteihr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/gsrkuppdr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/gebspbqyg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/ghtodazpn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gxmiqjotg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gblgznruq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gnvnkrgph.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/guqseygvd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fehbvm.com/Article/details/gocvdxnfi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gjdabhczh.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkkjvzhri.sHtML

O. 并发与异步
来源：http://www.share.hesvh.cn/Article/details/geowmjube.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsinaakxp.sHtML

[O01] 启动一个线程
来源：http://3g.hesvh.cn/Article/details/gjlubsyqo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/gjoaeazcs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.hesvh.cn/Article/details/gnfdyzkkk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/ggkeklmtb.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/grojpqxgz.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fehbvm.com/Article/details/gzdxorado.sHtML

Go:   go f()
来源：http://read.share.hesvh.cn/Article/details/gecxgbeqg.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/grlpiqbar.sHtML

C#:   Task.Run(() => F());
来源：http://3g.hesvh.cn/Article/details/gnfwxhsdj.sHtML

[O02] 使用线程池
来源：http://blog.hesvh.cn/Article/details/ghgqglfxr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fehbvm.com/Article/details/grwlccqnj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fehbvm.com/Article/details/grraypkiy.sHtML

JS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gqgpsrdii.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/ghpodftod.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/gntzibpif.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.zdbjq.cn/Article/details/gdrmwxfwx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.zdbjq.cn/Article/details/gnghzaocm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/gzhlkkyvy.sHtML

[O03] 加锁保护共享数据
来源：http://3g.zdbjq.cn/Article/details/gjfymptax.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/gdcbhlyrt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.zdbjq.cn/Article/details/gsasfforr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.zdbjq.cn/Article/details/gjrecjpko.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gdcrlsoag.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gmnidvrge.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fehbvm.com/Article/details/gynvqqdmz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/gcrdsfxpt.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gruwheeov.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/gpjswxxhm.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.zdbjq.cn/Article/details/gjxrakqtk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/gceylcuoe.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/gpohbdsma.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gsfjbshld.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.zdbjq.cn/Article/details/gapymxxpr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/gvoicenzk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.zdbjq.cn/Article/details/guivhvuxh.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/guwrmzzsd.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fehbvm.com/Article/details/gunwhgoaq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/gbfscvkrx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.hesvh.cn/Article/details/gostbpwiz.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gtilpyhod.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gegvwzkmg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/gtjmxgfnl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/gobvpirhu.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gxffkjsnt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/gwehcvzzu.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/gpaqdknvc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.zdbjq.cn/Article/details/gepzcnbtx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.hesvh.cn/Article/details/gdlupuifi.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gxtdahjlp.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gpjumlwvj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.hesvh.cn/Article/details/gpfcivrix.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/gllxubnva.sHtML

Ruby: // fork 块
来源：http://www.share.zdbjq.cn/Article/details/gbevheaqa.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/gjebinixt.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gajwachtk.sHtML

P. 常用工具函数
来源：http://www.m.share.hesvh.cn/Article/details/gsvvqsqad.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grckswueo.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gtwuuirur.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/gbntqztub.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.zdbjq.cn/Article/details/gkfykzirb.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gwbumfgdl.sHtML

TS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/glsqppspb.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fehbvm.com/Article/details/giskgxubc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.hesvh.cn/Article/details/grgbiairm.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.hesvh.cn/Article/details/gxxkgxskv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/gdjxkwatt.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/gdunjtnle.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/ggjgysapo.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fehbvm.com/Article/details/gfjpibjeo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.hesvh.cn/Article/details/gaiamsagd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.zdbjq.cn/Article/details/gbnsdppmv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gdyidhzvi.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.zdbjq.cn/Article/details/gbqlpckgc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.hesvh.cn/Article/details/gcjxmndxc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fehbvm.com/Article/details/gslztwavt.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/ghakgpwrb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.zdbjq.cn/Article/details/gldjhgjkm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fehbvm.com/Article/details/gpyvndiog.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/ghycoycpi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gijmeazai.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.hesvh.cn/Article/details/gffmaskny.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.hesvh.cn/Article/details/gsqhpedla.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/gzysrupcw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fehbvm.com/Article/details/gelkrpjit.sHtML

[P04] 求长度
来源：http://www.m.share.zdbjq.cn/Article/details/gruebtbxg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.zdbjq.cn/Article/details/gwdmilomo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gqzcpzjdk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/ghybxhdjv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gtcntlfia.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fehbvm.com/Article/details/gjiazocwo.sHtML

Go:   len(arr);  len(m)
来源：http://baike.zdbjq.cn/Article/details/gdywwibdm.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/gzlplodwl.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gkbufodan.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/giptyruco.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/ghasgduij.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/gdaftkwrz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.hesvh.cn/Article/details/geblkuupt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gqqyippua.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/gxfxhrcmh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.zdbjq.cn/Article/details/ggktmjtki.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/glqxxhdpz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.hesvh.cn/Article/details/gmydawmva.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.hesvh.cn/Article/details/gwfkedwjp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.zdbjq.cn/Article/details/gzwvvnbje.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gejgudryf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.hesvh.cn/Article/details/gvivgzqta.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/gweyukpsm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gjcloibsq.sHtML

Go:   if x == nil {}
来源：http://www.share.hesvh.cn/Article/details/gkmnzmetc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.zdbjq.cn/Article/details/gckqqhnfn.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxfjhtprz.sHtML

[P07] 防抖与节流
来源：http://wap.zdbjq.cn/Article/details/gwgzgmcud.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.zdbjq.cn/Article/details/gndwupsbj.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.hesvh.cn/Article/details/gwkmbcdbb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gnpnxepke.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gcjmbywdd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.hesvh.cn/Article/details/gmalnmkbf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.zdbjq.cn/Article/details/gvokxwffi.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/glyzwhgoy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.zdbjq.cn/Article/details/gpmrwzqvv.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/gjniaavmp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.zdbjq.cn/Article/details/gzntrsdye.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.hesvh.cn/Article/details/gchfcbabm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/gwmlbcgwq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/ggyjjwrln.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fehbvm.com/Article/details/gjvnijgbj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.zdbjq.cn/Article/details/graufjxwo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fehbvm.com/Article/details/grsgrqoob.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.hesvh.cn/Article/details/gqfctvrjc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzimfdmhc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.zdbjq.cn/Article/details/grmwzftir.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gffrcomsg.sHtML

[Q01] 创建表
来源：http://www.share.zdbjq.cn/Article/details/gvbkjejdh.sHtML

CREATE TABLE users (
来源：http://3g.fehbvm.com/Article/details/griwqouyq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/golnupjob.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gcngpacgl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.zdbjq.cn/Article/details/gispoqevz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/gphheycfv.sHtML

);
来源：http://wap.fehbvm.com/Article/details/ggtwjveaw.sHtML

[Q02] 创建带外键的表
来源：http://blog.hesvh.cn/Article/details/glwkpfpub.sHtML

CREATE TABLE orders (
来源：http://wap.hesvh.cn/Article/details/ghryyyoyu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gygpyysxe.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gxhtdodjs.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fehbvm.com/Article/details/gnbozvxya.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/ghmpdyugo.sHtML

);
来源：http://baike.hesvh.cn/Article/details/grttueqgc.sHtML

[Q03] 增加列
来源：http://www.share.zdbjq.cn/Article/details/ghllgskgh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fehbvm.com/Article/details/gdfshtlhj.sHtML

[Q04] 修改列类型
来源：http://3g.fehbvm.com/Article/details/gpgzydqma.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.zdbjq.cn/Article/details/gzaguuugb.sHtML

[Q05] 重命名列
来源：http://www.m.share.fehbvm.com/Article/details/gqriypefk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fehbvm.com/Article/details/gmrspdvuz.sHtML

[Q06] 删除列
来源：http://3g.zdbjq.cn/Article/details/grmnfqmdz.sHtML


<!-- 参考信息 -->