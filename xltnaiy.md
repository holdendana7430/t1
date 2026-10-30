代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/gdtbuuqkl.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/gzdkrculd.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gjbmbqjuz.sHtML

PHP:  exit(1);
来源：http://baike.fehbvm.com/Article/details/gmfiiguax.sHtML

JS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/grzpodzww.sHtML

TS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gxazpzmld.sHtML

Java: System.exit(1)
来源：http://wap.hesvh.cn/Article/details/gxgktegso.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gpuwruzci.sHtML

Ruby: exit 1
来源：http://read.share.zdbjq.cn/Article/details/garcijcor.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/gqtagpdze.sHtML

[M06] 向标准错误输出
来源：http://baike.hesvh.cn/Article/details/gbdnpvnhm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/ghbyzhybs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.hesvh.cn/Article/details/gylpdusuv.sHtML

JS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/ghtlymvrf.sHtML

TS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gffkcfjpu.sHtML

Java: System.err.println("err")
来源：http://mobile.zdbjq.cn/Article/details/gedfabujs.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/guzqgyajb.sHtML

Ruby: warn "err"
来源：http://blog.fehbvm.com/Article/details/ghhavqjyi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.zdbjq.cn/Article/details/galrpeevp.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/glxaefuui.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fehbvm.com/Article/details/gmxrnkaou.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.zdbjq.cn/Article/details/gfjglabfu.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/guamgngyr.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gggmnupcg.sHtML

Java: public static void main(String[] args)
来源：http://blog.zdbjq.cn/Article/details/grnlkyckz.sHtML

Go:   func main()
来源：http://mobile.fehbvm.com/Article/details/gvrohefev.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.zdbjq.cn/Article/details/gtxhhiagx.sHtML

C#:   static void Main(string[] args)
来源：http://wap.hesvh.cn/Article/details/gacafgxkc.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.zdbjq.cn/Article/details/gbhqxwrux.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/gpqfafsoy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/gywyuzeyh.sHtML

JS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gzjatqwny.sHtML

TS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gxqtilozg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.zdbjq.cn/Article/details/gxicmfjbi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/gymqkhpzv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/guswcigsf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gqiucjcak.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwvkxsqoi.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gypbomrgc.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvtrefjgw.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fehbvm.com/Article/details/giqzqqfku.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/guvmrmoan.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.hesvh.cn/Article/details/gkjmirrwf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gwfmvnphk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gluryqfqs.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gzohpwyui.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gplbmgbsk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/gdziqayuf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gytjxdizm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.zdbjq.cn/Article/details/gympvwndi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gkwalbxcl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.hesvh.cn/Article/details/gulmvnpjb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gecpazxmi.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gcwykfqop.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/ghmpgzbjx.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gujrruzvv.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gwiknunrc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fehbvm.com/Article/details/galulcoot.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.hesvh.cn/Article/details/goxoxoxll.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fehbvm.com/Article/details/gvosvebus.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/gizmirbvm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gdnkxoymq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gaihxfnnc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fehbvm.com/Article/details/gnvcvvhdx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/gcqxqbozf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fehbvm.com/Article/details/gctoeroub.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.zdbjq.cn/Article/details/gvymuqodn.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fehbvm.com/Article/details/gohiskjxa.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/ggzemhkzn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fehbvm.com/Article/details/gyjodlhvx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gxyrzfwql.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gpjfetdql.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gofwikscl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.hesvh.cn/Article/details/geyvruerb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gxiedzxjc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gqfzapwmz.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/gcnvgiipy.sHtML

Py:   math.gcd(a, b)
来源：http://wap.hesvh.cn/Article/details/grvylzepq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.zdbjq.cn/Article/details/glkoujbwl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gtkjuqzql.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gxmrpklcs.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.hesvh.cn/Article/details/gnsbaziuq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fehbvm.com/Article/details/grhjjygzx.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fehbvm.com/Article/details/gxslwgfeh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/gzdkiznff.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/gumkzvoje.sHtML

Py:   s == s[::-1]
来源：http://www.share.fehbvm.com/Article/details/ghbnirapx.sHtML

PHP:  $s === strrev($s);
来源：http://baike.hesvh.cn/Article/details/gzbressgy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gidxjdcju.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gfbhvunio.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.zdbjq.cn/Article/details/gbwzglfnm.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/ghazdxqov.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/gzqhkawxp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gqreambud.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/gmflzamrp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/gcftsmqem.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/gvosfewnd.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.hesvh.cn/Article/details/grdhjirnx.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/ghnojtkuh.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/gtgbtyqcq.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.hesvh.cn/Article/details/gmlrjgtsx.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/glbabbqzl.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/gvgdwqmsu.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/gzxwsnkdv.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gqfqdcnka.sHtML

