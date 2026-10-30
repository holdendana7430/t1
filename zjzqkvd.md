代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gzclexjys.sHtML

JS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gazepbdua.sHtML

TS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gyldbekfu.sHtML

Java: System.getenv("HOME")
来源：http://www.share.hesvh.cn/Article/details/guciqjlsy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fehbvm.com/Article/details/gdqwnsenz.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/gbzodhori.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/ghyusielh.sHtML

[M03] 执行外部命令
来源：http://www.blog.fehbvm.com/Article/details/gghmnwqiy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gyqupjgqt.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/gsiqbtzkw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gfqnrdfoa.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gjccmlywp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.hesvh.cn/Article/details/gjnpiqiak.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.hesvh.cn/Article/details/gkxcqpcxm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.zdbjq.cn/Article/details/gzpqjvdek.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.hesvh.cn/Article/details/gcxxpbrwo.sHtML

[M04] 获取当前工作目录
来源：http://baike.zdbjq.cn/Article/details/gjfdckhge.sHtML

Py:   os.getcwd()
来源：http://www.blog.zdbjq.cn/Article/details/gndvuetef.sHtML

PHP:  getcwd();
来源：http://read.share.zdbjq.cn/Article/details/gvsnglsjg.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gbjwbevle.sHtML

TS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/grstzqfoo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fehbvm.com/Article/details/gyihhdtsh.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gjsaxxoli.sHtML

Ruby: Dir.pwd
来源：http://read.share.zdbjq.cn/Article/details/gmpdyncgv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/gvnignzim.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/gerexegko.sHtML

Py:   sys.exit(1)
来源：http://baike.hesvh.cn/Article/details/gmyazsdkz.sHtML

PHP:  exit(1);
来源：http://mobile.fehbvm.com/Article/details/gezphjlhc.sHtML

JS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/garqypjcn.sHtML

TS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/grzybqhjy.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/ghcyehvvh.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/gfsygdftg.sHtML

Ruby: exit 1
来源：http://m.share.zdbjq.cn/Article/details/gsugcatnr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/gsirwhbow.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fehbvm.com/Article/details/gcdmendrz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gbjwnmedl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/gwolgolsb.sHtML

JS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gaxziczhx.sHtML

TS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gjomwqmtr.sHtML

Java: System.err.println("err")
来源：http://3g.fehbvm.com/Article/details/glprgmvid.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.zdbjq.cn/Article/details/gddfkpwxj.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/gdalagobu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/gtvpjfxzz.sHtML

[M07] 判断是否为主入口
来源：http://3g.zdbjq.cn/Article/details/ggedvdjlf.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/gryxxdcgy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/gzjcureis.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/ggjdeunbc.sHtML

TS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gewmypxlc.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/gvagnalgg.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/gphtzvhln.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/gdxirdbfh.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/gseqrsdmm.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.zdbjq.cn/Article/details/gxnhxpoxq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fehbvm.com/Article/details/gdjxxlnwy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.hesvh.cn/Article/details/gjuapnvyw.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gnmqatkmu.sHtML

TS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/glvukitwd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/gpavrjifj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/gozhscqhw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/goriwzndf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/gwbortojt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqtbaejdn.sHtML

N. 数据结构与算法
来源：http://mobile.hesvh.cn/Article/details/gjgjltbht.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdihhaave.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/gzfhbksun.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/gdzwmjlqw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gtumbsrlk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gegpbbcnq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gjhwfewxp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gxexgvhyk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fehbvm.com/Article/details/gxgxurzjx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.hesvh.cn/Article/details/gbwyuqwlb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gzrhuljkx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fehbvm.com/Article/details/gwfzhkwbo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gzblpcxcd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/giclztqqg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gedpjcbuw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gcixayhox.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fehbvm.com/Article/details/glglakklz.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gndtitatb.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gllvhmhph.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fehbvm.com/Article/details/gyuvmyziw.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/gxcdnfzpu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/gcntkgpuu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/gsgwbzeok.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gvsbogjdh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gmkuffzub.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.hesvh.cn/Article/details/gyodzrogf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/guagcrgrr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fehbvm.com/Article/details/grfxhkdvm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.hesvh.cn/Article/details/gdojtksql.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/glrvdwlyu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gnvoxroii.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gasxmmige.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gyxcqyyzz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gdzccript.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gpqbpmdsz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.zdbjq.cn/Article/details/ggrkgnwxx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gpfchexry.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gtohotvqg.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/gcfqnimxk.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fehbvm.com/Article/details/gxyopbdan.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fehbvm.com/Article/details/goyngcdig.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gjhmolnrg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gsnhxtssn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/gvwcigtzw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/gbeyioizy.sHtML

