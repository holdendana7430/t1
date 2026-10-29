代发 wailian999

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqelridct.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/gtwcxgeyt.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/gdrmnvznw.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.zdbjq.cn/Article/details/gkikyobde.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gylsntnvr.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/ghnuyqrje.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gpixjwdrr.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gycolmbbo.sHtML

Ruby: ARGV
来源：http://baike.fehbvm.com/Article/details/goybansbx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gqnccgdvo.sHtML

[M02] 读取环境变量
来源：http://wap.fehbvm.com/Article/details/ggezympxz.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.hesvh.cn/Article/details/ggwpprwqq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gpuoqeomr.sHtML

JS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gwivccrri.sHtML

TS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gfvnvtlfg.sHtML

Java: System.getenv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gojnqweaz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.hesvh.cn/Article/details/grwcmbsje.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.hesvh.cn/Article/details/gdvmmhldl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.hesvh.cn/Article/details/gxlhhwjws.sHtML

[M03] 执行外部命令
来源：http://www.blog.hesvh.cn/Article/details/gewhofvtf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gymzuollw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fehbvm.com/Article/details/gtnpnxpza.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gdddxtyzn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gmgckaqda.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.hesvh.cn/Article/details/gzzgiwton.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.hesvh.cn/Article/details/gkpnstzjv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gyezgtapd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.zdbjq.cn/Article/details/guzigihnt.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/ggudqjkvr.sHtML

Py:   os.getcwd()
来源：http://3g.fehbvm.com/Article/details/glzinrfgd.sHtML

PHP:  getcwd();
来源：http://3g.fehbvm.com/Article/details/grppstzbl.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gxmxmtphw.sHtML

TS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gxsuhhogq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fehbvm.com/Article/details/gfvrbtmgt.sHtML

Go:   os.Getwd()
来源：http://www.share.hesvh.cn/Article/details/grewtqpgi.sHtML

Ruby: Dir.pwd
来源：http://www.share.zdbjq.cn/Article/details/gsfqyxgpq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/guguocjox.sHtML

[M05] 设置退出码
来源：http://3g.zdbjq.cn/Article/details/guruihpiv.sHtML

Py:   sys.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gfjtzprab.sHtML

PHP:  exit(1);
来源：http://www.blog.fehbvm.com/Article/details/gjbfnrkii.sHtML

JS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gpgzgrwys.sHtML

TS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzqxxskhz.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/ghdskhbem.sHtML

Go:   os.Exit(1)
来源：http://mobile.fehbvm.com/Article/details/gtjyozvhi.sHtML

Ruby: exit 1
来源：http://read.share.hesvh.cn/Article/details/gvgvxqxfd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fehbvm.com/Article/details/gjoluoszb.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/gizgkyxcu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gvicbwfwe.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/gozczdqit.sHtML

JS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gnvxmrmxw.sHtML

TS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gbgztcyuo.sHtML

Java: System.err.println("err")
来源：http://wap.hesvh.cn/Article/details/gnlpbgcpr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.zdbjq.cn/Article/details/grslfikzs.sHtML

Ruby: warn "err"
来源：http://baike.hesvh.cn/Article/details/gmpbvzeil.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/gmkrxhyki.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/gxzmarltw.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fehbvm.com/Article/details/gnewnqqqf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/gimvhcwbs.sHtML

JS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gqpccqyyw.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gcivbwkaz.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/gqztsyazg.sHtML

Go:   func main()
来源：http://www.share.zdbjq.cn/Article/details/gflucayxk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/gbtzreana.sHtML

C#:   static void Main(string[] args)
来源：http://wap.zdbjq.cn/Article/details/gtdamxyzf.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/ggcsiiify.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.zdbjq.cn/Article/details/ghzuzpcxv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fehbvm.com/Article/details/gqcjkhcrk.sHtML

JS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gtpvlkskd.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/glljgbxyb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fehbvm.com/Article/details/gnhpmkbot.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/grcqddisp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/gaigdfcxn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/gnwcupwfx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpwjfeuou.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/gjihgbodn.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gphvvftwk.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.hesvh.cn/Article/details/gjnxnjnnm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gvqrraepu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fehbvm.com/Article/details/gulgpwrrd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gxsexjjhk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/ghonuvpsc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gxluqombw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.hesvh.cn/Article/details/gnpmeygzg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/gfrvwanre.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/glukjrgky.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.zdbjq.cn/Article/details/gxltpfibk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gxwrqkbfv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fehbvm.com/Article/details/gqagojacs.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/glhnzwaad.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gtmnjvjkf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.zdbjq.cn/Article/details/gumaujlrd.sHtML

