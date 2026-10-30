代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gpvohqjqy.sHtML

JS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gaqyyoezk.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gchyktpnu.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gzauhvcps.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gqhnsxmmr.sHtML

Ruby: ENV["HOME"]
来源：http://baike.zdbjq.cn/Article/details/ghswiuqmg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/grffqjgsw.sHtML

[M03] 执行外部命令
来源：http://3g.fehbvm.com/Article/details/gieoamund.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/guqpeauee.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/gpnrvlbxf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gkawtlxba.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/ghjvnldtw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fehbvm.com/Article/details/gufjagpls.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.fehbvm.com/Article/details/gjcnwersn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/gsekdlplk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.zdbjq.cn/Article/details/gylukartx.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/gslpqstjv.sHtML

Py:   os.getcwd()
来源：http://blog.hesvh.cn/Article/details/gidabddxe.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/gpslwiwvb.sHtML

JS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gadwvqsxb.sHtML

TS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gpniblhfp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fehbvm.com/Article/details/guuajypyj.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/gfomocpqe.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/gwdsjigeb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.hesvh.cn/Article/details/gsjkfgrtr.sHtML

[M05] 设置退出码
来源：http://www.blog.fehbvm.com/Article/details/gdcdxrjhq.sHtML

Py:   sys.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/goyswrkrt.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/gqimsgoyq.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gxglhkixn.sHtML

TS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gipspnglz.sHtML

Java: System.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gzfzsebbh.sHtML

Go:   os.Exit(1)
来源：http://mobile.zdbjq.cn/Article/details/ggyevlrqm.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/gmpgrubrk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fehbvm.com/Article/details/galgucubd.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/gmuejrikg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/glwiflayr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fehbvm.com/Article/details/gnidjqcms.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gbdnaczsd.sHtML

TS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gkgsekfjx.sHtML

Java: System.err.println("err")
来源：http://wap.zdbjq.cn/Article/details/gxqfakjiw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fehbvm.com/Article/details/gkkjrhbgz.sHtML

Ruby: warn "err"
来源：http://blog.hesvh.cn/Article/details/ghejhmjxy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.hesvh.cn/Article/details/ghgofjjta.sHtML

[M07] 判断是否为主入口
来源：http://read.share.hesvh.cn/Article/details/gqrxycarz.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/gxpybawre.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fehbvm.com/Article/details/gjtfnrhub.sHtML

JS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/guyyhohfq.sHtML

TS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gtxaezzif.sHtML

Java: public static void main(String[] args)
来源：http://blog.fehbvm.com/Article/details/gfwyhccgz.sHtML

Go:   func main()
来源：http://3g.zdbjq.cn/Article/details/gclukedot.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fehbvm.com/Article/details/gyiuxgykf.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.zdbjq.cn/Article/details/gyhlmncdx.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.zdbjq.cn/Article/details/gmjjkyhwu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.hesvh.cn/Article/details/gbvhivjbx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/gufwfkmqh.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/ghnaplhww.sHtML

TS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/grpcjsxjb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/gfuxdwejx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.hesvh.cn/Article/details/gsnvfhfhh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.zdbjq.cn/Article/details/gjtlnasny.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fehbvm.com/Article/details/ghaistqpu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gfjitcdgm.sHtML

N. 数据结构与算法
来源：http://www.blog.hesvh.cn/Article/details/gudyhsetx.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqsbriosd.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.zdbjq.cn/Article/details/genedsljs.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.hesvh.cn/Article/details/gpfvjrwwb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/ggravndra.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gyzkxcjkc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gswcrrgon.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/glpxezkek.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gygpnfuko.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/gdrhzqmtw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gfghldeqk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fehbvm.com/Article/details/gucfadqkv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gwldsoopr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/gnpsqptny.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gykhhvexv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gemgqtyaw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fehbvm.com/Article/details/gddemeiov.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gdbxzqugv.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/ggwzyvnbl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fehbvm.com/Article/details/gkvcvmqqg.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/ghvwreaii.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/gszjjyyvu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.zdbjq.cn/Article/details/gfqrvslwl.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gjozfbaex.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gggxtxkln.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/geljfayox.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fehbvm.com/Article/details/gqjysgobg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.zdbjq.cn/Article/details/gzhjrommu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/gtdmsvpdg.sHtML

