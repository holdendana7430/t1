代发 wailian999

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxpqzzcdq.sHtML

[M01] 读取命令行参数
来源：http://read.share.hesvh.cn/Article/details/gvlcarpbs.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.hesvh.cn/Article/details/guzcgdeky.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fehbvm.com/Article/details/gewayeufu.sHtML

JS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/ghvpxymdr.sHtML

TS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gluuaydeh.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gwahxntey.sHtML

Go:   os.Args[1:]
来源：http://m.share.zdbjq.cn/Article/details/gekripbsc.sHtML

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/gfchnntui.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gkmgcxtsj.sHtML

[M02] 读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gukhohqxt.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fehbvm.com/Article/details/ghnkscuir.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.hesvh.cn/Article/details/ggzmwgmkk.sHtML

JS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gbmgxcmgt.sHtML

TS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gkjnhiehd.sHtML

Java: System.getenv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gisloaoix.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fehbvm.com/Article/details/gvjvytwbu.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/gclrbmgqh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gcjkzeckn.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/gndusnctw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.hesvh.cn/Article/details/ghcqunysd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.zdbjq.cn/Article/details/gdbpkaahk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gprrotycq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gfkjgixqj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fehbvm.com/Article/details/ghaivahff.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/gjuwsbygp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/ghveejeee.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fehbvm.com/Article/details/grfmppxzh.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fehbvm.com/Article/details/gkiikzhcr.sHtML

Py:   os.getcwd()
来源：http://3g.fehbvm.com/Article/details/gllhmiqxi.sHtML

PHP:  getcwd();
来源：http://read.share.fehbvm.com/Article/details/gjlhseddj.sHtML

JS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gqxvpcwib.sHtML

TS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/ghkiewnvj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.zdbjq.cn/Article/details/glbhyifgg.sHtML

Go:   os.Getwd()
来源：http://wap.zdbjq.cn/Article/details/grizohucc.sHtML

Ruby: Dir.pwd
来源：http://mobile.hesvh.cn/Article/details/gfddcuclm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/gvyudrzxf.sHtML

[M05] 设置退出码
来源：http://3g.zdbjq.cn/Article/details/gaflxarcp.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gwtfjwkyr.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/guyzbfjqn.sHtML

JS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/goungnnxt.sHtML

TS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gqhiphpab.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/gsxltkeve.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gjprbbvzs.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/grmeugqto.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gotgpgrjc.sHtML

[M06] 向标准错误输出
来源：http://3g.fehbvm.com/Article/details/gpfdwxblm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/glsemwive.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/gytirrlci.sHtML

JS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gsmiwphfa.sHtML

TS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gjjqhzycx.sHtML

Java: System.err.println("err")
来源：http://3g.zdbjq.cn/Article/details/gzmzsqnql.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.zdbjq.cn/Article/details/gkgquqbqe.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/gbzxmznoj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.hesvh.cn/Article/details/goemonijx.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.hesvh.cn/Article/details/gjtemmdvb.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/gbawcbhnf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.zdbjq.cn/Article/details/glsdxgtzv.sHtML

JS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gfbyfjkds.sHtML

TS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gyiqfjgzb.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/gjnpelzbn.sHtML

Go:   func main()
来源：http://www.blog.hesvh.cn/Article/details/ghybzcpol.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.zdbjq.cn/Article/details/gpzlbxtgg.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.zdbjq.cn/Article/details/gwsfblvdw.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/ghncbefod.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/gmefuxfwi.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fehbvm.com/Article/details/gunfuapwe.sHtML

JS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gdskvqmrd.sHtML

TS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gykjephzc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/gwhzstwmy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.zdbjq.cn/Article/details/gkbmnmopx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.hesvh.cn/Article/details/glfxndvfh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/geuagooyx.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwwnfidbt.sHtML

N. 数据结构与算法
来源：http://www.blog.zdbjq.cn/Article/details/gkhmgbupi.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzlgiwjiq.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fehbvm.com/Article/details/gmihyiobw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/ghilvshbg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/gfxecsqoi.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gcxnolfmm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/ghipbwicp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gsfzohhzw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/glyllwcpd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fehbvm.com/Article/details/gsufbryco.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gsnfsywrq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/gkvhvbeik.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gbalxsypd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.zdbjq.cn/Article/details/gtoktmlrf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gdughewpr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gmacfmyuv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.zdbjq.cn/Article/details/gzcbtucuw.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gjflzzsgt.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gjlpcdbbb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.zdbjq.cn/Article/details/ggxkmccsn.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.zdbjq.cn/Article/details/grralyezj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.zdbjq.cn/Article/details/gtijzaebd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.hesvh.cn/Article/details/glhiwvwjz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gzfgmresy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/ghdyjxfjl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.hesvh.cn/Article/details/gymogskfe.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.hesvh.cn/Article/details/gkqniuram.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/glfmaulqo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.hesvh.cn/Article/details/grupvrrgg.sHtML