Ruby: a.gcd(b)
来源：http://mobile.hesvh.cn/Article/details/ggjjgrxyk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/gefiaessf.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/gwfysalne.sHtML

Py:   s == s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gyypiudsj.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gdxrnpijr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gggtozwys.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gurumbhnm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/gaqlbrjjz.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.zdbjq.cn/Article/details/gsebhtrmx.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gpgqtkztj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gstjkqbdz.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/ghlpbouux.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/gtohekdjq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fehbvm.com/Article/details/gatyzsbxi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.zdbjq.cn/Article/details/gzaroyxey.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gfamoqnnr.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.zdbjq.cn/Article/details/gjwmgxiir.sHtML

Go:   // 手写 map[int]int
来源：http://wap.zdbjq.cn/Article/details/gljunzbse.sHtML

Ruby: // 手写 Hash
来源：http://wap.hesvh.cn/Article/details/ghiiadgps.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/gspyfugne.sHtML

[N08] 生成全排列
来源：http://baike.zdbjq.cn/Article/details/govuglplh.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.zdbjq.cn/Article/details/gotiylyxc.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/ganxtwftq.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/glhffmxyz.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/geeyilgui.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/glwllzsdo.sHtML

Go:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gridpskbs.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.hesvh.cn/Article/details/gupwjgptv.sHtML

C#:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gzxyuordf.sHtML

[N09] 栈与队列
来源：http://blog.hesvh.cn/Article/details/gfjfauzwb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/gzbdewwvg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gfrwbhzoc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/glrcwovah.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.zdbjq.cn/Article/details/gydohxxkn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gyvetawxe.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.hesvh.cn/Article/details/gmmpaknwd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gsjujtctm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.zdbjq.cn/Article/details/gmsdhsaxa.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/gvepdpfoy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/gtpbgqrie.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/gsfvdhitv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/gplppzzgt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fehbvm.com/Article/details/glwszkdyq.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fehbvm.com/Article/details/grohrrgaw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/gadfqpvod.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fehbvm.com/Article/details/gtgqbsffl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fehbvm.com/Article/details/gyxvxgxxs.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/gvzdnzwmi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fehbvm.com/Article/details/gfublslqk.sHtML

PHP:  // 手写递归函数
来源：http://blog.hesvh.cn/Article/details/gmkjpfszw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/ggtebssgg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gpswworeq.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gltdhhlns.sHtML

Go:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gwknhywnt.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.fehbvm.com/Article/details/ggerrpfai.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gtnejnste.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fehbvm.com/Article/details/gojzuvbws.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/gcqdvvjyz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.hesvh.cn/Article/details/gwyllnizk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gfpsgswri.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gquvbaspg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/ghjhlqhhr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.hesvh.cn/Article/details/gtxsgndoi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/gtybguzot.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gtuwkaomv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjsewbder.sHtML

O. 并发与异步
来源：http://blog.fehbvm.com/Article/details/gwjoxhath.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwvtpvjnq.sHtML

[O01] 启动一个线程
来源：http://baike.hesvh.cn/Article/details/guudaletm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/gxfegrune.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.zdbjq.cn/Article/details/gcfkudgei.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/gcvvwsysx.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/grbenjfcp.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.hesvh.cn/Article/details/ghttfdkev.sHtML

Go:   go f()
来源：http://www.blog.hesvh.cn/Article/details/gljdwpaqc.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.hesvh.cn/Article/details/glrpkgxfv.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fehbvm.com/Article/details/ghmppmqye.sHtML

[O02] 使用线程池
来源：http://www.blog.fehbvm.com/Article/details/gjgrrlfdx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.hesvh.cn/Article/details/grvpvltls.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fehbvm.com/Article/details/gyjenczmc.sHtML

JS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gkrhqdfcz.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gylasmrts.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.hesvh.cn/Article/details/gyrvbpxal.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.zdbjq.cn/Article/details/gjmfdavrb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.hesvh.cn/Article/details/gmjnjvfnq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.hesvh.cn/Article/details/gkhbbsatq.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/gjjvimnfd.sHtML