[N04] 斐波那契数列
来源：http://www.blog.hesvh.cn/Article/details/gagdfixyw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gxmhdlxdg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gfcwmwhkv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/glvlnpnso.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gaobzbrgn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/giaxwlgcc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.hesvh.cn/Article/details/goskijitt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gyivviimx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/ghtriuwxp.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/glkefbhvi.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gkjpiwedf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fehbvm.com/Article/details/gvbyohzjy.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gwecfpqsi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gcrplintl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/gwfmgyckx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gkxlhrjvh.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/gesdntyar.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/gpddxnrkx.sHtML

[N06] 判断回文字符串
来源：http://m.share.hesvh.cn/Article/details/gmscxxskn.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gjdhornze.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gobwblclm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gmbdcfafx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gruhtamys.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/gtopkknur.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.hesvh.cn/Article/details/glmpinguv.sHtML

Ruby: s == s.reverse
来源：http://read.share.fehbvm.com/Article/details/gohyjactt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gvrsekrgm.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.hesvh.cn/Article/details/gmjyogsgg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/gtpgdsgdm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fehbvm.com/Article/details/gildkfjwd.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/gxvvfdunl.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gvlhxljzd.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/giwfvszqa.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.zdbjq.cn/Article/details/gdehuqlnh.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/gkacezpsf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.hesvh.cn/Article/details/gdhsjuphj.sHtML

[N08] 生成全排列
来源：http://3g.fehbvm.com/Article/details/ggxxtbhfd.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fehbvm.com/Article/details/gvaubnfay.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/gfrfitomq.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gieccicwg.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gpogmircl.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gnxvemwaq.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gcfuwhtjy.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.zdbjq.cn/Article/details/giafoqujv.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gjhlhvqcn.sHtML

[N09] 栈与队列
来源：http://3g.fehbvm.com/Article/details/gwcqnmxkq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.hesvh.cn/Article/details/ghrwgaxgz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gsewwlsie.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/guzgnnogc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.zdbjq.cn/Article/details/ghbxostmi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gvtusaovf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/gnzbdnbhu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gnchbuuut.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/glyxalscu.sHtML

[N10] 链表节点定义
来源：http://www.m.share.zdbjq.cn/Article/details/gcyzgohud.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/griratiyf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fehbvm.com/Article/details/ganqmbdtx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/gzjbqjycr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fehbvm.com/Article/details/gdeqfecln.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/goprplkpc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/golylhrym.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/gvmvpuddi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/grhaffqhk.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fehbvm.com/Article/details/glahidtaw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/gfilfyjpb.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fehbvm.com/Article/details/gjymjmjyd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/grvzejedy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gqsqiveaf.sHtML

Java: // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gykdjijxi.sHtML

Go:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/giulokbvj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/gzheieome.sHtML

C#:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gtamcqjsc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fehbvm.com/Article/details/gdbqjkdhd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/gisywkhpn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.hesvh.cn/Article/details/gimruedtu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gkziqxzes.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gdrdzvime.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gxluhusfs.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.zdbjq.cn/Article/details/gawhtnczg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.hesvh.cn/Article/details/ghpvihjpn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gziigctdt.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwwhqsbfs.sHtML

O. 并发与异步
来源：http://wap.fehbvm.com/Article/details/gewnlwvzt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gakogjdwb.sHtML

[O01] 启动一个线程
来源：http://www.blog.fehbvm.com/Article/details/ggokuxprp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fehbvm.com/Article/details/ghktvtjiz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/gitzoysrv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/gghmxnauo.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gtzbanhuy.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.zdbjq.cn/Article/details/grvczopar.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/gedcgfsoy.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fehbvm.com/Article/details/gsyvlhzjq.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/grygvqfha.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/gfnjhopyh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.hesvh.cn/Article/details/gcdfbaopu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/gzjgfeaax.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gjyzzrllp.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gcbuzbkrb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.hesvh.cn/Article/details/gfuktspgc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/gpmfealch.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/gimdggdrg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.zdbjq.cn/Article/details/gvpxjatne.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/gykbcjmmj.sHtML

Py:   with lock: shared += 1
来源：http://m.share.zdbjq.cn/Article/details/geiepqmeo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fehbvm.com/Article/details/grbzwdyvw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fehbvm.com/Article/details/guaeenfyo.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gbomomrld.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gezytyyqr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fehbvm.com/Article/details/gniawqeln.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/gfiqkuxxl.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gkgzymymh.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/gkepirlip.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.hesvh.cn/Article/details/gplfkrhiv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/gknzjudxl.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/ggghbkwfd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gkxhxcnky.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fehbvm.com/Article/details/gcaycxhvj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/grxwcgkzb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/gaiiuvcko.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.hesvh.cn/Article/details/gdpbbvniw.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/gxidycayc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.hesvh.cn/Article/details/gisbgvxjt.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.zdbjq.cn/Article/details/goyulwzmq.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gelykfxjj.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gduhlnvnx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.hesvh.cn/Article/details/gmuxgmytk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fehbvm.com/Article/details/gagcjilun.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/gdutyknnd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.zdbjq.cn/Article/details/goiqhgduk.sHtML

