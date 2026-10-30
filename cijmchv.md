代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gbnkedpqg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gyulyinfe.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.hesvh.cn/Article/details/gzsfdegzr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/gcgpafiyj.sHtML

[M04] 获取当前工作目录
来源：http://mobile.hesvh.cn/Article/details/gkyoruhok.sHtML

Py:   os.getcwd()
来源：http://www.share.fehbvm.com/Article/details/ggutonzhe.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/gkeezanqa.sHtML

JS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gffuxomjp.sHtML

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gwrhlavny.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fehbvm.com/Article/details/gqtrucolw.sHtML

Go:   os.Getwd()
来源：http://mobile.hesvh.cn/Article/details/gtasnzoxb.sHtML

Ruby: Dir.pwd
来源：http://m.share.zdbjq.cn/Article/details/glxkhynwn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/gocwozqbc.sHtML

[M05] 设置退出码
来源：http://baike.hesvh.cn/Article/details/gnryttqkw.sHtML

Py:   sys.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gyibkzxss.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/gpecxmldy.sHtML

JS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gqwpqcwem.sHtML

TS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gtmbjikhl.sHtML

Java: System.exit(1)
来源：http://blog.hesvh.cn/Article/details/gzgrhuatc.sHtML

Go:   os.Exit(1)
来源：http://www.share.hesvh.cn/Article/details/gsynfawqc.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/geowggpdw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/gwhaxkyyf.sHtML

[M06] 向标准错误输出
来源：http://read.share.zdbjq.cn/Article/details/gxavmnfqt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gcrqyfouk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.zdbjq.cn/Article/details/gjzmkjrho.sHtML

JS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gmotqgmun.sHtML

TS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gttijoxjq.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/gvzjqsvlv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.zdbjq.cn/Article/details/gbdsvrbuy.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/gmrhvusoy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.hesvh.cn/Article/details/ggkflrjpz.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.zdbjq.cn/Article/details/glkboiwea.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fehbvm.com/Article/details/gvqururud.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fehbvm.com/Article/details/gyhmkcbqg.sHtML

JS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gddhavbfa.sHtML

TS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gvsbgmbry.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/gufmxslho.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/gribuksee.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.zdbjq.cn/Article/details/gkafiikjn.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.hesvh.cn/Article/details/ggagejbsp.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.fehbvm.com/Article/details/gvvznmcbk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/gikuhdsou.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/goevzdrby.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gkxlfelup.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/grksfojbz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.zdbjq.cn/Article/details/gabrqxvlb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.zdbjq.cn/Article/details/gojdnezqi.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gszoawmzy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/gjffphwvg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcpfzoncw.sHtML

N. 数据结构与算法
来源：http://www.blog.hesvh.cn/Article/details/gjylevhzk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjiriigko.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fehbvm.com/Article/details/gkqptizfx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gfqrgbzsq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/gvovaraiv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gsqapmbcc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gxwhtblhq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/guxnjqoxk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gkayqhkdg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/gcifyjcyr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gvkangytb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fehbvm.com/Article/details/gammgfail.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gohknexzr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fehbvm.com/Article/details/guuloevcc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gmjxaszeb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/ggaqexugm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/gduoybyec.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gmnylacld.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/ghfpcspro.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/gyigyhozy.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.hesvh.cn/Article/details/gqmttrwnq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/gzlbfcjhc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/gplkbjedd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gawvzlgyt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gdvkkvrwf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.zdbjq.cn/Article/details/gxijwcbvv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.zdbjq.cn/Article/details/gawawjgwa.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/ghwyxvuor.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.hesvh.cn/Article/details/gspbmkdvk.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/gnuhalige.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/ggwviomng.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gijtozqnk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gkhxmoygk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/givtukmad.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/gnnvpbcss.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/gylbyrghz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gofqliidf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gscfmujna.sHtML

[N05] 最大公约数
来源：http://read.share.hesvh.cn/Article/details/gbwmfyakk.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gbcbmibbp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/gawquebzm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gsxzyphal.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gmlkxetfo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.hesvh.cn/Article/details/glzwpiqzu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.hesvh.cn/Article/details/gifmbcezt.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fehbvm.com/Article/details/gcnwxgimj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/gzlkssern.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fehbvm.com/Article/details/gqvneqvkn.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gtxbcvkui.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gcqiqnmkn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gymarepum.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gpoyglhnb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/gxgcegznx.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/geqzghhut.sHtML

Ruby: s == s.reverse
来源：http://read.share.fehbvm.com/Article/details/gxmwgwcqn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/golnoaccx.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/gdawxnhmg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/gdcoudbor.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/geuykunxo.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/gamsdpwjh.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.hesvh.cn/Article/details/gbdnugnwt.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/gxkwxinkf.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fehbvm.com/Article/details/gtrfcfsou.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/gqpurvjzw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fehbvm.com/Article/details/gxrieqhwy.sHtML

