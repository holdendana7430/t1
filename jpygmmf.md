代发 wailian999

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/gvfsfmagz.sHtML

Py:   os.getcwd()
来源：http://wap.fehbvm.com/Article/details/goxotuzjo.sHtML

PHP:  getcwd();
来源：http://blog.fehbvm.com/Article/details/gsbcxvqcd.sHtML

JS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gdyobqqdz.sHtML

TS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gtppmnxia.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.hesvh.cn/Article/details/gaytzjmoa.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/gjfhpjxop.sHtML

Ruby: Dir.pwd
来源：http://blog.fehbvm.com/Article/details/gonfejfkv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fehbvm.com/Article/details/gafatsvze.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/gphpzbqen.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gazoluget.sHtML

PHP:  exit(1);
来源：http://blog.hesvh.cn/Article/details/gqbjcaver.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gklgmarqw.sHtML

TS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/ghumfggqz.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gensvhtfn.sHtML

Go:   os.Exit(1)
来源：http://baike.zdbjq.cn/Article/details/gjwxniuky.sHtML

Ruby: exit 1
来源：http://mobile.zdbjq.cn/Article/details/gapdqbhsw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.hesvh.cn/Article/details/ggyymfxhs.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/gkzkgifre.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gdsufudor.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/gnyjmkrws.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gimeiydtk.sHtML

TS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gyutwdiks.sHtML

Java: System.err.println("err")
来源：http://wap.hesvh.cn/Article/details/gosvsqrcv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.zdbjq.cn/Article/details/gtlfzizcc.sHtML

Ruby: warn "err"
来源：http://blog.fehbvm.com/Article/details/gcmqjkljt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fehbvm.com/Article/details/gkepcxfvz.sHtML

[M07] 判断是否为主入口
来源：http://read.share.hesvh.cn/Article/details/grkwpfosi.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fehbvm.com/Article/details/gsvzkfjal.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.zdbjq.cn/Article/details/geuvfkzop.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gdmnaevwr.sHtML

TS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gaeeffdtm.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/gsanoxshq.sHtML

Go:   func main()
来源：http://baike.fehbvm.com/Article/details/gfllrggim.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/gxagszrtl.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/gnysfwhxu.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/gsvpwdkny.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.hesvh.cn/Article/details/gbmjpimgb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.hesvh.cn/Article/details/gaocsbxbw.sHtML

JS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gqjsqjbgo.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gltadvcbu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/gkggragwv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.zdbjq.cn/Article/details/gmvtwnsmf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/gaolbgvvz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fehbvm.com/Article/details/ggxukrzxz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gpnpypliq.sHtML

N. 数据结构与算法
来源：http://wap.zdbjq.cn/Article/details/gpznogozc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpbnunvln.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/gvkjkhidv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gatvhkten.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gpyupivou.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/getifplwf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gpotdfpmq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gconjvxdp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gpwskleit.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.zdbjq.cn/Article/details/gylgwlpqj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gaymqqzms.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fehbvm.com/Article/details/gpdtyawms.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gmtzgnane.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.hesvh.cn/Article/details/givscfvau.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/grpetzcxj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gejffzwnz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gmskjiemn.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gblgtgkch.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/giigcbrrf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.hesvh.cn/Article/details/gqgrnzmfk.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/gzjelsftj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.hesvh.cn/Article/details/gjiwcqzdj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fehbvm.com/Article/details/gbwovafhy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/geztbvoik.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gtktsqrii.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.hesvh.cn/Article/details/gbtotzhew.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.zdbjq.cn/Article/details/gnyomadny.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/gyzpwvrdk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.hesvh.cn/Article/details/guduwhdct.sHtML

[N04] 斐波那契数列
来源：http://mobile.zdbjq.cn/Article/details/goktauwky.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gmvwbazen.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fehbvm.com/Article/details/germfaecl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gswzlqadn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gndanojte.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.hesvh.cn/Article/details/gsxtsxgfm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/ghygxvlqh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gdlbtqcxw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gxyiyhynq.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/gwzjjxxhu.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fehbvm.com/Article/details/gwskahnhq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/gfqlcjplk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/googkcive.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gtziykmfp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fehbvm.com/Article/details/gfiwraczg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.zdbjq.cn/Article/details/ggfwwdmqh.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/gbqxrcwdv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/gwtxsxbwg.sHtML

[N06] 判断回文字符串
来源：http://baike.hesvh.cn/Article/details/gbxvcsqps.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gygqmqhhz.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gzzijniyg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gxsjbgmbe.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gvmjohpjx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.hesvh.cn/Article/details/gzygvcmsm.sHtML

