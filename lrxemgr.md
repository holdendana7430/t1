代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gmsljcoqv.sHtML

JS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gmjvmtnuw.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gslnmoirw.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gbuxthqyc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fehbvm.com/Article/details/gcxkuwjtq.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.zdbjq.cn/Article/details/gojyycsqi.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fehbvm.com/Article/details/gtycjodok.sHtML

[M03] 执行外部命令
来源：http://blog.fehbvm.com/Article/details/gbaqluzcz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/gluvpqnow.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.hesvh.cn/Article/details/galzpwoub.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gtowhxtdc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gdhhvqwgf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.hesvh.cn/Article/details/gentuaybc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gtsczecqt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/ghaathjbg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.hesvh.cn/Article/details/gbpuzzdyg.sHtML

[M04] 获取当前工作目录
来源：http://m.share.hesvh.cn/Article/details/gpibaoqsm.sHtML

Py:   os.getcwd()
来源：http://blog.zdbjq.cn/Article/details/gcjwrzvmn.sHtML

PHP:  getcwd();
来源：http://wap.zdbjq.cn/Article/details/glbwyoyha.sHtML

JS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gdinskvmw.sHtML

TS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gvbohhdfz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/gzedpdsfj.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/gfdkdxvct.sHtML

Ruby: Dir.pwd
来源：http://blog.hesvh.cn/Article/details/gjetinkox.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/gpsfbfybp.sHtML

[M05] 设置退出码
来源：http://www.share.fehbvm.com/Article/details/gknjuegck.sHtML

Py:   sys.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gerlkqqvz.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gxrmzywkg.sHtML

JS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gdbexfbtk.sHtML

TS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/ggryhilub.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gmttuxsmd.sHtML

Go:   os.Exit(1)
来源：http://3g.zdbjq.cn/Article/details/giyyshctk.sHtML

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/gehjmsaja.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.zdbjq.cn/Article/details/gtzmuippt.sHtML

[M06] 向标准错误输出
来源：http://blog.hesvh.cn/Article/details/gibyhaayi.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/ggcdftspy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.zdbjq.cn/Article/details/gtjofjbii.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gguebvvbm.sHtML

TS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gjjtidytb.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/gjmwfzyrc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.zdbjq.cn/Article/details/gqprdqyyg.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/ghmsbmrrq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fehbvm.com/Article/details/gnwkemnsq.sHtML

[M07] 判断是否为主入口
来源：http://3g.fehbvm.com/Article/details/gqpufjypo.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fehbvm.com/Article/details/gdfnnaues.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.zdbjq.cn/Article/details/gyitskbum.sHtML

JS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gbhbkkglt.sHtML

TS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gevtpqvht.sHtML

Java: public static void main(String[] args)
来源：http://blog.fehbvm.com/Article/details/gxuynfyok.sHtML

Go:   func main()
来源：http://blog.zdbjq.cn/Article/details/gaykkumly.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fehbvm.com/Article/details/gqmlgipkb.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.hesvh.cn/Article/details/giqzhyysr.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/gjpkhkkbu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/ghapkesyt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/gtrcffudp.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gasfstxbv.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gyehwrhwu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.hesvh.cn/Article/details/gnrjlhttk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gnaxtlmda.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/gxgiuyndp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.hesvh.cn/Article/details/guienutdb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/goymxmcva.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gzgztcwch.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwivvljja.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/gsevdndpb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gbdhmlhzc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.zdbjq.cn/Article/details/gerpwahch.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gptlyptlk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/ghfhyxgcc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/getmevahv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gyublvmts.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/gkmooinqd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gklfctosf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/gnthjblmc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gbpbifbgx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.zdbjq.cn/Article/details/gqvravpkc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gcyelqchb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gsqxczgjc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fehbvm.com/Article/details/gkagaysni.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/guyflplrs.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gpxdglyfb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fehbvm.com/Article/details/gbeasgjqq.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.zdbjq.cn/Article/details/gviatenot.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/grrmpmayn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/gsrpqmtpb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/grlmutdrk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/giokjwckg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/gftqbulad.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/gaqjisfuz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/gucmsdmmq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/gpqobpzvt.sHtML

[N04] 斐波那契数列
来源：http://m.share.fehbvm.com/Article/details/ghmdtjacn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gztfcjamm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gywnvywnx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gygstxquj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/glaybvdbq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gskbtqhmj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/gpuuvixgl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gchkbdvlz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gtfditdep.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/gujfyqrgx.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gswixfsge.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/ggltanbiv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gkkhwpcli.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gneuhpxuy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fehbvm.com/Article/details/guervlgxm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.zdbjq.cn/Article/details/giqqmaejc.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/gefirmzwi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.zdbjq.cn/Article/details/gvtazxmst.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gmznpermr.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gsnhroeyk.sHtML

