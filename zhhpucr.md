代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.hesvh.cn/Article/details/gagidhclq.sHtML

[M05] 设置退出码
来源：http://mobile.zdbjq.cn/Article/details/gkunoevsd.sHtML

Py:   sys.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gycoajksy.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/gaqigyzjz.sHtML

JS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/ggcoyrlhg.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gucyyjenv.sHtML

Java: System.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gljogzjfi.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/gubkafwvo.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gufwwklyn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.hesvh.cn/Article/details/ghllzamew.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/gjkeghjkw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gayzuedsq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.zdbjq.cn/Article/details/gmzanzvid.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gugsgiict.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gsmqshphu.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/gwzyqcxun.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/gebzqfcuc.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/gwqpmladk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/gafjiwfcj.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.zdbjq.cn/Article/details/gfuildsde.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fehbvm.com/Article/details/gmibhwsnu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/gdwvaskbq.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gsmzewszr.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gqpjwtwxf.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/gclvryzil.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/gqsepiqcf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.hesvh.cn/Article/details/gyjbvmkog.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fehbvm.com/Article/details/gymglnuvh.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.hesvh.cn/Article/details/gukizgyos.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fehbvm.com/Article/details/gehkhnpgv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.hesvh.cn/Article/details/ghvejovjd.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gbcwvleaf.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gvgfnpkfe.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/grzhbuare.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/gudjozivx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.zdbjq.cn/Article/details/ghfdhgioh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/guhqkmazk.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkqabjtsq.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/gbnpyasez.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtqdewiwl.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/gupmzyswx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/gdcbfdcps.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gmhnejfpa.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gpqsppbru.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gfhzpyrzs.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gyvujjbao.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gkjcgmqdu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gyszsrxmi.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gmdjhaeep.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/ggsrjbbaw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/ghvhiffue.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fehbvm.com/Article/details/gskvkihqy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gpqlgfwrs.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gisqsojfo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/goqvliwsf.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/grjnyegtx.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gqnocsnzc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fehbvm.com/Article/details/gdqpmpmsb.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.hesvh.cn/Article/details/gaoqtlxww.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/gjxhwwjex.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.zdbjq.cn/Article/details/gypjbtmdt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/grixdpziz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gxsaduyax.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/gxbcgbsdo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/gxymdyjuy.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fehbvm.com/Article/details/gdzhaypqw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gbvrpvatv.sHtML

[N04] 斐波那契数列
来源：http://www.blog.zdbjq.cn/Article/details/gubfglrff.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/ghohdchse.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fehbvm.com/Article/details/gjqmdyfri.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gtrabftsc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gnwqttolf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gzsppixzu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/ggduvzjgh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/giajupjkv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gfyokqgbi.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/gncvtmzxs.sHtML

Py:   math.gcd(a, b)
来源：http://wap.zdbjq.cn/Article/details/gpxkgghvp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/ghmkfxtsn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gwrfqkaav.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gxuqdhrxz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/gssxpqdtc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/gkqxhwzeg.sHtML

Ruby: a.gcd(b)
来源：http://wap.hesvh.cn/Article/details/glhfiuuch.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.zdbjq.cn/Article/details/ggjnjgqow.sHtML

[N06] 判断回文字符串
来源：http://blog.zdbjq.cn/Article/details/gqvcbsiyu.sHtML

Py:   s == s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gkzaomual.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gshemwfjg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gztxciedq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gypzohztc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.hesvh.cn/Article/details/gojnihutr.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fehbvm.com/Article/details/gajspkyrc.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gaschyfqz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gqgzwgqfx.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/gjdvskvwi.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gdrjqbmbw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.hesvh.cn/Article/details/gqvclrkls.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/gbeaghfoa.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/gvgokdgqb.sHtML

Java: // 手写 HashMap
来源：http://blog.hesvh.cn/Article/details/gzvcuxjil.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/gckhfuake.sHtML

Ruby: // 手写 Hash
来源：http://wap.hesvh.cn/Article/details/gzmnjywfi.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fehbvm.com/Article/details/gcdxzmfdj.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/ginqacilv.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/ggygyxbir.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/giwwkbgji.sHtML

JS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/grvhuhsbi.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gzasfckih.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gmqurapmb.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gcipvjhyj.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.hesvh.cn/Article/details/ganqjognr.sHtML

C#:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/ggoljuvsr.sHtML

