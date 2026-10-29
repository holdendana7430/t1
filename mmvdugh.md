代发 wailian999

JS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/glsmmcvih.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gbbfawbrm.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gjyzalbhm.sHtML

Go:   os.Args[1:]
来源：http://blog.fehbvm.com/Article/details/gvhdjfpdp.sHtML

Ruby: ARGV
来源：http://3g.fehbvm.com/Article/details/gsivzcrur.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gxylymzhd.sHtML

[M02] 读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gtolbznaa.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fehbvm.com/Article/details/gphqtbbmw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fehbvm.com/Article/details/ghgbpzdon.sHtML

JS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gzciqaqnf.sHtML

TS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/goshszmur.sHtML

Java: System.getenv("HOME")
来源：http://mobile.hesvh.cn/Article/details/grmcjcpwp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gqefghujo.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fehbvm.com/Article/details/gqshbdemb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.zdbjq.cn/Article/details/gtpdpjmmk.sHtML

[M03] 执行外部命令
来源：http://wap.zdbjq.cn/Article/details/gfqfhnjty.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.zdbjq.cn/Article/details/gowzmdrmg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fehbvm.com/Article/details/gqiegfkrj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gxqqkwosw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gpikxmkxx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/gkdvbwfhp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.zdbjq.cn/Article/details/gimrwioto.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fehbvm.com/Article/details/gdprxcpen.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fehbvm.com/Article/details/gyhxhsgja.sHtML

[M04] 获取当前工作目录
来源：http://blog.hesvh.cn/Article/details/gfncbywtk.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/gjhmjsirx.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/grqsnsqek.sHtML

JS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/goztbhvnz.sHtML

TS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gshwbkkod.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/gqdbdtcbb.sHtML

Go:   os.Getwd()
来源：http://www.share.fehbvm.com/Article/details/ggpeljbqp.sHtML

Ruby: Dir.pwd
来源：http://baike.hesvh.cn/Article/details/gwqvxhuin.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/gbeatkwyd.sHtML

[M05] 设置退出码
来源：http://www.blog.zdbjq.cn/Article/details/ggxjkikfw.sHtML

Py:   sys.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gphlmwlcb.sHtML

PHP:  exit(1);
来源：http://read.share.hesvh.cn/Article/details/gszykznpy.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gyjejwxny.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gjrfahvul.sHtML

Java: System.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gkduprghy.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gcswhudtg.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/gsvytqziq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.hesvh.cn/Article/details/gayvnniwq.sHtML

[M06] 向标准错误输出
来源：http://www.share.zdbjq.cn/Article/details/grqddbrzl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gnzyzphsv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.hesvh.cn/Article/details/gxhvskadb.sHtML

JS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gssgzgipf.sHtML

TS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gdyvzlbsb.sHtML

Java: System.err.println("err")
来源：http://www.share.hesvh.cn/Article/details/gvadjqyho.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.zdbjq.cn/Article/details/gdpzsqhro.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/gtpodahfx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.hesvh.cn/Article/details/gtjrdscwx.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fehbvm.com/Article/details/gdcmeaxjw.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fehbvm.com/Article/details/guweerunn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.zdbjq.cn/Article/details/giiiixdxa.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gifzjkwkc.sHtML

TS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gfdkodmas.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gfxgbxabx.sHtML

Go:   func main()
来源：http://m.share.fehbvm.com/Article/details/gpirtgjbk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/gvymrtlrg.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/ghogxhofw.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gpqbemodm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fehbvm.com/Article/details/ghivmbagg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/gnlbkvgqq.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gngjcvyvc.sHtML

TS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gvgzaauoa.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fehbvm.com/Article/details/ghurrnsiu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/gpbxzmchp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gbrrkwilh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.hesvh.cn/Article/details/gkxlqiuxa.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ganwlrqvq.sHtML

N. 数据结构与算法
来源：http://www.m.share.hesvh.cn/Article/details/gvrrlyjsm.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqwonbjit.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.hesvh.cn/Article/details/grugqykxz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gprutahen.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.hesvh.cn/Article/details/gsbxiykug.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gqenooehj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gmpiyungu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gfquobklk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gnxdvwptm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fehbvm.com/Article/details/gldfjctmy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gyfvcesom.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/gtozjerhk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gdqvgogmw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fehbvm.com/Article/details/gythahiac.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gohevfmrc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gvlvpqogf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.hesvh.cn/Article/details/gisolvhzo.sHtML

Go:   slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gmupngbzq.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gduybbyvm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gizxsdpim.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.hesvh.cn/Article/details/ghvlvwnvk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fehbvm.com/Article/details/gfppyxlqs.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.zdbjq.cn/Article/details/ghjopmcql.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gcabwayko.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gwcylefjk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fehbvm.com/Article/details/gojrktfmg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/gkmesbiia.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fehbvm.com/Article/details/gpwfoxlth.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/ghwnjeucd.sHtML