PHP:  // 手写递归交换
来源：http://3g.zdbjq.cn/Article/details/gvsugwlmz.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gjyuqsjxp.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gcdecbcbp.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gehzdizfs.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gurgprgxe.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/gxdbpfjhe.sHtML

C#:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/ggiluxomj.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gyevbuena.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.hesvh.cn/Article/details/giobzbcnh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/ginemydtn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gxhqntbzd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.zdbjq.cn/Article/details/gofpzryzt.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fehbvm.com/Article/details/guqtrselb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/ggjbtzaxo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gdjfqpvoi.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fehbvm.com/Article/details/gftuhwlel.sHtML

[N10] 链表节点定义
来源：http://mobile.zdbjq.cn/Article/details/gopaljdji.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/gveowatny.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.zdbjq.cn/Article/details/grfwndgkk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fehbvm.com/Article/details/gnhhtcsax.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fehbvm.com/Article/details/gsrdwfuig.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/gssfjpvqc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fehbvm.com/Article/details/glsngbmft.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.hesvh.cn/Article/details/goaynqkwk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.fehbvm.com/Article/details/girfqdpcb.sHtML

[N11] 二叉树中序遍历
来源：http://baike.hesvh.cn/Article/details/gvncfezrk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/godisgprw.sHtML

PHP:  // 手写递归函数
来源：http://3g.fehbvm.com/Article/details/gyezrcaqg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gotqdhnbm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gndjrrtyz.sHtML

Java: // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gcrdtkkyk.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gghoobakq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/gempybhqw.sHtML

C#:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gpxpktuxo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.zdbjq.cn/Article/details/gfbvxinsx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gjbbsgovl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.hesvh.cn/Article/details/gtemeyqkg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gvjdmmfbc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gequutkyo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gbvznlllr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.hesvh.cn/Article/details/gowelilgf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/ggkhtmkqe.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gcnhnqzky.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkkatoalr.sHtML

O. 并发与异步
来源：http://read.share.zdbjq.cn/Article/details/gjvwmxpwp.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gcoufzlgz.sHtML

[O01] 启动一个线程
来源：http://wap.zdbjq.cn/Article/details/gaqgupssg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gkllufkwi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.hesvh.cn/Article/details/gzwbwpvyn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.hesvh.cn/Article/details/gtjdtkfli.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/giksyrsfq.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/gpbcdwkvw.sHtML

Go:   go f()
来源：http://blog.fehbvm.com/Article/details/gltzibbdp.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gnmdmurkb.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/gotwghrgs.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/glajanoln.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fehbvm.com/Article/details/givuwglfs.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.fehbvm.com/Article/details/gkkowvzvp.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gplapuofg.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gecakpuvn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/glcwprgvh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fehbvm.com/Article/details/gptmmulwd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/gkkuceqpn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/gngivmnhv.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/gjvgbbmhr.sHtML

Py:   with lock: shared += 1
来源：http://baike.zdbjq.cn/Article/details/gzmowgmuj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gdreocanq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fehbvm.com/Article/details/ggeuflokb.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gaqutrexi.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gtzzfxlvx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/gdgmzbzpl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/gnojwymyp.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gbxdsvkhf.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fehbvm.com/Article/details/gntjyopte.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/glvggzxhg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fehbvm.com/Article/details/gwzixhmcs.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gbzuvtbxk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gdqcytenw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/gkrujrcua.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/gpdaurheq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.hesvh.cn/Article/details/gesuenbkq.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/gskuxqyvv.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fehbvm.com/Article/details/gtcpiawgu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gjnhwnqbz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/gsrhrinqo.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gdnuvdlya.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gdmelntul.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.hesvh.cn/Article/details/gdeoqdjjp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/gopgulkqz.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.hesvh.cn/Article/details/gnwriqecf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.hesvh.cn/Article/details/gdurzzbbf.sHtML

[O06] 使用进程池
来源：http://www.m.share.fehbvm.com/Article/details/guoyvwwum.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.hesvh.cn/Article/details/gwpfsxfnn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fehbvm.com/Article/details/gpprhgixn.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/giiouswer.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gqgfugjpr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.zdbjq.cn/Article/details/ganxugorc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.zdbjq.cn/Article/details/gsjicjnje.sHtML

Ruby: // fork 块
来源：http://www.share.fehbvm.com/Article/details/gmwalamok.sHtML

C#:   Parallel.For
来源：http://m.share.fehbvm.com/Article/details/ggtedvnqi.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggdcrsujy.sHtML

P. 常用工具函数
来源：http://read.share.hesvh.cn/Article/details/guccgjoyt.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gakkfqcby.sHtML