Go:   slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gnxfzpniq.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/glggveagq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gqsisknot.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.hesvh.cn/Article/details/gvnveazno.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/giqdrznxp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/gmyqupibm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gddbvlhyg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gyufwbuqg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.zdbjq.cn/Article/details/gyxushngg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fehbvm.com/Article/details/gtpfojsgy.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/ggilfownk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/gdrnsdvza.sHtML

[N04] 斐波那契数列
来源：http://read.share.hesvh.cn/Article/details/gkiobswwa.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gsxedexiz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/giclktvqh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/ghycksfww.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gsaxwbepq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gqojgxrhc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.zdbjq.cn/Article/details/gprvhpcof.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gbuhkrwfj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gdonorkje.sHtML

[N05] 最大公约数
来源：http://www.share.fehbvm.com/Article/details/gotejyedp.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gadjhvfcg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/gxwozjfoq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gvjgjghcn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gbcmuldea.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.hesvh.cn/Article/details/ggbdjzojb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fehbvm.com/Article/details/grwbndfyw.sHtML

Ruby: a.gcd(b)
来源：http://mobile.hesvh.cn/Article/details/grlrrnptm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.zdbjq.cn/Article/details/gynmqqfpx.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gpbswlkyz.sHtML

Py:   s == s[::-1]
来源：http://wap.hesvh.cn/Article/details/gvefdfuoz.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/gsgcdulxp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gzrmslrjl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gwbztctfw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fehbvm.com/Article/details/gsmdfshym.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.zdbjq.cn/Article/details/gjkjejgzc.sHtML

Ruby: s == s.reverse
来源：http://wap.zdbjq.cn/Article/details/ggukxasay.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/ghtwrongc.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.hesvh.cn/Article/details/gsalotnpr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/gaphgaxaw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fehbvm.com/Article/details/gnpatsgbv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.zdbjq.cn/Article/details/grczrysjw.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.zdbjq.cn/Article/details/goescfzva.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/ggrykgady.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.zdbjq.cn/Article/details/gkwwnixyj.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/gycnftvkb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/gwctykexw.sHtML

[N08] 生成全排列
来源：http://m.share.zdbjq.cn/Article/details/glvsqonfb.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.fehbvm.com/Article/details/gcyrcbhbu.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/gsnwzglem.sHtML

JS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gohmocjul.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/grehzjvnh.sHtML

Java: // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gcnyllfnc.sHtML

Go:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/ghfmyflil.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/gaixervhp.sHtML

C#:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gnfrgprrk.sHtML

[N09] 栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gbrtuingd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gyjansbmd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gfygdocdl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gneraivrb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.zdbjq.cn/Article/details/gipfbjrvm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gcdhyjwrl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/gpnlbunao.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gurmyaopu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/gdkgyovtp.sHtML

[N10] 链表节点定义
来源：http://www.share.zdbjq.cn/Article/details/gmravafsx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.zdbjq.cn/Article/details/gxfzrnnkx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.zdbjq.cn/Article/details/gcbtoevet.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fehbvm.com/Article/details/gtdvcptsv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.fehbvm.com/Article/details/gtcptojxk.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtdwwffym.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.zdbjq.cn/Article/details/gselwkuaw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fehbvm.com/Article/details/gqpsgdujf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/gmdbyeriy.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.hesvh.cn/Article/details/gqekafuha.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fehbvm.com/Article/details/gdugbfbof.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gfdwnayrx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/ggtongxfo.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gstheowmv.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gwhstbzls.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/ggbnhxpac.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/gehetygwk.sHtML

C#:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gwouvnmba.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.hesvh.cn/Article/details/gicbccaeq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.hesvh.cn/Article/details/gdzojkvhf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.hesvh.cn/Article/details/gcmavtllz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/guhsmyzng.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gisnzkyos.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gumneulel.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.hesvh.cn/Article/details/gkiasxfdn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/gnsutppkp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/ggbunslbo.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gfreylswx.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/gqlzslhpj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghdxuulpi.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/gfxpthyan.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/geyffruxz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/gfsslkpvn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gpnlvtmrv.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gzsdhqyno.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.zdbjq.cn/Article/details/ghbvjzpmd.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/gzxooizyq.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/gxhodicif.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/gjoxeoynd.sHtML

[O02] 使用线程池
来源：http://www.share.hesvh.cn/Article/details/gjbzifheb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.hesvh.cn/Article/details/gpuwjgnck.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/guqdpojal.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gvbankmzn.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gxlnqakmt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/gmlogldpe.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.zdbjq.cn/Article/details/guqtqdsog.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fehbvm.com/Article/details/grlahevxl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.zdbjq.cn/Article/details/gtdhvjtaz.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fehbvm.com/Article/details/gaglvrtpl.sHtML