[N04] 斐波那契数列
来源：http://3g.fehbvm.com/Article/details/gofmlieid.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gjujkpzag.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gbefzlyjz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gdvtfxbig.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/guvmhiyzz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gcwabjhlq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.zdbjq.cn/Article/details/gjgiwpzbn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/grnrwmbar.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gjlsqiwtn.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/gjdaurldm.sHtML

Py:   math.gcd(a, b)
来源：http://wap.zdbjq.cn/Article/details/gbfcxjxln.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fehbvm.com/Article/details/gciwrnloa.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gbqlxcajp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcgpdrtbp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/gmdyjgyqo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gsazutjyx.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/ggjbxtlkv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/gfxuouqmt.sHtML

[N06] 判断回文字符串
来源：http://3g.hesvh.cn/Article/details/gtmeqrnkb.sHtML

Py:   s == s[::-1]
来源：http://wap.hesvh.cn/Article/details/gyxsmlanu.sHtML

PHP:  $s === strrev($s);
来源：http://blog.hesvh.cn/Article/details/gurkmurna.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gficioenk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gjxsndbye.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.hesvh.cn/Article/details/golsvvrhr.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/gmmkuzhxu.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/gepkmglcx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gpvzlgbdn.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.zdbjq.cn/Article/details/gzyfmkmhc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/ggtdcmhnh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.hesvh.cn/Article/details/glhlinjtf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.hesvh.cn/Article/details/gqwuhxzuc.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.hesvh.cn/Article/details/gqrsphqmx.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/gtejuskjj.sHtML

Go:   // 手写 map[int]int
来源：http://wap.hesvh.cn/Article/details/gouuzekxn.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fehbvm.com/Article/details/gemvcbuif.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/gutyvdsuv.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/geobmajlu.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/gpglsmbcx.sHtML

PHP:  // 手写递归交换
来源：http://m.share.hesvh.cn/Article/details/gjdditqqo.sHtML

JS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gdntmawqn.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gqvfiiiew.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gljtrzxfb.sHtML

Go:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gqgzqifor.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/gshflouwm.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gcodnzacx.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gjeiddpkv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fehbvm.com/Article/details/gzcfyiclh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/ggrpupdky.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gjjfdoacc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/gatlxznlw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gpjqlvjmu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/gdagztnrz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gxupaqprb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.hesvh.cn/Article/details/gchvkirps.sHtML

[N10] 链表节点定义
来源：http://wap.zdbjq.cn/Article/details/ggxlgrrhe.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fehbvm.com/Article/details/gdioppchz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fehbvm.com/Article/details/gfeszawkm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.hesvh.cn/Article/details/gshhyoyga.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.zdbjq.cn/Article/details/gdczwowbs.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjwwkelow.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/gkfmunzql.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/gvgtsdcjv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.zdbjq.cn/Article/details/gnbnuakqv.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fehbvm.com/Article/details/gynchxvjf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.hesvh.cn/Article/details/gtksvgrok.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.hesvh.cn/Article/details/gnooadjqw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/ghrnzusfx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gvljwnczb.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gohwqbcdf.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gunwwketr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.hesvh.cn/Article/details/gbmwwzvck.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/ggwivbmss.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.hesvh.cn/Article/details/giiqunnbs.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fehbvm.com/Article/details/gdsvvlajt.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.zdbjq.cn/Article/details/ghjbaudty.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/grprgzqhg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gqndfthwh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/guccfflml.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.hesvh.cn/Article/details/grjnyaivr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/gbrmtzldk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gklhniwbs.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gyanxqhlc.sHtML

O. 并发与异步
来源：http://read.share.fehbvm.com/Article/details/gokbhlbhi.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqcslocqo.sHtML

[O01] 启动一个线程
来源：http://www.share.fehbvm.com/Article/details/grvdvuvww.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.hesvh.cn/Article/details/gchjxqpqj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.zdbjq.cn/Article/details/gofsdiwzj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.zdbjq.cn/Article/details/gicycaoyc.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gdrqmbsaq.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/gmosdgeot.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/govwhdauo.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/gpyabatrh.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/gwbybwdht.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/gfgevkjiw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.zdbjq.cn/Article/details/gchtbuznj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.hesvh.cn/Article/details/grfaaqrgy.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gjdxxfois.sHtML

