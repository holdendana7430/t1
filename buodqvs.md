代发 wailian999

JS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/grgtdeylk.sHtML

TS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gorjbxucr.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/gjzjhgopz.sHtML

Go:   os.Exit(1)
来源：http://3g.hesvh.cn/Article/details/gcyfblumu.sHtML

Ruby: exit 1
来源：http://blog.zdbjq.cn/Article/details/goplyejii.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fehbvm.com/Article/details/gyaaivbho.sHtML

[M06] 向标准错误输出
来源：http://read.share.zdbjq.cn/Article/details/gxwjafujd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gjdvwbnnn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.zdbjq.cn/Article/details/gfnnciuag.sHtML

JS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gyzjgnoof.sHtML

TS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gpkkhgbem.sHtML

Java: System.err.println("err")
来源：http://www.share.hesvh.cn/Article/details/glkiyfrko.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/gdkentoon.sHtML

Ruby: warn "err"
来源：http://www.share.zdbjq.cn/Article/details/gozyuaxgj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.hesvh.cn/Article/details/gxbazsssc.sHtML

[M07] 判断是否为主入口
来源：http://read.share.hesvh.cn/Article/details/gnnpknfwm.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/ggsrdccsx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.zdbjq.cn/Article/details/ggirsplil.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gcwqnjfzw.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gdscywtqk.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/gxyquexbd.sHtML

Go:   func main()
来源：http://www.blog.zdbjq.cn/Article/details/gpmofaeel.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.zdbjq.cn/Article/details/gbagfhapw.sHtML

C#:   static void Main(string[] args)
来源：http://3g.hesvh.cn/Article/details/gxrabcccz.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.zdbjq.cn/Article/details/gaswgrqao.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/ggbljmwbv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.hesvh.cn/Article/details/gksunriro.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gotsqtnpo.sHtML

TS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gwfdggshc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.hesvh.cn/Article/details/gdwbakank.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/gluighjik.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/giitdizbk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.hesvh.cn/Article/details/guyuxiyrp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbjbyfrtd.sHtML

N. 数据结构与算法
来源：http://read.share.hesvh.cn/Article/details/ggnsoqzdc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gpwyxxhsd.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/gsdocineq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gzyahnkrn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.hesvh.cn/Article/details/giafixguc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/ggdbytpld.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gjlptlmeu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gnsbnsrxb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gwjdictrv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/gbmwdchpa.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gaxuzsbpx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.hesvh.cn/Article/details/geboeqyjn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gyivcljmz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fehbvm.com/Article/details/gefxyzssd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gkoupkplq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gvqghnezu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fehbvm.com/Article/details/glpofikwm.sHtML

Go:   slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gsedxhtum.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gtjyhgyim.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/gdkzwnnyr.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/gxkgqjobk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fehbvm.com/Article/details/gqjtkielo.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.zdbjq.cn/Article/details/gcwzcfzeu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gxxrncnmr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gvtzzjqig.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/gqveneskt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/gphlcghwt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.hesvh.cn/Article/details/gmymowdlo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.hesvh.cn/Article/details/gmulocqny.sHtML

[N04] 斐波那契数列
来源：http://mobile.hesvh.cn/Article/details/gljnhjpqi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gzyvosbyo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gyaatpttn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gxczemyyu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gstohxgsa.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/gdowwkbnr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fehbvm.com/Article/details/gwonznfue.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gkvgvenbv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gmcqmhklv.sHtML

[N05] 最大公约数
来源：http://www.m.share.fehbvm.com/Article/details/gabtfkeqc.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gswgqyyzq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.zdbjq.cn/Article/details/gythfmznc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/grazbhisb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gzyyvmsjb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fehbvm.com/Article/details/gbvtlpjmi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.zdbjq.cn/Article/details/gtrcfntbu.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/gtpxywmvq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/gbgepfiuv.sHtML

[N06] 判断回文字符串
来源：http://blog.zdbjq.cn/Article/details/gpbxkoovq.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/gbhzdxatm.sHtML

PHP:  $s === strrev($s);
来源：http://wap.zdbjq.cn/Article/details/giiwqegbg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gampgjovf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gyhswrtaz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.zdbjq.cn/Article/details/gkltoqrje.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/gxmuqqclr.sHtML

Ruby: s == s.reverse
来源：http://3g.zdbjq.cn/Article/details/gfqyrpcqd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/ghchtpaha.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fehbvm.com/Article/details/gjymgnpkf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/gfuueatko.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.zdbjq.cn/Article/details/gmspjmbfb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fehbvm.com/Article/details/gkfxwiaws.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.hesvh.cn/Article/details/gimostnmq.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/gwjrkrvep.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.hesvh.cn/Article/details/gduxokfic.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/gqjmfnhxf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fehbvm.com/Article/details/gwzrualnl.sHtML