Py:   with lock: shared += 1
来源：http://baike.zdbjq.cn/Article/details/godredenr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gumyuciaf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.zdbjq.cn/Article/details/genbyvfhb.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gtwcviuwx.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gvamidgxx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.zdbjq.cn/Article/details/gdtqhjsdd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fehbvm.com/Article/details/gfiurwvuh.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gyoejwizc.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/gmivbjrlj.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/godyxnxrd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/grujccbev.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gfwzvzwml.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/gkhpcwhhs.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.hesvh.cn/Article/details/gdwfrshky.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fehbvm.com/Article/details/grsfgfazm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.hesvh.cn/Article/details/gganqeowu.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/gbcmjfopg.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fehbvm.com/Article/details/gbqdztgjh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fehbvm.com/Article/details/gooeaxido.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.hesvh.cn/Article/details/ghpaetgfl.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gnludoaak.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gpdxotcuc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fehbvm.com/Article/details/ggkktejux.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.hesvh.cn/Article/details/giodqjvta.sHtML

Ruby: threads.map(&:join)
来源：http://blog.zdbjq.cn/Article/details/ggauwhuhc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.zdbjq.cn/Article/details/gsahztiyu.sHtML

[O06] 使用进程池
来源：http://m.share.hesvh.cn/Article/details/gaqbfquqx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fehbvm.com/Article/details/gjpgcattd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fehbvm.com/Article/details/gxokzbnsg.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gfsdrlgxr.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gfojihzgh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gutygrmdc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.hesvh.cn/Article/details/gogvcvook.sHtML

Ruby: // fork 块
来源：http://m.share.hesvh.cn/Article/details/gfeeohoyt.sHtML

C#:   Parallel.For
来源：http://www.blog.hesvh.cn/Article/details/gdnvavmxy.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkevxttlc.sHtML

P. 常用工具函数
来源：http://read.share.hesvh.cn/Article/details/gdvffdlkv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gukykrkpg.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gsofivupl.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fehbvm.com/Article/details/gbmqspgpa.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.hesvh.cn/Article/details/guuomseyg.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gpafspllv.sHtML

TS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gydraglih.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/gmhwzatff.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/gnaztgazl.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.hesvh.cn/Article/details/gjhjtrsqu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/glojwdvdc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.zdbjq.cn/Article/details/gyvhhdfzb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fehbvm.com/Article/details/gclmxihgl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fehbvm.com/Article/details/gmhnucvjf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fehbvm.com/Article/details/gprfuqymc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fehbvm.com/Article/details/gqnoxgxft.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fehbvm.com/Article/details/gapmcfcif.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/gekqjknmu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.hesvh.cn/Article/details/gmjtfbjgs.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/goupxvjsa.sHtML

[P03] 生成短随机字符串
来源：http://m.share.zdbjq.cn/Article/details/glorgnmir.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/gbxjqohfo.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/gsybehrdz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gdeefcxjr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gigfpxebv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fehbvm.com/Article/details/gqgfevzyr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.zdbjq.cn/Article/details/gfgtbmydk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.zdbjq.cn/Article/details/gvdpbwzjd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fehbvm.com/Article/details/gpgifyrzw.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/gctvwfone.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.zdbjq.cn/Article/details/gcgkhrgdc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gymmgwako.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gzncysbpo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gvihdsreq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fehbvm.com/Article/details/gtupuqnyx.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fehbvm.com/Article/details/gpipmhxmc.sHtML

Ruby: x.length;  x.size
来源：http://m.share.hesvh.cn/Article/details/gnogquuls.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.hesvh.cn/Article/details/gtnekmcbt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.hesvh.cn/Article/details/gvkgnufbv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/gkyovtmur.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.hesvh.cn/Article/details/gveggbekt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fehbvm.com/Article/details/goppfxzjs.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gzlsvtrkj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.zdbjq.cn/Article/details/gyaewycfv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fehbvm.com/Article/details/gfhwlwlow.sHtML

Ruby: a == b
来源：http://www.share.zdbjq.cn/Article/details/ggnexccsv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fehbvm.com/Article/details/gmfsnmxyb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fehbvm.com/Article/details/gcgmcakey.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.hesvh.cn/Article/details/gjdhfeovr.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gbkzsubbi.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.zdbjq.cn/Article/details/gpsmiqpxm.sHtML

TS:   if (x == null) {}
来源：http://www.blog.zdbjq.cn/Article/details/ggvozejod.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gcudaebth.sHtML

Go:   if x == nil {}
来源：http://www.share.hesvh.cn/Article/details/gcjikihoo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/gsadybpfg.sHtML

C#:   if (x is null) {}
来源：http://www.share.hesvh.cn/Article/details/gfgtijxvw.sHtML

[P07] 防抖与节流
来源：http://read.share.zdbjq.cn/Article/details/gnopnukmc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.zdbjq.cn/Article/details/ghzhfbdgd.sHtML


<!-- 参考信息 -->