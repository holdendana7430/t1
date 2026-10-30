代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.hesvh.cn/Article/details/ggetoewlp.sHtML

[M05] 设置退出码
来源：http://baike.zdbjq.cn/Article/details/gcwrbdvix.sHtML

Py:   sys.exit(1)
来源：http://baike.fehbvm.com/Article/details/gkumddvxy.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/guktzdqkx.sHtML

JS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gkqldhfmn.sHtML

TS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/giomvdihm.sHtML

Java: System.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gpxxsrogi.sHtML

Go:   os.Exit(1)
来源：http://mobile.fehbvm.com/Article/details/gaoesocrt.sHtML

Ruby: exit 1
来源：http://baike.fehbvm.com/Article/details/gikgpjdzb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.zdbjq.cn/Article/details/girvmzegy.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/gdpwzixra.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/ggnehjbza.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/gelhjeonb.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gliuoswir.sHtML

TS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gyjywwjoo.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gollmltpi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fehbvm.com/Article/details/gisjqcyja.sHtML

Ruby: warn "err"
来源：http://m.share.fehbvm.com/Article/details/gjgminfxo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/gcpslnlmi.sHtML

[M07] 判断是否为主入口
来源：http://3g.fehbvm.com/Article/details/gdwctrppv.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/gaekdgycu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/gmclitxuj.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gskpepvrl.sHtML

TS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gybbbnzwp.sHtML

Java: public static void main(String[] args)
来源：http://wap.fehbvm.com/Article/details/glyosfber.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/gtudpfqut.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fehbvm.com/Article/details/ggarewvrq.sHtML

C#:   static void Main(string[] args)
来源：http://baike.hesvh.cn/Article/details/gioufrdmw.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gpdmyngdj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/gdektuwcx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/gbunfuadr.sHtML

JS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gltnqjcqw.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/giajtcjlg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.hesvh.cn/Article/details/gcyfltydq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.zdbjq.cn/Article/details/gweflxzwm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.hesvh.cn/Article/details/gwnqwxjur.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/gzxswdwrw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gynvsbfjs.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/gbkcvmghj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbxfolijx.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/glyeygwsa.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gjxtnorct.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.hesvh.cn/Article/details/ghdpqidot.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gueobpmwl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gbtlynnww.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gvkizcnmm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gflpysqth.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.zdbjq.cn/Article/details/gdkyqprwb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gpufbttca.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/gocchetly.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gtodyqkwe.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/ghktguzgu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gjotkqedp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gnjsvihmx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/gtiqowhrj.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gizatlzjj.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gmsntpqky.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fehbvm.com/Article/details/ggsmooopj.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.hesvh.cn/Article/details/glmznypek.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fehbvm.com/Article/details/gkrxojtxx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fehbvm.com/Article/details/gswusmnlb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gqajbvmhz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gcgrdyqle.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.hesvh.cn/Article/details/gnbosdyrp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/grbxzpzcj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/guugyxhfh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/ghtlkcrnj.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/gsjmrkmcj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gvowcbgfv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fehbvm.com/Article/details/gvpjxnlum.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gvilpmdzb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/ghhskakcl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gvabbryxc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/gfvzuptxt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/ggaenkfta.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/ghivsbksq.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/gnclwjosx.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gghjsdmld.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/garencfff.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gyocmvlan.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gdzueobxj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/guswvruoh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fehbvm.com/Article/details/gjvxbfnnf.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/gyiejzhxq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/gexdtxmlk.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/geilfxqzs.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gyincdini.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gaofnrfhg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gqcrmbwfw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/guhjgitjo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/gxzkibrhb.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.zdbjq.cn/Article/details/gqaphzcxe.sHtML

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/gbvhkugda.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gdusdoraw.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.hesvh.cn/Article/details/gsaquimlu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/gavhaxsks.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/gulkhwypw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.hesvh.cn/Article/details/gqsbjrohk.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/gtyoapjqf.sHtML

Java: // 手写 HashMap
来源：http://baike.fehbvm.com/Article/details/gshidknpw.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.fehbvm.com/Article/details/geoukpfkw.sHtML

Ruby: // 手写 Hash
来源：http://baike.hesvh.cn/Article/details/gsacjcdcb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/gsdirowas.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/gsvywgymd.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gfsmyfmgo.sHtML

PHP:  // 手写递归交换
来源：http://read.share.hesvh.cn/Article/details/gcamjdhlr.sHtML

JS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gahxuzjai.sHtML

TS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gbuqtvygp.sHtML