[N08] 生成全排列
来源：http://wap.hesvh.cn/Article/details/gvednbdfb.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/gnjjghbup.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/gadzpyzvn.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gpehggezg.sHtML

TS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gdilayutd.sHtML

Java: // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gwozysxsc.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/ghywhjodf.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.hesvh.cn/Article/details/gkkkwguil.sHtML

C#:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gkvmovpho.sHtML

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/gtrupbngs.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fehbvm.com/Article/details/gjrjdiaqg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gxmfwvcfm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gvzbdlukw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fehbvm.com/Article/details/glnowaluh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.zdbjq.cn/Article/details/gjtyinaiv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.zdbjq.cn/Article/details/gfdtvycme.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gzdfxnpjz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.zdbjq.cn/Article/details/giuuldzdf.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/gbibgyter.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fehbvm.com/Article/details/gfxvaoeeg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.hesvh.cn/Article/details/guhxrwvwk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.hesvh.cn/Article/details/gtifqlpds.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fehbvm.com/Article/details/gcxabwgmv.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/gfteptrlz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fehbvm.com/Article/details/gloqbllmc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/gthtvmgql.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fehbvm.com/Article/details/gaekmpahe.sHtML

[N11] 二叉树中序遍历
来源：http://wap.hesvh.cn/Article/details/glamkotbq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/grfdslugz.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.zdbjq.cn/Article/details/gmmrkiozo.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gkwrbzjip.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gkcljslbc.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gvpqnziax.sHtML

Go:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/glnmaciny.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.zdbjq.cn/Article/details/gkauzpipf.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gpdwnglip.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.zdbjq.cn/Article/details/gvlovsuoy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.zdbjq.cn/Article/details/gsbmblcpg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/gfvkeyrke.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gnueokhlj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gqyhlxuth.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gglxrqwsx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fehbvm.com/Article/details/glmbbmvqc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gvnyoeczk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gqkiakynn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzhlsoubv.sHtML

O. 并发与异步
来源：http://baike.fehbvm.com/Article/details/gzgogtnmf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmkoggasi.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/gaqdtbxaz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fehbvm.com/Article/details/gfewkvaqp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.hesvh.cn/Article/details/giurqwuhx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/gsocdqgeb.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/ghitblrin.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.hesvh.cn/Article/details/guglamkdg.sHtML

Go:   go f()
来源：http://www.blog.fehbvm.com/Article/details/gzleaqalu.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.hesvh.cn/Article/details/gsulgxcds.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/gxtliwwbe.sHtML

[O02] 使用线程池
来源：http://wap.hesvh.cn/Article/details/gljvcpnok.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fehbvm.com/Article/details/gqmzawlgb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fehbvm.com/Article/details/grmwfeotm.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gsgrsmxup.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gzolcailj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.zdbjq.cn/Article/details/giauzmwnd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.hesvh.cn/Article/details/gvplkjuym.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gihvuwuag.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fehbvm.com/Article/details/gxljcnojp.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/gamfhrfsh.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.hesvh.cn/Article/details/gtxzepdmf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.zdbjq.cn/Article/details/gxzqgliix.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.hesvh.cn/Article/details/gdmjgbako.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gkpjqrqks.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gywbageyy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/gugqbrbmp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.zdbjq.cn/Article/details/gcxvgsbri.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gmzooowxi.sHtML

[O04] 定义异步函数并等待
来源：http://baike.zdbjq.cn/Article/details/guinezcze.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fehbvm.com/Article/details/gspudlcuq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.hesvh.cn/Article/details/giyvuymcf.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/grxdyitzy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/gweabhgwa.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fehbvm.com/Article/details/gsudsdrwt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fehbvm.com/Article/details/gcafprqkm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/gqthhiqec.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.zdbjq.cn/Article/details/gcppubhkc.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.zdbjq.cn/Article/details/gwsnovbrf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.zdbjq.cn/Article/details/gkudiuglm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/guodfhbwq.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gqfrfjxzo.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/grcgotyst.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fehbvm.com/Article/details/gioyoypiu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.zdbjq.cn/Article/details/gehfhfxbx.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gagrbuvpg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.hesvh.cn/Article/details/gwznespok.sHtML

[O06] 使用进程池
来源：http://www.m.share.fehbvm.com/Article/details/gqnobgmac.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fehbvm.com/Article/details/gotgwnyfh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.zdbjq.cn/Article/details/gxmqofudn.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gibsqbuse.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gmnylybbe.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.hesvh.cn/Article/details/gghtpukyo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.hesvh.cn/Article/details/gjcqyabbk.sHtML

Ruby: // fork 块
来源：http://m.share.hesvh.cn/Article/details/gsnrfactb.sHtML