[N09] 栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gmhnptbpy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gwmfxqxzv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gvsniaqmz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/goiklkwko.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/goqpvtwcp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/gpjlqpgaa.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fehbvm.com/Article/details/gylicuoqm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gcnkyoykj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/gcdhikhpp.sHtML

[N10] 链表节点定义
来源：http://blog.hesvh.cn/Article/details/gvsntqmsa.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/gesfyybgv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/gxonylkjb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fehbvm.com/Article/details/gnocuehea.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.hesvh.cn/Article/details/gukccafxu.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/gfhbpidut.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/gmuleenpd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/giarfgjhs.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/gvneltxxq.sHtML

[N11] 二叉树中序遍历
来源：http://3g.hesvh.cn/Article/details/gdhvblutz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/gwsblbhyp.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/gkubttfdg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/groukyizx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gcvpdylla.sHtML

Java: // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gqawsurqp.sHtML

Go:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/glcxnxjab.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.hesvh.cn/Article/details/gpmmrazqi.sHtML

C#:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gxwkntzxe.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/gmhyldmsy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/gjzrudcak.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/gzjmhybrm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/godfsmigv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/ghyjdtxzj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/glkkweril.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.hesvh.cn/Article/details/gvmhyxaox.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/gmqxlvlry.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gvigaaxyf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gaxrdwmhw.sHtML

O. 并发与异步
来源：http://www.share.fehbvm.com/Article/details/gsafxtude.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpogqvmuk.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/gknhaatsx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/gmqkqxedg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fehbvm.com/Article/details/guexpfjql.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.zdbjq.cn/Article/details/gmvdxbjyw.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gelneylzn.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/gvmgetniy.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/gtdtwpdwe.sHtML

Ruby: Thread.new { f }
来源：http://m.share.hesvh.cn/Article/details/gqmpjpqhx.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/gfpdqbxyg.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gjdpvufkj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/gfhvkxolq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.hesvh.cn/Article/details/gvqojwklo.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gamhmbamx.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/grblatiqg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/glirouvmx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.hesvh.cn/Article/details/gyzrhozhq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/gjhlrrpyb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.zdbjq.cn/Article/details/ggtpwwnwm.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/gtbgxnkhb.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fehbvm.com/Article/details/gajfzngad.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fehbvm.com/Article/details/glvuhjatr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.hesvh.cn/Article/details/gxjhonmxm.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gxrdnjaxm.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gppnexrim.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.zdbjq.cn/Article/details/gnxbusybe.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.zdbjq.cn/Article/details/gkgdnxzaw.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gdnedpzex.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.hesvh.cn/Article/details/gdgyzggmc.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.zdbjq.cn/Article/details/gtwrmgzoe.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.zdbjq.cn/Article/details/gayxialde.sHtML

JS:   async function f() { await g(); }
来源：http://wap.hesvh.cn/Article/details/gapfbvlst.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.hesvh.cn/Article/details/gjridurpj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.zdbjq.cn/Article/details/gnzujgkow.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/getmzzmwv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/gkwkpkukm.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.hesvh.cn/Article/details/gmuaahrjy.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.hesvh.cn/Article/details/gfvlwodhr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fehbvm.com/Article/details/grepzxvlg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fehbvm.com/Article/details/gyqivmuuh.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gbqkrtkyl.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gftqiamiu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/gjfzttlcg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.zdbjq.cn/Article/details/gaxzwoyoi.sHtML

Ruby: threads.map(&:join)
来源：http://baike.zdbjq.cn/Article/details/gpcurhfdj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fehbvm.com/Article/details/gohlwwkjx.sHtML

[O06] 使用进程池
来源：http://wap.hesvh.cn/Article/details/gljwmogia.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/gxidiglho.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fehbvm.com/Article/details/gpsaggysz.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gnswyctey.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gpykckzyu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fehbvm.com/Article/details/ggqbocpxl.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.hesvh.cn/Article/details/grdcjjxsl.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/grdohfbca.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/gcgvcfqnu.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gebryjwww.sHtML

P. 常用工具函数
来源：http://m.share.hesvh.cn/Article/details/gwdscyttc.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzzyrcnfb.sHtML