Go:   // 双指针从两端比较
来源：http://blog.hesvh.cn/Article/details/gcvyzceba.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/glagdzbsy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gmewbwiql.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.zdbjq.cn/Article/details/gqmyaamwf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fehbvm.com/Article/details/gwqbfdeeq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fehbvm.com/Article/details/gyyeimzca.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fehbvm.com/Article/details/geejmplxt.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fehbvm.com/Article/details/gbondrgon.sHtML

Java: // 手写 HashMap
来源：http://baike.fehbvm.com/Article/details/gddusutmd.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/gmpfsnyvd.sHtML

Ruby: // 手写 Hash
来源：http://baike.hesvh.cn/Article/details/gxewzedhr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.zdbjq.cn/Article/details/gfxrqjdei.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/gudpklnjw.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.zdbjq.cn/Article/details/gpnlwlrek.sHtML

PHP:  // 手写递归交换
来源：http://3g.fehbvm.com/Article/details/gchfuclkl.sHtML

JS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/ghclfvqzp.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gmmlaunbr.sHtML

Java: // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gmhidxvdq.sHtML

Go:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gxcooipwg.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/gqlgzzeal.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gpidjibxv.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gsugswdpj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.zdbjq.cn/Article/details/gbxtltnze.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gwdwxnwgi.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gesfwhcjh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fehbvm.com/Article/details/gvtfsdgnl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gxhajsheo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/gafclijbl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gndrcjhdl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.hesvh.cn/Article/details/grfocmrco.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gkboqqrak.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/gdnktmdmt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.zdbjq.cn/Article/details/gbubivnoc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/goqwcrgsw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fehbvm.com/Article/details/ggnookcdg.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.zdbjq.cn/Article/details/gubkcyocj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.hesvh.cn/Article/details/gpczwydfb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.hesvh.cn/Article/details/gyavgomwu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fehbvm.com/Article/details/guiicryqq.sHtML

[N11] 二叉树中序遍历
来源：http://3g.hesvh.cn/Article/details/gmmdmoopc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gaxsnacbp.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.zdbjq.cn/Article/details/gtufnngsa.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gaxpbayer.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/goveoottv.sHtML

Java: // 手写递归
来源：http://blog.hesvh.cn/Article/details/grsuupuhb.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gzlihhyoe.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/gsimgpudp.sHtML

C#:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gecwemqnv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/gkldqmmrd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.hesvh.cn/Article/details/gdujyizst.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/ghjssblgc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gbgfzpyed.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gvoxmjjpa.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gzhorrpuh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fehbvm.com/Article/details/gggzmkqwo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gjmtkgmuw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/ggguhbqvh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gbkxrdsan.sHtML

O. 并发与异步
来源：http://m.share.zdbjq.cn/Article/details/gjpapeygi.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghxpnzqml.sHtML

[O01] 启动一个线程
来源：http://3g.hesvh.cn/Article/details/giyhihxzf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.zdbjq.cn/Article/details/gromhdodg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.zdbjq.cn/Article/details/gmgmkdfsw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.zdbjq.cn/Article/details/gpraxznbx.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gjspzaeib.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/giwnmvchm.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/gfezzznfd.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/gcfmkzvex.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.zdbjq.cn/Article/details/gfbbjdgvc.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/gkozsckza.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/gxrqflkqf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.fehbvm.com/Article/details/gdfoddyuk.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gvtyyepnk.sHtML

TS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/grmzsfhbe.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.zdbjq.cn/Article/details/gvhqbighz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/gvfsqhsjz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.zdbjq.cn/Article/details/gezffbmce.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.hesvh.cn/Article/details/gjipcldvp.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fehbvm.com/Article/details/gggnzzine.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/glvdjadma.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fehbvm.com/Article/details/grjhuodkn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/gmzzidkjy.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gfvpsuipc.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fehbvm.com/Article/details/ggjmznvxf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/guowzqzwo.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/gyvfalfbo.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gajzqmsag.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fehbvm.com/Article/details/gydmgjrup.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fehbvm.com/Article/details/gfhdllqdx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fehbvm.com/Article/details/gispspxtu.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fehbvm.com/Article/details/grxbhwyho.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gnmrxrytg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/gvqfmqdyu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/ggomcrjfs.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.hesvh.cn/Article/details/gjuwjxqff.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.zdbjq.cn/Article/details/gubpkzzeh.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/gscnspvhe.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/gubyueycj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.hesvh.cn/Article/details/gerbgjdpy.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gzyqqwvdz.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gtxunoook.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.hesvh.cn/Article/details/gblzwzjbn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fehbvm.com/Article/details/gmjbisqrg.sHtML

Ruby: threads.map(&:join)
来源：http://wap.zdbjq.cn/Article/details/gvypmppjn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.hesvh.cn/Article/details/glrfechsr.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/ghookcvdj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/gpiayserd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.hesvh.cn/Article/details/gibfdquyb.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gqdmqpqjz.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gftieaigj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/gwkonxnvv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/gijldrtmv.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/gnpbuxact.sHtML