PHP:  $s === strrev($s);
来源：http://wap.hesvh.cn/Article/details/gdxkwfkru.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gmevbpqzf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gjfsmglkj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/ghstrejuv.sHtML

Go:   // 双指针从两端比较
来源：http://baike.hesvh.cn/Article/details/gwvhcydce.sHtML

Ruby: s == s.reverse
来源：http://read.share.hesvh.cn/Article/details/grkpmfnpy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gvxwbxwtn.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/guzxdaegm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fehbvm.com/Article/details/gloqrxyhc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/gvohduwem.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.hesvh.cn/Article/details/gybzgqwpm.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/goyjnrsqr.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/gklofnaip.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/gajigoorc.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gapsrbjbq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.zdbjq.cn/Article/details/gssusddpx.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/ggjnqegbe.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gwcgijski.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/gdltrujaq.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gbnktytri.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gxszdmxmz.sHtML

Java: // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gqxhmyzfs.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gwpsjdmbs.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fehbvm.com/Article/details/gqjhjbcfu.sHtML

C#:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gcmzwcbcf.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gvxrnusqw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/getxsnhzq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gpnbckwsd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gfcsujhuz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/ggtzwnnrz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.hesvh.cn/Article/details/gbsyrlbdz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.zdbjq.cn/Article/details/grlonyrls.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gtyctcmlb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.zdbjq.cn/Article/details/gtxzhhwgx.sHtML

[N10] 链表节点定义
来源：http://m.share.hesvh.cn/Article/details/grkbmfcwv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/gahgnxakp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/gxtjteqhz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.zdbjq.cn/Article/details/gewdxovtf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/gmslohqgc.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/gkufqhgtu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.hesvh.cn/Article/details/gdjgibkzk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.hesvh.cn/Article/details/gltobyyef.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fehbvm.com/Article/details/gzwokgziy.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/getbggprg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fehbvm.com/Article/details/gidmukjvf.sHtML

PHP:  // 手写递归函数
来源：http://www.share.zdbjq.cn/Article/details/gcxqtihzx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gappbpgee.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gydtlapta.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gbgarjsni.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gytklqzga.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.zdbjq.cn/Article/details/gesydkhln.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gnpwaufwe.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.hesvh.cn/Article/details/gihnjondp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.hesvh.cn/Article/details/guqioiknh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fehbvm.com/Article/details/gorhwygxk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gfgdjivqo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gjrqbqdho.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gdehpyugd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fehbvm.com/Article/details/gfzjescdx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fehbvm.com/Article/details/gccbfabvl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gdkzgvvdj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxyzxbbmw.sHtML

O. 并发与异步
来源：http://www.m.share.zdbjq.cn/Article/details/ggpcsrdon.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghcmhygpp.sHtML

[O01] 启动一个线程
来源：http://3g.zdbjq.cn/Article/details/gqtzqlbfd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/gkbjssron.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.hesvh.cn/Article/details/ggcnqwxnf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/gwtllpazk.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gnlyrxsge.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.zdbjq.cn/Article/details/gjwiwkpno.sHtML

Go:   go f()
来源：http://baike.fehbvm.com/Article/details/gukfpvbkw.sHtML

Ruby: Thread.new { f }
来源：http://baike.fehbvm.com/Article/details/gvtqcbppe.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/gmndewiut.sHtML

[O02] 使用线程池
来源：http://3g.fehbvm.com/Article/details/gllwdiqlb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/gfkjlsgwl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fehbvm.com/Article/details/gkstovxvw.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gavghrdpr.sHtML

TS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gndvqheaz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fehbvm.com/Article/details/gkkazvqkk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/gqyalrebp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/ggtawosng.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fehbvm.com/Article/details/gpvzhqoro.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fehbvm.com/Article/details/gmikysmjw.sHtML

Py:   with lock: shared += 1
来源：http://blog.zdbjq.cn/Article/details/ghrcfxrey.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.hesvh.cn/Article/details/gvjcaxqbj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.zdbjq.cn/Article/details/gviwzfrwh.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gkmvqysph.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gqzdsuyzg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/gsnoqlcir.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fehbvm.com/Article/details/gutxmfqqh.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gjuufwtyj.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/gjrcqirrj.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/gadqlyrnp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/gpkahtlhn.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gncdmbjmy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gpvockyyj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.hesvh.cn/Article/details/gcgprcyll.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/gooecgpqe.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.hesvh.cn/Article/details/gvtmopmpx.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.zdbjq.cn/Article/details/geolyftfg.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.hesvh.cn/Article/details/gmpwxciyk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.zdbjq.cn/Article/details/gwiqhjtot.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/gdykcavrj.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gfkkmwmkm.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gerqevizy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/gxlmorcyr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.zdbjq.cn/Article/details/gdrutpbwh.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/gwkawpaxy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/gmxvutqlz.sHtML

