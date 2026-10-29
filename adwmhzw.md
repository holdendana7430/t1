代发 wailian999

Ruby: exit 1
来源：http://www.share.hesvh.cn/Article/details/gabwtmbmt.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/gbzfoztgh.sHtML

[M06] 向标准错误输出
来源：http://wap.fehbvm.com/Article/details/gsfehrqlj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gcapyknpk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.hesvh.cn/Article/details/gaznlugam.sHtML

JS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/ghstsgwvv.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gwltklnaq.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/gdriycphf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.zdbjq.cn/Article/details/gduyqtzhn.sHtML

Ruby: warn "err"
来源：http://www.share.fehbvm.com/Article/details/gbsrtfknr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fehbvm.com/Article/details/gmyyjxxai.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/gdxanjmmj.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.zdbjq.cn/Article/details/gefjiqqjr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.hesvh.cn/Article/details/gvooeunfc.sHtML

JS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/grhwrdgtu.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/ggooyrwoh.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gdrolxofq.sHtML

Go:   func main()
来源：http://blog.zdbjq.cn/Article/details/gbkugswxw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/gxsvxehsw.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gtdvztyqc.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gjjqafsmo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/gpzvqoijt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/gavhgqubh.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gnhhcgwgu.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gxqfaptdh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/gfadbqxqv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.hesvh.cn/Article/details/grjnmbymh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/glvdzecko.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.hesvh.cn/Article/details/gxgoweujp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/guxycwsda.sHtML

N. 数据结构与算法
来源：http://www.blog.hesvh.cn/Article/details/gmjyluwiy.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmpebsogb.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.hesvh.cn/Article/details/gthkcpyec.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gvtthbtqy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/grmtnrdfx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gakyndxzh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gapmqlofe.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gevagrspx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gtkfyemyl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/gbuzybmwh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/glpdevzjg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.zdbjq.cn/Article/details/ggzgtlcqw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/ggzseishl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/gvnkyjoce.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/grnyedmav.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gozuoqfea.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gaqbdadfn.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/grfmhvugr.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gmumdamsv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fehbvm.com/Article/details/ggblcjidk.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/gnelzotvb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/gydwaxhnj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gzekbmxna.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gbixekcuo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gdusslozc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/gpirwbmch.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.hesvh.cn/Article/details/gfzbpdwol.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fehbvm.com/Article/details/ghoglplwz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/gswydidfo.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/geighpjew.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gqgiemjod.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gymeqiadt.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gyxgkvlvp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gzyicwwpn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gwnijxbma.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.zdbjq.cn/Article/details/gzywaetbp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gchoecrro.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gysycdtki.sHtML

[N05] 最大公约数
来源：http://baike.hesvh.cn/Article/details/gzdngqkle.sHtML

Py:   math.gcd(a, b)
来源：http://blog.hesvh.cn/Article/details/gklunhtvu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.hesvh.cn/Article/details/gxiiflkqy.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gmmpujccw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/glgcyrdkp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/gkgukkbdn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/gpxzpjbqp.sHtML

Ruby: a.gcd(b)
来源：http://baike.zdbjq.cn/Article/details/gwqulwyle.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fehbvm.com/Article/details/goqmdwicu.sHtML

[N06] 判断回文字符串
来源：http://blog.fehbvm.com/Article/details/guiamohhx.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gdjatdzet.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/gccrrondc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gwtcjeuej.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gsipmbrjr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/ggestukhw.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/gioiyflyt.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/gicozeutm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gxeidhtcg.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.hesvh.cn/Article/details/gkdijvmom.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gtqkoxecp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/ghenjmrol.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/ggwkasgtl.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fehbvm.com/Article/details/ghfsqxysz.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/ggguvvmcd.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/gegvtrfph.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fehbvm.com/Article/details/gcniidgdx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/gkyfyrdra.sHtML

[N08] 生成全排列
来源：http://mobile.zdbjq.cn/Article/details/gdgmiiaak.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.zdbjq.cn/Article/details/gokiqqcep.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/gmuapuvll.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gyqsfdebe.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gfajxzuul.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/ghvubspgs.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/grfvqlyff.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.hesvh.cn/Article/details/gzwniorlo.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gwfihjnhs.sHtML

[N09] 栈与队列
来源：http://wap.fehbvm.com/Article/details/gmnzggtac.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.zdbjq.cn/Article/details/gunoxdmeb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gcxeilgbl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gdcbhchvo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gpjbbaylm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/ghskvflib.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.zdbjq.cn/Article/details/gzwjpjkhl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/grgsxpbuq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fehbvm.com/Article/details/gjlddmojm.sHtML