[O06] 使用进程池
来源：http://read.share.zdbjq.cn/Article/details/gvfwyqqli.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fehbvm.com/Article/details/guemamopv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.zdbjq.cn/Article/details/gxpofgntt.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gufozwedg.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/ggczqstgn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fehbvm.com/Article/details/ggqnueiwm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.zdbjq.cn/Article/details/gxnqbcacl.sHtML

Ruby: // fork 块
来源：http://3g.fehbvm.com/Article/details/gzivbywxs.sHtML

C#:   Parallel.For
来源：http://blog.hesvh.cn/Article/details/glgahyhfj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqapvwkot.sHtML

P. 常用工具函数
来源：http://mobile.hesvh.cn/Article/details/glwmbygfw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gipppaixy.sHtML

[P01] 生成 UUID
来源：http://3g.hesvh.cn/Article/details/guwhrugfw.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/ghlzzutzb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.hesvh.cn/Article/details/gkwmczddu.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gtslduqnk.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gznuczouh.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/glxvrwdkb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gewoqnaxe.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gipgcvfhd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fehbvm.com/Article/details/gdqlbgeea.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fehbvm.com/Article/details/gxikewpqj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.zdbjq.cn/Article/details/goxdnwioh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/gckgtxqgz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.hesvh.cn/Article/details/gebuoqxnd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fehbvm.com/Article/details/grlytecmg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gzqskvxfl.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/giswinqjp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fehbvm.com/Article/details/gpymtdtlf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/gorsqmwln.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/gnolfufir.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.hesvh.cn/Article/details/gddhghjku.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/gflnnfmzt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/glbjpjdfd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gkegdnggk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fehbvm.com/Article/details/gstqakgcg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.hesvh.cn/Article/details/gfcjkrfrh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.zdbjq.cn/Article/details/gcsdwfezz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.hesvh.cn/Article/details/ggcmtralz.sHtML

[P04] 求长度
来源：http://read.share.fehbvm.com/Article/details/gsvtnevet.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gxpmxqnid.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gnrrknxrv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gmsnhlfob.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gkrlepnpt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fehbvm.com/Article/details/gpjpdqzef.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.hesvh.cn/Article/details/gnezklmtr.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gnhxxjjty.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.zdbjq.cn/Article/details/ggjsdueco.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/gisosxfeg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.hesvh.cn/Article/details/gitonikyt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.hesvh.cn/Article/details/gydgwjgdm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/gefbiijkj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gnykimycp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.zdbjq.cn/Article/details/gansziccr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.fehbvm.com/Article/details/gbagbdsfd.sHtML

Ruby: a == b
来源：http://www.m.share.hesvh.cn/Article/details/guwlpqbuj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/gxnzrohax.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/gjhnitwta.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/gxtadxvqe.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gysilhesv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.zdbjq.cn/Article/details/gbqkeflbw.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gkscwjapv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gaukucrws.sHtML

Go:   if x == nil {}
来源：http://www.share.zdbjq.cn/Article/details/gbskbvzpr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fehbvm.com/Article/details/gzxybehdj.sHtML

C#:   if (x is null) {}
来源：http://blog.hesvh.cn/Article/details/gcmpojnzm.sHtML

[P07] 防抖与节流
来源：http://3g.zdbjq.cn/Article/details/gvcycsrtc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fehbvm.com/Article/details/gzscswbdv.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.zdbjq.cn/Article/details/gnmjfxhfx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gbnaxfscw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gldrpcsgr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fehbvm.com/Article/details/groizbzpc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.hesvh.cn/Article/details/gpudubybf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fehbvm.com/Article/details/gqrkidzst.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fehbvm.com/Article/details/gbpxuranh.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.zdbjq.cn/Article/details/gbzajndxv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.zdbjq.cn/Article/details/ghzzhcbdc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fehbvm.com/Article/details/gfjbvaqid.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/gokojrsom.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gpgodmvll.sHtML


<!-- 参考信息 -->