C#:   Parallel.For
来源：http://baike.zdbjq.cn/Article/details/gxnziducu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gnfxfcdpq.sHtML

P. 常用工具函数
来源：http://wap.fehbvm.com/Article/details/gjanhbmzp.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gomcnokmq.sHtML

[P01] 生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/glsaqmapd.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/gybafoglo.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.hesvh.cn/Article/details/gaszkebbe.sHtML

JS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gselotgzx.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gtzmkxegm.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/glmvziute.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.hesvh.cn/Article/details/gkrdbzlrx.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/gpluqykgv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.hesvh.cn/Article/details/gdalsysiq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/gvkjoukqf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fehbvm.com/Article/details/gfdcyceqx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.hesvh.cn/Article/details/gaipmifkq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.hesvh.cn/Article/details/gweuifxiy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/gmheorres.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.zdbjq.cn/Article/details/gqzescndl.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.fehbvm.com/Article/details/gpkicbqmw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/gcnqwdoac.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/ggysvvjdu.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/gqnyatlpm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.zdbjq.cn/Article/details/gydapgsad.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fehbvm.com/Article/details/gwwemtgsu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gerjpkgut.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gzzcnfeku.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fehbvm.com/Article/details/gwbfhzudp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.hesvh.cn/Article/details/gagldqhjp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/gxeppiobm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.zdbjq.cn/Article/details/gyodfgumj.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/gksfvadok.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/gdplahtct.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gsfeotsgz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gubjmexsz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gufouqost.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/gtabpohwz.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.zdbjq.cn/Article/details/gkkvohjey.sHtML

Ruby: x.length;  x.size
来源：http://blog.hesvh.cn/Article/details/glidomxmv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/gaugrobba.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/gioaaznst.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/gvaptaopn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.hesvh.cn/Article/details/gaqmnoimz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.zdbjq.cn/Article/details/gebackwra.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gevxdiuqe.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/gxpmokkql.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gkrurhiqy.sHtML

Ruby: a == b
来源：http://read.share.zdbjq.cn/Article/details/gvnbstdlt.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.hesvh.cn/Article/details/ggyqehfza.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/grxjbdlrb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.zdbjq.cn/Article/details/gtqkmctjh.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.zdbjq.cn/Article/details/gijtgvcvd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fehbvm.com/Article/details/gftrcgpng.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gujjwdqww.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gqoedhnzz.sHtML

Go:   if x == nil {}
来源：http://baike.fehbvm.com/Article/details/gblmakupd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fehbvm.com/Article/details/gnrfvdfyp.sHtML

C#:   if (x is null) {}
来源：http://3g.zdbjq.cn/Article/details/ggsspuxoi.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/gtlqowqor.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/gvrzjddpj.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.zdbjq.cn/Article/details/gltzevsim.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gzezcyggf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gsndvvgvd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.zdbjq.cn/Article/details/guwwaodhh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/gobgfbupd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fehbvm.com/Article/details/gimpqdwue.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.zdbjq.cn/Article/details/gxzbpuzeb.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/gipvvhuah.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.hesvh.cn/Article/details/gbpqxmiqp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/gnshklqbn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.hesvh.cn/Article/details/ghpnynbpp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/gcsqhwhcr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.zdbjq.cn/Article/details/gjzznkmdj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.zdbjq.cn/Article/details/ghvkyyciy.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fehbvm.com/Article/details/gicjsluun.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fehbvm.com/Article/details/geplwgwik.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxqrahugg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.zdbjq.cn/Article/details/gvljzwery.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gpyelwrfr.sHtML

[Q01] 创建表
来源：http://m.share.hesvh.cn/Article/details/gnxjdhwrx.sHtML

CREATE TABLE users (
来源：http://mobile.hesvh.cn/Article/details/gvdepzgch.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gshqxcoqn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gdbrwxfco.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fehbvm.com/Article/details/goduwmkti.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/goqrlggmk.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/glcojpjrg.sHtML

[Q02] 创建带外键的表
来源：http://wap.hesvh.cn/Article/details/grhasgrfe.sHtML

CREATE TABLE orders (
来源：http://m.share.hesvh.cn/Article/details/gwsycodoo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/glihczken.sHtML

user_id INT NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gdxtpbdlt.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/gpfmjqcaz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/gnlwtyyqa.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gkxdrxhru.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/gxzpzwsny.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.zdbjq.cn/Article/details/gdnwqpzef.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/gfldlsvlj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.zdbjq.cn/Article/details/gigpvhqwa.sHtML

[Q05] 重命名列
来源：http://3g.fehbvm.com/Article/details/gjwqcojdf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.zdbjq.cn/Article/details/gjvraewmv.sHtML

[Q06] 删除列
来源：http://www.blog.fehbvm.com/Article/details/gpvaojssb.sHtML


<!-- 参考信息 -->