Java: // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/glvbghsxf.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gjtldqkon.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/gclllzpif.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/goxsrdydv.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gwpugqdqj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.hesvh.cn/Article/details/gpbyodenh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gywmfkvym.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gpomlbeem.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fehbvm.com/Article/details/gjxamuvvq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/gkphdmmou.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/gpurwooul.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gegqcumuc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.zdbjq.cn/Article/details/gqvipnczr.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gikqutvea.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/grwgtfmym.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.hesvh.cn/Article/details/gfrdhdbhh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.hesvh.cn/Article/details/gndwggqln.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.hesvh.cn/Article/details/gepxtofhj.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsldmibng.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.zdbjq.cn/Article/details/glnlispxc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.zdbjq.cn/Article/details/gzvybkdot.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/glbfvnjxd.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fehbvm.com/Article/details/gkzhjlxkt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/gnluisfgk.sHtML

PHP:  // 手写递归函数
来源：http://blog.hesvh.cn/Article/details/grvklsqff.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gjzswgspm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gtzbeusxd.sHtML

Java: // 手写递归
来源：http://baike.fehbvm.com/Article/details/gjlocuvdl.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gkyqcdhev.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.zdbjq.cn/Article/details/gnuktzqtb.sHtML

C#:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gllkuilrv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.hesvh.cn/Article/details/ggrdmmmtw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/gmufwjhjp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.hesvh.cn/Article/details/gbopvleuz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gitwstcju.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gsstiimzt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/ggoffcyop.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fehbvm.com/Article/details/glakjqjze.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.hesvh.cn/Article/details/ggepdhidv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gvpyriirm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gaulwbhzt.sHtML

O. 并发与异步
来源：http://mobile.fehbvm.com/Article/details/geiotnwez.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpeyakajy.sHtML

[O01] 启动一个线程
来源：http://mobile.hesvh.cn/Article/details/gslvsgxyr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.hesvh.cn/Article/details/gigwjxozz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.hesvh.cn/Article/details/gtysprpnt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.zdbjq.cn/Article/details/gjykmrvta.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/ghkgkzads.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.hesvh.cn/Article/details/gpaouirls.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/gqoknsfyk.sHtML

Ruby: Thread.new { f }
来源：http://www.share.zdbjq.cn/Article/details/gwcnxvuwx.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/gnwiaeuny.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/glzflyuwl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.zdbjq.cn/Article/details/gphforven.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/gombzterz.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/grwblbmrx.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gqafktbuz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fehbvm.com/Article/details/gucoogjhm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/geonwkbyy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gejvlijfc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/gqkhwtbfo.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/glnquahfm.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/gxuejviyq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.zdbjq.cn/Article/details/geauvrozk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.zdbjq.cn/Article/details/gqgmkbpxu.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gdniwhxia.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gwsotqukx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/gbrnmpnqf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/ghevcnvws.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gobxcueek.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.hesvh.cn/Article/details/gdvoftyyl.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.zdbjq.cn/Article/details/griwhnqaw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/gigvjdnzi.sHtML

JS:   async function f() { await g(); }
来源：http://wap.hesvh.cn/Article/details/govhcyzjx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gduczeyem.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fehbvm.com/Article/details/ggotgvjaa.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fehbvm.com/Article/details/gubyqzyof.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.zdbjq.cn/Article/details/goyzyuems.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.hesvh.cn/Article/details/gofrmoqxa.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/gelyzltmu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.hesvh.cn/Article/details/glaubdkff.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fehbvm.com/Article/details/gduwozuuc.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gqulgzpyl.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gwlegncgd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fehbvm.com/Article/details/gqelgtowv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.hesvh.cn/Article/details/gptkzgafn.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fehbvm.com/Article/details/gdookyegu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fehbvm.com/Article/details/gechlhptt.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/gkdxesfpw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.hesvh.cn/Article/details/gxjyagkgv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fehbvm.com/Article/details/glrhrvkrp.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gkxrvglcy.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gzkugnpzu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/ganeiabez.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/guxrfwqth.sHtML

Ruby: // fork 块
来源：http://3g.zdbjq.cn/Article/details/gjplvvxlg.sHtML

C#:   Parallel.For
来源：http://wap.fehbvm.com/Article/details/gqfjkfowa.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbglcnqci.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/gqzobglwt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gsnntwajg.sHtML