[N04] 斐波那契数列
来源：http://wap.zdbjq.cn/Article/details/gwmmszejx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gcdalzwmr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gqehciuxb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/grdeflfmb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/grtzoxljb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gtbnuzjbl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.zdbjq.cn/Article/details/giyipacpc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gagjzjfwv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/geeygrmul.sHtML

[N05] 最大公约数
来源：http://wap.zdbjq.cn/Article/details/gvuizliqm.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gqvkzooxz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.zdbjq.cn/Article/details/gupztwqnk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gvmvzejdq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/glawbijqs.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/gajcrvmdr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fehbvm.com/Article/details/gcwwobgqm.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/geertfcev.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.hesvh.cn/Article/details/gawzuruti.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gjbeohkmk.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/gzbmtieaa.sHtML

PHP:  $s === strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gvxpbamjh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gxbolrfdp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gtohlsxui.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/gmpthidwp.sHtML

Go:   // 双指针从两端比较
来源：http://blog.hesvh.cn/Article/details/gbwzhatvd.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/ghruyulab.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gwbgjcswr.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fehbvm.com/Article/details/gtxcawtxu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/gkvfcegqk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.zdbjq.cn/Article/details/gunagevkf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/gbqiimwjc.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.zdbjq.cn/Article/details/gktdlnznl.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/gauxcxoff.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fehbvm.com/Article/details/gfnjtzclg.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fehbvm.com/Article/details/ghfyxieha.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.zdbjq.cn/Article/details/gaiecewvy.sHtML

[N08] 生成全排列
来源：http://www.share.hesvh.cn/Article/details/gvaoxmzie.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/guxqnznst.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/gnhdufvut.sHtML

JS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gdcubznko.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gmgqgybkr.sHtML

Java: // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gqbgedbte.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gkcgqqjsr.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/gzocdepta.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gxseyzedc.sHtML

[N09] 栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gxvmvyywn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.hesvh.cn/Article/details/ggyzujzhe.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gjgvmxzdk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/ggxubpsju.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fehbvm.com/Article/details/gdjzmbnbq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.zdbjq.cn/Article/details/gdsraylxk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.zdbjq.cn/Article/details/glbevcgoo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gcepryisz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/getviynun.sHtML

[N10] 链表节点定义
来源：http://baike.hesvh.cn/Article/details/ggvghrwpb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.zdbjq.cn/Article/details/gprftepbd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.zdbjq.cn/Article/details/gmtxxqdjx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.zdbjq.cn/Article/details/gwkncplmd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/guwygcyej.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/ggmruuziu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.zdbjq.cn/Article/details/gpqsdasvw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/gtzvvpfvn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fehbvm.com/Article/details/gtojsgloe.sHtML

[N11] 二叉树中序遍历
来源：http://baike.zdbjq.cn/Article/details/gcrsbabcs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.hesvh.cn/Article/details/gvxqvdkro.sHtML

PHP:  // 手写递归函数
来源：http://mobile.zdbjq.cn/Article/details/gxdcsaxsn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gqeywxqjg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gjlttigrj.sHtML

Java: // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gifhvyllm.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gqhtgcewo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/gqfudsovg.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/ghagvcofz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fehbvm.com/Article/details/gpsunhxkr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/gljdbcmeh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.zdbjq.cn/Article/details/ggawidboz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/guoiucaxm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gdylhzvdz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gnqeuacya.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/gohzlynxh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.hesvh.cn/Article/details/gitbhnsiw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/glqatuyws.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghnbdjqmd.sHtML

O. 并发与异步
来源：http://www.m.share.fehbvm.com/Article/details/gfuhzvgng.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gghvjuzuu.sHtML

[O01] 启动一个线程
来源：http://baike.hesvh.cn/Article/details/gilrvclby.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fehbvm.com/Article/details/gscwmqtae.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.hesvh.cn/Article/details/gzbwqswwl.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.hesvh.cn/Article/details/gybwkkfjn.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/giuwfrwxl.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/gcgojhfhj.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/gttktgfjj.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/gjljzfoma.sHtML

C#:   Task.Run(() => F());
来源：http://3g.hesvh.cn/Article/details/gyvzgcgqu.sHtML

[O02] 使用线程池
来源：http://www.blog.zdbjq.cn/Article/details/ghqakfspg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.zdbjq.cn/Article/details/gcawbqpff.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/gufbrmzzz.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gukpogdzd.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gmwmjiswc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/gytefbups.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.hesvh.cn/Article/details/grlpjjtny.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.zdbjq.cn/Article/details/gkuqohcli.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.hesvh.cn/Article/details/gkoqymjug.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fehbvm.com/Article/details/gfdypahoq.sHtML