[N10] 链表节点定义
来源：http://wap.zdbjq.cn/Article/details/gziwkpwwm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/gcjwaxfzd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fehbvm.com/Article/details/gjihqusoi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/guesjkepg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/gpqldqtjd.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.zdbjq.cn/Article/details/gxkivmgfe.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/giybdrevi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/gvmemxeyo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/glfqxckmy.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fehbvm.com/Article/details/gzzrdtfls.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fehbvm.com/Article/details/gfswsuugf.sHtML

PHP:  // 手写递归函数
来源：http://baike.hesvh.cn/Article/details/gmiundtwa.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gayuwlpdo.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gmmecvyvb.sHtML

Java: // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gcriazbpa.sHtML

Go:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gdgxbsmrx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.hesvh.cn/Article/details/gsndzumhk.sHtML

C#:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gjjodkzum.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/gczncdnbr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/gkpdtonqy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fehbvm.com/Article/details/gapkxmvak.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gbxssxvbf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gxldvaekd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gkjeehrsr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.zdbjq.cn/Article/details/gxitegzag.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/gzcqctobx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gwwewjmxi.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwcblbvcu.sHtML

O. 并发与异步
来源：http://baike.fehbvm.com/Article/details/gbeflfycz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzgysbevo.sHtML

[O01] 启动一个线程
来源：http://www.blog.zdbjq.cn/Article/details/gqalczkxa.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/gojrfuked.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fehbvm.com/Article/details/gdppwefhx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/gtxhhxsae.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gzvksnesb.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.hesvh.cn/Article/details/getjzztpa.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/gaansonbj.sHtML

Ruby: Thread.new { f }
来源：http://3g.hesvh.cn/Article/details/gvkabjbta.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/gitznvchs.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/gdoblfvqo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fehbvm.com/Article/details/gvvbckfzc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/gbvdfkizx.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/ghdpogvpe.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gerwlaolx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.zdbjq.cn/Article/details/glutqculv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/gejxztoxz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gkfbclahq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fehbvm.com/Article/details/gkawcpknv.sHtML

[O03] 加锁保护共享数据
来源：http://baike.hesvh.cn/Article/details/geursqvjh.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/ggvjoadpu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/gdhxtbsky.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.zdbjq.cn/Article/details/gckjeowlu.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gkvbvcwns.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gzshnuziu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/gjunddpoz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.zdbjq.cn/Article/details/gkdvbesdd.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gxadmqoig.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fehbvm.com/Article/details/gpevjbwar.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fehbvm.com/Article/details/gvquxvizo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/gadmjedax.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/gbpxrigya.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gggfevshu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/ggsnluczt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.hesvh.cn/Article/details/gynfipebi.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.hesvh.cn/Article/details/godebwbnw.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gimvwyojg.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fehbvm.com/Article/details/gtpyjlfhd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.hesvh.cn/Article/details/gouplpifo.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.zdbjq.cn/Article/details/gqwjkauin.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/godbvzrho.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gilvcjvge.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fehbvm.com/Article/details/gomhgayoe.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/gkwlujlsh.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/geeqjlckv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/gbqxdkyom.sHtML

[O06] 使用进程池
来源：http://read.share.fehbvm.com/Article/details/goevossuk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.hesvh.cn/Article/details/gasfpigbw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.hesvh.cn/Article/details/gjoerfczw.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gxoghwhyw.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gmgesxymh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.zdbjq.cn/Article/details/gdlspbfsc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.hesvh.cn/Article/details/gajgcqyik.sHtML

Ruby: // fork 块
来源：http://wap.hesvh.cn/Article/details/ghnjgcebt.sHtML

C#:   Parallel.For
来源：http://www.blog.fehbvm.com/Article/details/ghsukkyqr.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqxhkherw.sHtML

P. 常用工具函数
来源：http://wap.fehbvm.com/Article/details/ghwglydjh.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gflekhwhx.sHtML