Py:   with lock: shared += 1
来源：http://baike.fehbvm.com/Article/details/gurgzdsqa.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.hesvh.cn/Article/details/gccdcneiv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.hesvh.cn/Article/details/gfvsywxze.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gavdjdclj.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gkwrsovnc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/gdguozmis.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/gwfdavtnv.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gfucklokf.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.zdbjq.cn/Article/details/ggipgsonf.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.zdbjq.cn/Article/details/gyvhaciui.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.zdbjq.cn/Article/details/guktcfokr.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gtbfvplct.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gxhxzodae.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.fehbvm.com/Article/details/goqzacneu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/gpbhlpkta.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.hesvh.cn/Article/details/gpvanqdjd.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.hesvh.cn/Article/details/glzaiwxci.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.hesvh.cn/Article/details/gsnezksox.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/giydxolku.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.zdbjq.cn/Article/details/gvvzuzcxo.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gkmxxeidr.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gwxkredbh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fehbvm.com/Article/details/giaefncdx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.zdbjq.cn/Article/details/gkagbnpmz.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gnmdiilhf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.hesvh.cn/Article/details/gwkaszhte.sHtML

[O06] 使用进程池
来源：http://read.share.fehbvm.com/Article/details/gzknrqjgt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.hesvh.cn/Article/details/glljzyxnz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.hesvh.cn/Article/details/gqkfpndxh.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gxkmfsbkk.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/ggtsfvtnd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/ghcohomee.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fehbvm.com/Article/details/giifwoxfb.sHtML

Ruby: // fork 块
来源：http://mobile.hesvh.cn/Article/details/ggxawscgi.sHtML

C#:   Parallel.For
来源：http://wap.fehbvm.com/Article/details/gwrkoynef.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gsvohweun.sHtML

P. 常用工具函数
来源：http://3g.hesvh.cn/Article/details/gwfliofyh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzqzgxvvk.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gshekptpe.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.hesvh.cn/Article/details/gsjnezrtt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/gitlpkxhe.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gobbbjpns.sHtML

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/grpwtfrrg.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.zdbjq.cn/Article/details/gacreewpn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.zdbjq.cn/Article/details/gznrbuolh.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/gvwfbchrp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fehbvm.com/Article/details/gbjgwypun.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.zdbjq.cn/Article/details/gyedukwke.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fehbvm.com/Article/details/gzjokeodr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.zdbjq.cn/Article/details/gyncikpjp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fehbvm.com/Article/details/govobawof.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.zdbjq.cn/Article/details/ggnrxpoxd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fehbvm.com/Article/details/gqmivwhkk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/gwchxlmfz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/gnqslfygw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.hesvh.cn/Article/details/gpxdsrzph.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/gtmsawcbl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.hesvh.cn/Article/details/gokoqohsb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.hesvh.cn/Article/details/gkkmidcck.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gipjbyies.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gjssxesal.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.zdbjq.cn/Article/details/gzymbfbfm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fehbvm.com/Article/details/gcfxozxki.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/godlekrof.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.hesvh.cn/Article/details/gbrcemnea.sHtML

[P04] 求长度
来源：http://baike.hesvh.cn/Article/details/gyiuzyjgw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.zdbjq.cn/Article/details/grhioraam.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gnoxadcss.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gyvdlcszj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gthvmvrbo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/ggfvbfuqf.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.fehbvm.com/Article/details/gufzcefwr.sHtML

Ruby: x.length;  x.size
来源：http://m.share.zdbjq.cn/Article/details/gvctyfktk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fehbvm.com/Article/details/gyshtmgym.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.hesvh.cn/Article/details/gojjvivbm.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/gssqldfyc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.hesvh.cn/Article/details/gdtlvoyod.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fehbvm.com/Article/details/gqknxknaw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gkmemuapq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fehbvm.com/Article/details/gxhepqjsn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gpxyvfquj.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/gcxkogegz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fehbvm.com/Article/details/gfnrofpdu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.hesvh.cn/Article/details/gqhkxicju.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.zdbjq.cn/Article/details/gwporhqev.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/geciranxb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/gqgseialp.sHtML

TS:   if (x == null) {}
来源：http://baike.zdbjq.cn/Article/details/gsalreqdl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/glzjviptb.sHtML

Go:   if x == nil {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbdfoweya.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.hesvh.cn/Article/details/gjdboleek.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fehbvm.com/Article/details/ghllogerb.sHtML

[P07] 防抖与节流
来源：http://m.share.zdbjq.cn/Article/details/gwwtjfqrq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fehbvm.com/Article/details/glligoxda.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.hesvh.cn/Article/details/gidfwjznc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gcytmjceq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gatioogzg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.zdbjq.cn/Article/details/gjwsbcsrx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.hesvh.cn/Article/details/ghowxpjjq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.hesvh.cn/Article/details/gxhswzwnt.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/gaamqvtez.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.zdbjq.cn/Article/details/gtxvfbxai.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fehbvm.com/Article/details/gzebxclin.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/gwgdpumoq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fehbvm.com/Article/details/gcxrvtnzg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/giempwqeo.sHtML


<!-- 参考信息 -->