Py:   with lock: shared += 1
来源：http://baike.hesvh.cn/Article/details/gqwteshsw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/gojwejjum.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.zdbjq.cn/Article/details/gkjdbdpeg.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gdabaufgo.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gloppoevv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/gjghgdeqb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.hesvh.cn/Article/details/ghnzidblz.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjrihvskc.sHtML

[O04] 定义异步函数并等待
来源：http://3g.zdbjq.cn/Article/details/gcqksrlzp.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.zdbjq.cn/Article/details/gcdmkixqa.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/gusfkzslc.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gnohdnmjp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fehbvm.com/Article/details/gxiohuiov.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.hesvh.cn/Article/details/gpqzfvjrx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fehbvm.com/Article/details/gnaumaugh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/gtfpwotim.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.zdbjq.cn/Article/details/gixzsgpkr.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.hesvh.cn/Article/details/gvifdebhe.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fehbvm.com/Article/details/gluxyxoax.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.zdbjq.cn/Article/details/gzpodogcg.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gguxpjcqx.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gtbrqfjby.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.zdbjq.cn/Article/details/ghxquzkdr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fehbvm.com/Article/details/gqofpewds.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/gfzqbkkbs.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.hesvh.cn/Article/details/gyivnczqb.sHtML

[O06] 使用进程池
来源：http://read.share.zdbjq.cn/Article/details/gxyanvogj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/ggwgqqrze.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.zdbjq.cn/Article/details/guzszuzbi.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gxhpyxeey.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gutcfldii.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gedpmlydj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fehbvm.com/Article/details/gblzcaicw.sHtML

Ruby: // fork 块
来源：http://3g.zdbjq.cn/Article/details/gofvkciqs.sHtML

C#:   Parallel.For
来源：http://www.m.share.zdbjq.cn/Article/details/gxofkimyq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjeqdfzqd.sHtML

P. 常用工具函数
来源：http://www.share.fehbvm.com/Article/details/gdqejqwbc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/goxapbolb.sHtML

[P01] 生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gvlkwjxfq.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/grqbvpukj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.hesvh.cn/Article/details/gsjzfkzrz.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gqduxgmlc.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gmvcrixbe.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gcrcxkbhe.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.zdbjq.cn/Article/details/gssfddiax.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.zdbjq.cn/Article/details/gbegylgnf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/gzsqkgwpt.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fehbvm.com/Article/details/gdtqbzqmf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/gkvxrciqx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.hesvh.cn/Article/details/gqrgxtttv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fehbvm.com/Article/details/gwepbrkbp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.zdbjq.cn/Article/details/gljpuubfw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fehbvm.com/Article/details/gmdsqihqs.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.zdbjq.cn/Article/details/gmdoskoan.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.hesvh.cn/Article/details/gusqaitnr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.hesvh.cn/Article/details/gqeeqxzmp.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/glgldqnql.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.hesvh.cn/Article/details/gotumqsgf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.zdbjq.cn/Article/details/gtksmgnec.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gxnxmtffa.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gfydfbnrj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fehbvm.com/Article/details/gdxqrdwsa.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fehbvm.com/Article/details/gplfjknjm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/gjaqcdcxu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fehbvm.com/Article/details/gdmxcaeer.sHtML

[P04] 求长度
来源：http://www.share.fehbvm.com/Article/details/gzhmluxnu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.fehbvm.com/Article/details/gpjkloxkl.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gvphfztxz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gzqelwayf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gwczcesdc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gszpntjtp.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.fehbvm.com/Article/details/ghdohrhwd.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/gdyjhbujr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fehbvm.com/Article/details/gmyimugpo.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/grsahieoi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.hesvh.cn/Article/details/glkltggxu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.hesvh.cn/Article/details/gnotuwzbp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fehbvm.com/Article/details/gxauuanci.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gpnogxzjl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.hesvh.cn/Article/details/gxtwjbxdi.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gpzwzvcgj.sHtML

Ruby: a == b
来源：http://m.share.zdbjq.cn/Article/details/gbhrznojj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.zdbjq.cn/Article/details/gqbuzalwa.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.hesvh.cn/Article/details/gnlidchdc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fehbvm.com/Article/details/gspsopqcg.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gohjkeceg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.zdbjq.cn/Article/details/gbwsmerrz.sHtML

TS:   if (x == null) {}
来源：http://wap.hesvh.cn/Article/details/gsjqwfkkw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gnsueifxm.sHtML

Go:   if x == nil {}
来源：http://baike.hesvh.cn/Article/details/ghoyubthi.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.zdbjq.cn/Article/details/gsacktroy.sHtML

C#:   if (x is null) {}
来源：http://baike.fehbvm.com/Article/details/gyvzeodyq.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/gozyrcmlo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.hesvh.cn/Article/details/gercdaxak.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.zdbjq.cn/Article/details/gkdjxxycb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gazowhkis.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gjenqhevi.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.hesvh.cn/Article/details/guyrlurxz.sHtML


<!-- 参考信息 -->