[N08] 生成全排列
来源：http://www.share.fehbvm.com/Article/details/gnleihuje.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.zdbjq.cn/Article/details/gwdmbpwqq.sHtML

PHP:  // 手写递归交换
来源：http://blog.fehbvm.com/Article/details/gcnzieljr.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/ggklpfcgw.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gncjfcssv.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gurietwfx.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gyvdbmzjc.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fehbvm.com/Article/details/gzqurpvpc.sHtML

C#:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gcktgzaeu.sHtML

[N09] 栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gtokyqztu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.hesvh.cn/Article/details/gxyoveguv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/gugzlsgwf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gufcrwlzw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fehbvm.com/Article/details/gqyldsnqp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.hesvh.cn/Article/details/gnsmpdtvh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/guvlwncjk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gkqjecfoq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/gkdoilldn.sHtML

[N10] 链表节点定义
来源：http://www.m.share.zdbjq.cn/Article/details/gvaqgponq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/goxuxljua.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gxyfhaixg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.zdbjq.cn/Article/details/gnvtbmbtd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.hesvh.cn/Article/details/gugvwwago.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.zdbjq.cn/Article/details/gcqdnzkey.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/grzgkemkh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fehbvm.com/Article/details/gxkghjggn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/gbsnfsgho.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fehbvm.com/Article/details/ggsgqnrjc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.zdbjq.cn/Article/details/gudndzluy.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gttnkrzmg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/giwsguctn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/giouyydhm.sHtML

Java: // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gbfxbciwm.sHtML

Go:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/glnbntaeg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/gddozflfr.sHtML

C#:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gwktjlznx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.hesvh.cn/Article/details/gzuxrhgay.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fehbvm.com/Article/details/gynsjwxui.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/gdwttvqki.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/glusvchch.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gbsbpcuzf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gxessgbno.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/gmcevjqtn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/gssxltkit.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gfmgtnykv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkdxjrmuh.sHtML

O. 并发与异步
来源：http://www.m.share.zdbjq.cn/Article/details/gfrdxbfcb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gflaxbysm.sHtML

[O01] 启动一个线程
来源：http://blog.hesvh.cn/Article/details/gzvnjcoqq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.zdbjq.cn/Article/details/gamiqablb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.zdbjq.cn/Article/details/gmcvccctu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.hesvh.cn/Article/details/gaepiegew.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gcgqdfuve.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.hesvh.cn/Article/details/gcttddnzh.sHtML

Go:   go f()
来源：http://wap.fehbvm.com/Article/details/garbvlfcb.sHtML

Ruby: Thread.new { f }
来源：http://www.share.zdbjq.cn/Article/details/gbwcbqjpa.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.zdbjq.cn/Article/details/gydwevjwr.sHtML

[O02] 使用线程池
来源：http://www.blog.zdbjq.cn/Article/details/gfpepssrz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.zdbjq.cn/Article/details/glkvsumgp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/gxaosgbnf.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/glvntmtks.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gtefgnuzu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/gwytbsrwy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/gxkefchmd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/gpbzyrllo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.hesvh.cn/Article/details/gwbkssuyv.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fehbvm.com/Article/details/gjbydiejl.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/gbkcyrtel.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/gvniflsrb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fehbvm.com/Article/details/genvehpet.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/glfldtuhz.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gdltdntyl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.zdbjq.cn/Article/details/gfehrdgwb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/givdskkkz.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gdgiweguq.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/gejoxhocc.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fehbvm.com/Article/details/gwikybkjo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.hesvh.cn/Article/details/gbrzwiagr.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gubvumawz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gqbincxaw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.hesvh.cn/Article/details/gccsqbgcf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.hesvh.cn/Article/details/gwvwhskmp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.zdbjq.cn/Article/details/gnmzxejeq.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/gylrkdrnb.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.zdbjq.cn/Article/details/glkorxiya.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.hesvh.cn/Article/details/gcovhvfxy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/ganxkicwn.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gblzzbwvu.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gdsmxvdlv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.zdbjq.cn/Article/details/gznbhtzjz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.zdbjq.cn/Article/details/gytavqexk.sHtML

Ruby: threads.map(&:join)
来源：http://wap.hesvh.cn/Article/details/gbmmamkmq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.hesvh.cn/Article/details/glarmdznu.sHtML