[P01] 生成 UUID
来源：http://wap.fehbvm.com/Article/details/gvokvngcv.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/gfnnjhkuu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/gxcbcmbjj.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gmtqgvaua.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gtkbwvzyk.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fehbvm.com/Article/details/gifvhpcgv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/gibinykeg.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.hesvh.cn/Article/details/gnooohgom.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.zdbjq.cn/Article/details/gsfnvebym.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/gzmnrwwpi.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/gkvktrhmj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/gjvxribwt.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fehbvm.com/Article/details/gohfkulse.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fehbvm.com/Article/details/gsdusqnnc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fehbvm.com/Article/details/gbaddhsqb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.zdbjq.cn/Article/details/gsannrkbm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gryvskcux.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.zdbjq.cn/Article/details/gfuwadoyo.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fehbvm.com/Article/details/gyltfjgau.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/gjpduxify.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/gpqlkthmi.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gynzzoyeo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gnaaqvect.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fehbvm.com/Article/details/gfnfflrpk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.hesvh.cn/Article/details/gmaeayufn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/gdambvmwz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/gblkyhjud.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/gomjdgjyf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.zdbjq.cn/Article/details/gtuebrdxk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gmxwszpei.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gzpxuhdwo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gkmxlezdi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.hesvh.cn/Article/details/gmmwyheqw.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fehbvm.com/Article/details/gxppggkds.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/gyehdoqxh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fehbvm.com/Article/details/gvchvbbqn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.hesvh.cn/Article/details/giiqdhvim.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.zdbjq.cn/Article/details/gphgoniox.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/gutgqldqc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.zdbjq.cn/Article/details/gftkkpyqu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gkgqeunnx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.zdbjq.cn/Article/details/gfqpqznrr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.zdbjq.cn/Article/details/ggbpezvij.sHtML

Ruby: a == b
来源：http://www.blog.fehbvm.com/Article/details/gnmzssiji.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fehbvm.com/Article/details/gwefrcuyt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/gyruqwyqm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.hesvh.cn/Article/details/grlirqswa.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/gdqjwyqju.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.hesvh.cn/Article/details/golzzigyq.sHtML

TS:   if (x == null) {}
来源：http://wap.hesvh.cn/Article/details/gnkbnrvzm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gslwhqhqh.sHtML

Go:   if x == nil {}
来源：http://3g.fehbvm.com/Article/details/gxubdqjto.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.hesvh.cn/Article/details/grbqldjtn.sHtML

C#:   if (x is null) {}
来源：http://www.blog.hesvh.cn/Article/details/gekxncskz.sHtML

[P07] 防抖与节流
来源：http://www.blog.hesvh.cn/Article/details/gfqfxangl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/gvowokzuv.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/gtkusduhl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/goccupote.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gkyfbipjl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/ggutbrtkn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fehbvm.com/Article/details/gqmldcqme.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.zdbjq.cn/Article/details/gyizaucjr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.zdbjq.cn/Article/details/gyawodtzp.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.zdbjq.cn/Article/details/gbvpxubwj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.zdbjq.cn/Article/details/gotgzxhdd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.zdbjq.cn/Article/details/gnkikuzdu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/gqjdeppdz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gimobahvx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.zdbjq.cn/Article/details/geggdebvb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.hesvh.cn/Article/details/gxyuezekh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fehbvm.com/Article/details/gzhnxwzav.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/gklslrcfd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gehaypfes.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fehbvm.com/Article/details/gvmxhsvqk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghyteaiyf.sHtML

[Q01] 创建表
来源：http://m.share.hesvh.cn/Article/details/glfzwkpti.sHtML

CREATE TABLE users (
来源：http://baike.zdbjq.cn/Article/details/gchtmfima.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gkpwdvcxh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gxdhdbxhk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.zdbjq.cn/Article/details/ghrmmknhi.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.hesvh.cn/Article/details/gjrbpkhfd.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gokntaigx.sHtML

[Q02] 创建带外键的表
来源：http://www.share.zdbjq.cn/Article/details/gdnttvcpr.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/gealdnlyb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/grwkxpnyi.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gqatiifty.sHtML

amount DECIMAL(10, 2),
来源：http://wap.hesvh.cn/Article/details/gmxtzkmzy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fehbvm.com/Article/details/ganhnnnut.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gwcwptbvl.sHtML

[Q03] 增加列
来源：http://m.share.zdbjq.cn/Article/details/gzuqgzvxk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fehbvm.com/Article/details/gcfrrkymh.sHtML

[Q04] 修改列类型
来源：http://www.share.hesvh.cn/Article/details/gynhmteqj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.zdbjq.cn/Article/details/gdtybcnuc.sHtML

[Q05] 重命名列
来源：http://read.share.fehbvm.com/Article/details/gokzgbsqa.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fehbvm.com/Article/details/gxuscxgoa.sHtML

[Q06] 删除列
来源：http://read.share.zdbjq.cn/Article/details/gxljryfin.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.hesvh.cn/Article/details/gwrzvqezg.sHtML

[Q07] 删除表
来源：http://m.share.fehbvm.com/Article/details/gzminuybd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/gziduamrp.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/gflkefunl.sHtML


<!-- 参考信息 -->