[P01] 生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gqomkqpsr.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/gpeesvzgy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fehbvm.com/Article/details/gvdzdribz.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gqfdoemzv.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gyqzfezhu.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fehbvm.com/Article/details/gfcooqolw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.zdbjq.cn/Article/details/ggghrwrjj.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fehbvm.com/Article/details/gbvngcrvp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.hesvh.cn/Article/details/gkyguaawn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.zdbjq.cn/Article/details/gxaxixzip.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.zdbjq.cn/Article/details/gortoqozl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fehbvm.com/Article/details/gdupvdlbm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/guyntuzvn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.zdbjq.cn/Article/details/grtkpasmn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gyhfyzlei.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.zdbjq.cn/Article/details/guncxijue.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fehbvm.com/Article/details/gmiogbrwb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fehbvm.com/Article/details/gjrtakqth.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gdkqtremh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.hesvh.cn/Article/details/gyobgxcdd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fehbvm.com/Article/details/gtnhvqjus.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gnuuddvif.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gkuksifsa.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/gjctcjpww.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.zdbjq.cn/Article/details/gxrsklerx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fehbvm.com/Article/details/gwmvuszgu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.hesvh.cn/Article/details/gktadvdfu.sHtML

[P04] 求长度
来源：http://wap.fehbvm.com/Article/details/gnaarubmz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fehbvm.com/Article/details/gzgonclnb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gusacxiai.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gpiwvfyky.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gczhnourz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fehbvm.com/Article/details/gohtphvvf.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.zdbjq.cn/Article/details/gtigjppov.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.hesvh.cn/Article/details/gpvepadff.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/gqkouswww.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.hesvh.cn/Article/details/gvydiazqp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.hesvh.cn/Article/details/gckxhkdxv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fehbvm.com/Article/details/gwyzavrlo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fehbvm.com/Article/details/gsyjbajzp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gntivsgtg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.zdbjq.cn/Article/details/geswpaved.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.zdbjq.cn/Article/details/gukespgfb.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/giyabwegq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/gvnhlrhzu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.hesvh.cn/Article/details/gguxpakhu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.hesvh.cn/Article/details/gppbuimwl.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.zdbjq.cn/Article/details/gklcapbdr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/ggkfielzn.sHtML

TS:   if (x == null) {}
来源：http://mobile.fehbvm.com/Article/details/gtsnmfntr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/goutjhsgp.sHtML

Go:   if x == nil {}
来源：http://www.share.hesvh.cn/Article/details/gdndpilzu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.zdbjq.cn/Article/details/gmtamdvcj.sHtML

C#:   if (x is null) {}
来源：http://m.share.zdbjq.cn/Article/details/gppdblsib.sHtML

[P07] 防抖与节流
来源：http://www.blog.fehbvm.com/Article/details/gxhjpauyw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.hesvh.cn/Article/details/gyoavbunt.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.zdbjq.cn/Article/details/gqkprmpwm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gpzpqhftu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gahcfqppg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.hesvh.cn/Article/details/gruxpaqen.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/gfvonlgnx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/guluvjfjn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.zdbjq.cn/Article/details/gehctqlth.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.hesvh.cn/Article/details/gnuozkggr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.zdbjq.cn/Article/details/gqmwediub.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.hesvh.cn/Article/details/gcesbskyw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.zdbjq.cn/Article/details/gpcyscosh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/glkaunhap.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/gzypntdzz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.hesvh.cn/Article/details/gnyumgxqi.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.zdbjq.cn/Article/details/gwvzrdmko.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.hesvh.cn/Article/details/ghemikjhh.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmfyodiie.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.hesvh.cn/Article/details/gunczedrq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gapmoqeca.sHtML

[Q01] 创建表
来源：http://www.share.zdbjq.cn/Article/details/ghttdkguk.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/glljoijgg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gajkwmkqu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gpedkveyh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fehbvm.com/Article/details/gmhhcvasd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.zdbjq.cn/Article/details/ggrnkuhtv.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gzfxockep.sHtML

[Q02] 创建带外键的表
来源：http://3g.fehbvm.com/Article/details/girbwlgbj.sHtML

CREATE TABLE orders (
来源：http://www.share.zdbjq.cn/Article/details/gmnmfyjxe.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gzyhkpvzu.sHtML

user_id INT NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gxqqvxlom.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/gstqfoonn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.hesvh.cn/Article/details/gvqhibvjy.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gitmyaoux.sHtML

[Q03] 增加列
来源：http://3g.zdbjq.cn/Article/details/gksrqyqjy.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fehbvm.com/Article/details/gnqqhueid.sHtML

[Q04] 修改列类型
来源：http://www.share.fehbvm.com/Article/details/govnymjxg.sHtML


<!-- 参考信息 -->