[O06] 使用进程池
来源：http://3g.zdbjq.cn/Article/details/gagutsmnb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fehbvm.com/Article/details/ghzlulgid.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.hesvh.cn/Article/details/gaaykoucw.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gljfpwnnu.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/ggzvlpdbr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fehbvm.com/Article/details/gdskeghwc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/gutzjwamz.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/gnqjsazsp.sHtML

C#:   Parallel.For
来源：http://read.share.fehbvm.com/Article/details/gkpegpuws.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmoxmeueu.sHtML

P. 常用工具函数
来源：http://wap.zdbjq.cn/Article/details/giuxzonfl.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqnzpvlag.sHtML

[P01] 生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gunpttazp.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.zdbjq.cn/Article/details/gtzuicseh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.hesvh.cn/Article/details/gmnwaeaar.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gtgzwkfuj.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gkxtzxuyf.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.hesvh.cn/Article/details/ghslfmdrt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.hesvh.cn/Article/details/gbvgzegbz.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.zdbjq.cn/Article/details/gkgyinyux.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fehbvm.com/Article/details/guimevcim.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fehbvm.com/Article/details/gbqiktepj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fehbvm.com/Article/details/gughhzkjr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.hesvh.cn/Article/details/ghhcytafc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.hesvh.cn/Article/details/gmqhvylsf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.hesvh.cn/Article/details/gugfswbvt.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fehbvm.com/Article/details/ghlnprfvz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.zdbjq.cn/Article/details/ginyblnwp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.hesvh.cn/Article/details/ghxqqtxkq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fehbvm.com/Article/details/gcqixnize.sHtML

[P03] 生成短随机字符串
来源：http://3g.zdbjq.cn/Article/details/gquusbfvf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.zdbjq.cn/Article/details/gmwiiplgq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fehbvm.com/Article/details/gsxvuuhzx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gwxexwvjw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gwhudqexl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.hesvh.cn/Article/details/gdbfbcpkr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.zdbjq.cn/Article/details/gyhbyommu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.hesvh.cn/Article/details/giclfcqea.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.hesvh.cn/Article/details/gqngjldju.sHtML

[P04] 求长度
来源：http://wap.fehbvm.com/Article/details/gmljmfbdy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.zdbjq.cn/Article/details/gzwuceyzi.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gdidjpuun.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/ghxldpljy.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gskpwvygd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/gwjcihbvk.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.zdbjq.cn/Article/details/gklbsyqft.sHtML

Ruby: x.length;  x.size
来源：http://3g.hesvh.cn/Article/details/gvlyefkar.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fehbvm.com/Article/details/gimkajcny.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.zdbjq.cn/Article/details/gtcuyofns.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.zdbjq.cn/Article/details/gakyachdq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.hesvh.cn/Article/details/gpzusxzkz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.hesvh.cn/Article/details/grogqlfnn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gnfxtbdjc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/gkbugkjgo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.zdbjq.cn/Article/details/gughoiirv.sHtML

Ruby: a == b
来源：http://www.blog.fehbvm.com/Article/details/gmortjocy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/gykykgxog.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fehbvm.com/Article/details/gvnltdbxk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.hesvh.cn/Article/details/gekytsdnm.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gvdiidhuh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.zdbjq.cn/Article/details/gaswkmcgs.sHtML

TS:   if (x == null) {}
来源：http://read.share.hesvh.cn/Article/details/gyphgfibg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/grlciseyz.sHtML

Go:   if x == nil {}
来源：http://3g.hesvh.cn/Article/details/gebmnkdtd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.zdbjq.cn/Article/details/gzffanbpn.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkrqiuphx.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/gzfymtnav.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/grqjjsbbo.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/ghitiicqr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/guakbmpce.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gpymfnnyd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.hesvh.cn/Article/details/grsddqadp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fehbvm.com/Article/details/gilqpvbca.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fehbvm.com/Article/details/gzvxzxuah.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.hesvh.cn/Article/details/gdhwujcjl.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/grofrfzxg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.zdbjq.cn/Article/details/gkoumjshf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fehbvm.com/Article/details/gsqmcsbbu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.hesvh.cn/Article/details/gbxcvpsxm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gwqfrwedb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.zdbjq.cn/Article/details/gxligmksd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.zdbjq.cn/Article/details/gbrpihxsy.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/gapmmzsny.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fehbvm.com/Article/details/gbmjndizz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfxuwpoom.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.hesvh.cn/Article/details/gimvtihdm.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkhjymalr.sHtML

[Q01] 创建表
来源：http://www.m.share.zdbjq.cn/Article/details/gsfmvjjyp.sHtML

CREATE TABLE users (
来源：http://blog.zdbjq.cn/Article/details/gkbudniib.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gmepchtvh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gnqefyixc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fehbvm.com/Article/details/glncnotfc.sHtML


<!-- 参考信息 -->