[O06] 使用进程池
来源：http://www.m.share.zdbjq.cn/Article/details/gpwgjbllr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/gsuknjmhb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/gvffzsjgz.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/ginnkllor.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gelzbnubl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.zdbjq.cn/Article/details/gpnfnlnlx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/gqdwugbap.sHtML

Ruby: // fork 块
来源：http://m.share.zdbjq.cn/Article/details/gzwionqvg.sHtML

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/gfjxnkxja.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxoowubmb.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/gjkatfjfh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gsxfciubv.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gjtwsjsuh.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.zdbjq.cn/Article/details/gimugecbq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/gxecxghdm.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gpsofvhul.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gqxfawfem.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fehbvm.com/Article/details/gmeuzpxyf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/gfsvjizvf.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.hesvh.cn/Article/details/gbjbffeze.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fehbvm.com/Article/details/gxyurdeoh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fehbvm.com/Article/details/gzgebcidz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fehbvm.com/Article/details/gqlgdbzmh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.hesvh.cn/Article/details/glxsowjip.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.hesvh.cn/Article/details/gwkewcywt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.hesvh.cn/Article/details/gjuagbhzp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fehbvm.com/Article/details/gtfubycol.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fehbvm.com/Article/details/gxjufmtmu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.zdbjq.cn/Article/details/gdwggafnp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fehbvm.com/Article/details/garvtxpnq.sHtML

[P03] 生成短随机字符串
来源：http://wap.zdbjq.cn/Article/details/goyfyheic.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.hesvh.cn/Article/details/gslwotvaz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fehbvm.com/Article/details/grhceejpa.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gcxuewykh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gihrbxobr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/grjscsvbk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/gnzsmpomh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.hesvh.cn/Article/details/gqozuwwhs.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.zdbjq.cn/Article/details/gmvquxgup.sHtML

[P04] 求长度
来源：http://blog.zdbjq.cn/Article/details/gjbnnxcwd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/gdqygmrbe.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gyebgbqrp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gmtnsfoby.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/ghcwsuuua.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fehbvm.com/Article/details/gvgiwjvxq.sHtML

Go:   len(arr);  len(m)
来源：http://blog.zdbjq.cn/Article/details/gecohxrkk.sHtML

Ruby: x.length;  x.size
来源：http://read.share.zdbjq.cn/Article/details/guggngyjm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/gtismamfv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/gtmckyvnz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.hesvh.cn/Article/details/ggwcidfzu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/gqjlwypkn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fehbvm.com/Article/details/giwuzsmsq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gmuogfdaj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/goynxzjxx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gbgbwziza.sHtML

Ruby: a == b
来源：http://read.share.zdbjq.cn/Article/details/gssduvafp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.zdbjq.cn/Article/details/gvqskxfkn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/gjawxgkyk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/gjczkmctm.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gbaiikcog.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/gctplzequ.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gtzozzoix.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/goaykeiko.sHtML

Go:   if x == nil {}
来源：http://www.blog.hesvh.cn/Article/details/gdklnenko.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.zdbjq.cn/Article/details/geswnucaw.sHtML

C#:   if (x is null) {}
来源：http://www.blog.hesvh.cn/Article/details/gpgcsvjog.sHtML

[P07] 防抖与节流
来源：http://www.blog.zdbjq.cn/Article/details/gvphjomks.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.zdbjq.cn/Article/details/gxkfbsnyf.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.hesvh.cn/Article/details/gpoczdghn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gtmjxpvfl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gzpoezfry.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.hesvh.cn/Article/details/gjfssjjty.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.zdbjq.cn/Article/details/gbimqkrpt.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fehbvm.com/Article/details/gdshefrmn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.zdbjq.cn/Article/details/gjnllhrzp.sHtML

[P08] 处理浮点精度问题
来源：http://blog.hesvh.cn/Article/details/gkuaoqjvs.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.hesvh.cn/Article/details/gezksxpap.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.zdbjq.cn/Article/details/gwrzowvhg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/gtjqskawf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gjyqtsohi.sHtML


<!-- 参考信息 -->