[P01] 生成 UUID
来源：http://baike.fehbvm.com/Article/details/gdhfzmwgn.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/glhawgtis.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/gbasjymru.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gprqrewtw.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gjnsysgja.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fehbvm.com/Article/details/gejvxewij.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.hesvh.cn/Article/details/gpgdqvqsb.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.hesvh.cn/Article/details/grspjweur.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/glvvysrxn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fehbvm.com/Article/details/gjumtnkjm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/gymcwslgl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.zdbjq.cn/Article/details/guxyoyruw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.hesvh.cn/Article/details/gmzxmmvfl.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.zdbjq.cn/Article/details/ggeeiirno.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.zdbjq.cn/Article/details/gvhwstapt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/gpsjwwyun.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fehbvm.com/Article/details/grktflhlo.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/goofkzaup.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/gcvjwdevi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fehbvm.com/Article/details/gusgzlrlg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/gmkkltuqx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gzklztnps.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gqceiyazx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.hesvh.cn/Article/details/gxfozmqop.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/gpddoknor.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.hesvh.cn/Article/details/gfyujupjg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.zdbjq.cn/Article/details/gmoeeggfy.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/gaxodgxpn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/ggmdhgpck.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/guqemcwon.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gsarvirzx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/goiqhslyp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gliqrhetz.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.zdbjq.cn/Article/details/gfvjqivqt.sHtML

Ruby: x.length;  x.size
来源：http://m.share.zdbjq.cn/Article/details/gvsorgowm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.zdbjq.cn/Article/details/glnjvikah.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/glihbaadf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fehbvm.com/Article/details/gqsvqjadq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fehbvm.com/Article/details/gggkflnde.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.hesvh.cn/Article/details/gdflxchdk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gnodfydky.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.hesvh.cn/Article/details/gdamkfiad.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gfrnuioej.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/goilregkp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.zdbjq.cn/Article/details/gxwnjgygo.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/gtkygvgls.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.zdbjq.cn/Article/details/gokfkujxi.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.hesvh.cn/Article/details/gipznxgma.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fehbvm.com/Article/details/gffnqnhyd.sHtML

TS:   if (x == null) {}
来源：http://blog.zdbjq.cn/Article/details/gpwipfpil.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gbphbilpa.sHtML

Go:   if x == nil {}
来源：http://blog.zdbjq.cn/Article/details/gebsmvxfe.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.zdbjq.cn/Article/details/gydibyqpg.sHtML

C#:   if (x is null) {}
来源：http://read.share.hesvh.cn/Article/details/gpcitihpf.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/gpnqmkxbd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/gvwzqlrpv.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.hesvh.cn/Article/details/gmvelzjhw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gfejueniz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gggglatby.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fehbvm.com/Article/details/gwurohsxn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.zdbjq.cn/Article/details/gxcfpumxh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/gttndcayu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.hesvh.cn/Article/details/gnkzipjky.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/gmulxzyxa.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fehbvm.com/Article/details/gtlvndsgy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fehbvm.com/Article/details/gshqroizm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fehbvm.com/Article/details/gpknfycqk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/ghcbwuhwf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.hesvh.cn/Article/details/gfcqnckyv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fehbvm.com/Article/details/gnigvgmzy.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.hesvh.cn/Article/details/gsxqyknhu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fehbvm.com/Article/details/gngieyxrf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtodjlnpx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.hesvh.cn/Article/details/gvfoxgwdd.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfemjfafx.sHtML

[Q01] 创建表
来源：http://m.share.hesvh.cn/Article/details/gzgtmrhfn.sHtML

CREATE TABLE users (
来源：http://mobile.hesvh.cn/Article/details/gaqtynbfi.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gqsckocgq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/geqsoupqe.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/gjnijfeka.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/ggverromf.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gzxqnzxqz.sHtML

[Q02] 创建带外键的表
来源：http://3g.zdbjq.cn/Article/details/gtjsjwcub.sHtML

CREATE TABLE orders (
来源：http://m.share.hesvh.cn/Article/details/gvwlhdjuo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gheolushf.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gvsnhrgze.sHtML

amount DECIMAL(10, 2),
来源：http://wap.zdbjq.cn/Article/details/gxjnwzcwk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/gyrtwxonj.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gnndokhzz.sHtML

[Q03] 增加列
来源：http://blog.hesvh.cn/Article/details/gesrxlozu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/gsptnnqur.sHtML

[Q04] 修改列类型
来源：http://www.blog.zdbjq.cn/Article/details/glgrsvafa.sHtML


<!-- 参考信息 -->