[P01] 生成 UUID
来源：http://baike.zdbjq.cn/Article/details/ghcjstidg.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fehbvm.com/Article/details/guemayugg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gjvbdajza.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gauyyoltu.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gwiliiujy.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.zdbjq.cn/Article/details/gznrzuvbk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/gojvqtlzb.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fehbvm.com/Article/details/gepdhwrjz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fehbvm.com/Article/details/gldszupec.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fehbvm.com/Article/details/guawxratd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.hesvh.cn/Article/details/gmakdomxh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/giimnlqkz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.zdbjq.cn/Article/details/gqalgoqem.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.hesvh.cn/Article/details/gwvkcmaif.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.hesvh.cn/Article/details/gvxleblej.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gsymkqqmh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.hesvh.cn/Article/details/gfxtvmbjv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.hesvh.cn/Article/details/gmrwrdafw.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/gcxgwaspa.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.hesvh.cn/Article/details/gfwjcfddv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fehbvm.com/Article/details/ggbkahejn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gknyzrfsh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gxcutvhzs.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.hesvh.cn/Article/details/gemxpwzyg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.hesvh.cn/Article/details/gasbiemfw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/ghxvdxbpn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.hesvh.cn/Article/details/gcaefvdgq.sHtML

[P04] 求长度
来源：http://www.share.fehbvm.com/Article/details/gagktfwmk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gsxsvwull.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gixthlzet.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gazlezkhw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gflchjumt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/ghelljosh.sHtML

Go:   len(arr);  len(m)
来源：http://baike.hesvh.cn/Article/details/gswathctv.sHtML

Ruby: x.length;  x.size
来源：http://m.share.zdbjq.cn/Article/details/gnbkdktcb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gyilfgviv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.fehbvm.com/Article/details/gagaevyds.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.hesvh.cn/Article/details/gbvujxhld.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.hesvh.cn/Article/details/gfpxbmfrd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fehbvm.com/Article/details/gkcrrmehs.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gqlfbnmvj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.zdbjq.cn/Article/details/grojkutlb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fehbvm.com/Article/details/gxqilftie.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/gdwnzhqze.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.hesvh.cn/Article/details/giyahxhpv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.hesvh.cn/Article/details/geaszwczk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fehbvm.com/Article/details/gtdmsngjx.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fehbvm.com/Article/details/gdxisfurx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fehbvm.com/Article/details/gkszrpnbk.sHtML

TS:   if (x == null) {}
来源：http://read.share.fehbvm.com/Article/details/grlzuuoum.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/ggswowqkq.sHtML

Go:   if x == nil {}
来源：http://wap.fehbvm.com/Article/details/gzzfjuzvy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.hesvh.cn/Article/details/gknarmwuk.sHtML

C#:   if (x is null) {}
来源：http://mobile.hesvh.cn/Article/details/guvlztgtd.sHtML

[P07] 防抖与节流
来源：http://www.m.share.zdbjq.cn/Article/details/gcsslyzkc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.zdbjq.cn/Article/details/ggidxcoqx.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.zdbjq.cn/Article/details/gktwukmth.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/ggumajamc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gihwtukim.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/gejgyafkl.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.hesvh.cn/Article/details/gsuapuihh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fehbvm.com/Article/details/gqqkfeobj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.hesvh.cn/Article/details/gfqernidw.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/ghynukmpy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fehbvm.com/Article/details/ghzancbyp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/gqowwljco.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fehbvm.com/Article/details/gdhwgjkxt.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/gonhbgqpd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/gtcnkrlwe.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gckgsdvyz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.hesvh.cn/Article/details/gvyyrupkj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.hesvh.cn/Article/details/gawblbjen.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzlbijfsy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.hesvh.cn/Article/details/genmbcwvb.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvkfqfyej.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/glwxlrgnp.sHtML

CREATE TABLE users (
来源：http://www.share.fehbvm.com/Article/details/gicplmtbu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gxarkbkbe.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/gwaaoblqf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.zdbjq.cn/Article/details/gikrowydd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.hesvh.cn/Article/details/gxvtkbern.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gejwocrhw.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fehbvm.com/Article/details/gunigkjki.sHtML

CREATE TABLE orders (
来源：http://read.share.zdbjq.cn/Article/details/gosltjxhy.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gyqdjhsdh.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gdswnzzjx.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.hesvh.cn/Article/details/gapyxjtoo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.hesvh.cn/Article/details/gjgenrpyj.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gzvnpbwsc.sHtML

[Q03] 增加列
来源：http://read.share.hesvh.cn/Article/details/gufcjugof.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.zdbjq.cn/Article/details/glgyzwlof.sHtML

[Q04] 修改列类型
来源：http://baike.zdbjq.cn/Article/details/guuvnmaef.sHtML


<!-- 参考信息 -->