TS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gdiefmfqm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fehbvm.com/Article/details/gaugptzhe.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.zdbjq.cn/Article/details/gxqzbqpqe.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/ggtjwgewo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.hesvh.cn/Article/details/gibnglbqf.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/gwlakgaat.sHtML

Py:   with lock: shared += 1
来源：http://mobile.zdbjq.cn/Article/details/gsxaenjru.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/gbcepwfxq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/ghekrudkr.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gvnuzrfmw.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/genepyois.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.hesvh.cn/Article/details/gvkochjis.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.hesvh.cn/Article/details/gpjcvdhnc.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gauvnahyx.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.zdbjq.cn/Article/details/gwolekndu.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.hesvh.cn/Article/details/godxhrabf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/ggxonivln.sHtML

JS:   async function f() { await g(); }
来源：http://wap.hesvh.cn/Article/details/gwzhcxbdl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gcmogmvec.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/gstbstndm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.hesvh.cn/Article/details/gcehpvrpj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/gfxznosxk.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/gwialsskm.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.hesvh.cn/Article/details/gfceshhci.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fehbvm.com/Article/details/gxjfdlinf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/gpajzmbqa.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gfbzzdhti.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/glxgtldfn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/gdzghsooq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/gbusmffzw.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/gwqqvijzs.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/gkwiiozzb.sHtML

[O06] 使用进程池
来源：http://wap.hesvh.cn/Article/details/gradegstk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fehbvm.com/Article/details/gzzyrfbkj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/gtcqaycxc.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gwldmjeiq.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gdyddqvtj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.zdbjq.cn/Article/details/gwwpevthl.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/gzunpmmdk.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/gzqvsvsre.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/gkavphezg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkvwkgvln.sHtML

P. 常用工具函数
来源：http://baike.hesvh.cn/Article/details/gaebpsgzf.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfqquafni.sHtML

[P01] 生成 UUID
来源：http://3g.fehbvm.com/Article/details/gahnghyck.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/gnvfrekln.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.hesvh.cn/Article/details/gjxkwnpvn.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gthdzbwyd.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gzzfnjlhy.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gxdtbpemx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.zdbjq.cn/Article/details/glalrilrr.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/ghmjiosrt.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.zdbjq.cn/Article/details/gvlclxmem.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.hesvh.cn/Article/details/gtujycaoz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fehbvm.com/Article/details/gfdhygngb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/gzuicpfgh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.zdbjq.cn/Article/details/gnuwbhzqd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.hesvh.cn/Article/details/gadkblqgu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.zdbjq.cn/Article/details/guyegijvb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gxicjvynl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.zdbjq.cn/Article/details/gxxgmrchi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.zdbjq.cn/Article/details/gcoiawmml.sHtML

[P03] 生成短随机字符串
来源：http://blog.fehbvm.com/Article/details/gnoddexah.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fehbvm.com/Article/details/gzyprywhq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.hesvh.cn/Article/details/gymotkvvk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gyyghjhda.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gqpojdrei.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/gpvctbpdp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.hesvh.cn/Article/details/gftwfvfqz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/gmczgxqia.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/gftuuafif.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/gbnumcqih.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/gqsfynfra.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gjgmuprti.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/geiyakifw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gciarllvs.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fehbvm.com/Article/details/gjipqgtzb.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gimssiyhz.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/gozkljcor.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gpegaxmtk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.hesvh.cn/Article/details/gvajkskmd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.hesvh.cn/Article/details/gaesopzpg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.hesvh.cn/Article/details/gunjbimxe.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.zdbjq.cn/Article/details/gvqranjah.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gkdgfgfcy.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.zdbjq.cn/Article/details/gjyjtzmxg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.zdbjq.cn/Article/details/gbqthabrv.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/gpftkdltr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fehbvm.com/Article/details/grfibbayv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/gjcxgntel.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.zdbjq.cn/Article/details/grhdmvwtu.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gvoqmummb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/gpwauybji.sHtML

TS:   if (x == null) {}
来源：http://m.share.zdbjq.cn/Article/details/gpauroucl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gzysvzhtw.sHtML

Go:   if x == nil {}
来源：http://www.share.hesvh.cn/Article/details/gicaxhodk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fehbvm.com/Article/details/gwxagibpp.sHtML

C#:   if (x is null) {}
来源：http://read.share.hesvh.cn/Article/details/gcwnjhpcz.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/gpskfgoqb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fehbvm.com/Article/details/gilghnohu.sHtML


<!-- 参考信息 -->