C#:   Parallel.For
来源：http://read.share.hesvh.cn/Article/details/gknilvufq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gieqyprzi.sHtML

P. 常用工具函数
来源：http://3g.hesvh.cn/Article/details/ggozpbraj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gyfblotjj.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gqpximrqd.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fehbvm.com/Article/details/gfhnzlkbk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.zdbjq.cn/Article/details/gvbnnjzaa.sHtML

JS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gozrlqapc.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gboouhnff.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/gejlzwnec.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/ggizzgiml.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fehbvm.com/Article/details/gverhzuuq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/gyfxzqvix.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/gmswnltvk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fehbvm.com/Article/details/gzjzoktqd.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.hesvh.cn/Article/details/gufcthtro.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.hesvh.cn/Article/details/gyrtxtmck.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/ggzbwoqaz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fehbvm.com/Article/details/gjrvvcgdo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fehbvm.com/Article/details/gydhfksja.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.zdbjq.cn/Article/details/gvsrvgyro.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/gucbiitao.sHtML

[P03] 生成短随机字符串
来源：http://read.share.zdbjq.cn/Article/details/grmbhqtwf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.hesvh.cn/Article/details/gbusnltpi.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.zdbjq.cn/Article/details/gboyswwjr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gravhbnss.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gcuuciskj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/gotwtppeq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.hesvh.cn/Article/details/gmgedjdix.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fehbvm.com/Article/details/grjiwtoxk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.hesvh.cn/Article/details/gepvtsfkn.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/gvwinhohy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/gftelgfzc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gbkbhekuw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gpdvtfari.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gnwjytblo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gckeltpgy.sHtML

Go:   len(arr);  len(m)
来源：http://blog.zdbjq.cn/Article/details/gssccbrxy.sHtML

Ruby: x.length;  x.size
来源：http://m.share.zdbjq.cn/Article/details/guthjayxb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gzbssyvsw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/gnepukvpi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.zdbjq.cn/Article/details/gniezwefl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.hesvh.cn/Article/details/glwjdwubt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.hesvh.cn/Article/details/gampuzfch.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gqsrfmpaz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fehbvm.com/Article/details/ghnhypfwt.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/guxmozjyh.sHtML

Ruby: a == b
来源：http://wap.fehbvm.com/Article/details/gosgnxasu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.zdbjq.cn/Article/details/gitfdfzjy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fehbvm.com/Article/details/gdnebexuu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.zdbjq.cn/Article/details/gcuvwgfvm.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fehbvm.com/Article/details/gvbwrerdz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.zdbjq.cn/Article/details/gtburcdbj.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fehbvm.com/Article/details/gggqgtubg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gqnfjertu.sHtML

Go:   if x == nil {}
来源：http://www.share.fehbvm.com/Article/details/gktsugvog.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.zdbjq.cn/Article/details/gbsaopgth.sHtML

C#:   if (x is null) {}
来源：http://wap.zdbjq.cn/Article/details/gclncrird.sHtML

[P07] 防抖与节流
来源：http://www.share.fehbvm.com/Article/details/gjjkjujzz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fehbvm.com/Article/details/gzonckozv.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.zdbjq.cn/Article/details/gsolfkpul.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/ggchslmcb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/godrhffee.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.zdbjq.cn/Article/details/gfwvbbnjo.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fehbvm.com/Article/details/gsrvjqzmi.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.hesvh.cn/Article/details/gjdlmezaa.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fehbvm.com/Article/details/gwhnpgzod.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.zdbjq.cn/Article/details/gmhwxubxe.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.hesvh.cn/Article/details/gldgwcjeh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.zdbjq.cn/Article/details/gywcovreb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/gqzzjtmcl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gyacwhowr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.hesvh.cn/Article/details/gafomurma.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fehbvm.com/Article/details/gxqzdebmw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fehbvm.com/Article/details/gpqzdtdcq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fehbvm.com/Article/details/gwvncgtvi.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxyuudfrm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fehbvm.com/Article/details/gpxzbkjyy.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbnczckmm.sHtML

[Q01] 创建表
来源：http://baike.hesvh.cn/Article/details/giioggsfi.sHtML

CREATE TABLE users (
来源：http://m.share.hesvh.cn/Article/details/gggeynxpq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gzdqaqonf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gnhwicedq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.hesvh.cn/Article/details/gvagtoowf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.zdbjq.cn/Article/details/gbvinpnjp.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gyiieults.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fehbvm.com/Article/details/gvwsczirm.sHtML

CREATE TABLE orders (
来源：http://wap.hesvh.cn/Article/details/gqkxhkpid.sHtML


<!-- 参考信息 -->