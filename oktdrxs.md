代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fehbvm.com/Article/details/gaznchcei.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.hesvh.cn/Article/details/gtndqcnwf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gssywaxxj.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.hesvh.cn/Article/details/gnfvuhdjg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gekevhqor.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/gpyyacpif.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.fehbvm.com/Article/details/gljfflfot.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fehbvm.com/Article/details/gcojwgmwt.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gwruxhiat.sHtML

TS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gvesrobjo.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gmaqpdblq.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/gpyikiwzm.sHtML

Ruby: ARGV
来源：http://mobile.hesvh.cn/Article/details/gbcnuaiuq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gnorwlqeg.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/glmmwokpp.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.hesvh.cn/Article/details/gvlrxxypd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gocigenwh.sHtML

JS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gjxnhompk.sHtML

TS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/grwmfmrka.sHtML

Java: System.getenv("HOME")
来源：http://baike.fehbvm.com/Article/details/gyiaxjmti.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.hesvh.cn/Article/details/gpwwtfiku.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fehbvm.com/Article/details/gznyzmzke.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/goleolldj.sHtML

[M03] 执行外部命令
来源：http://www.m.share.zdbjq.cn/Article/details/gtjmmyouv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.zdbjq.cn/Article/details/ghlvpappn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.hesvh.cn/Article/details/giwjputdw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gygtoljei.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gfkuzyuby.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/gkuuekwud.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/gppmhibuu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fehbvm.com/Article/details/gzcwnvbue.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/gfbawajrq.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.zdbjq.cn/Article/details/gilgkvjhp.sHtML

Py:   os.getcwd()
来源：http://baike.fehbvm.com/Article/details/gmqbmtacy.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/ginxkpbmg.sHtML

JS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/giznnrcun.sHtML

TS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gzilwnxoa.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fehbvm.com/Article/details/ggmljhahy.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/gjlysxynx.sHtML

Ruby: Dir.pwd
来源：http://3g.hesvh.cn/Article/details/gftpkwmdm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.hesvh.cn/Article/details/gttsvveyp.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/gfqfmiggs.sHtML

Py:   sys.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gkqwohokt.sHtML

PHP:  exit(1);
来源：http://m.share.fehbvm.com/Article/details/gggsbhkoi.sHtML

JS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gvhlwjgdg.sHtML

TS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gwunnwpgl.sHtML

Java: System.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gcgbxtmef.sHtML

Go:   os.Exit(1)
来源：http://m.share.hesvh.cn/Article/details/gpvdbovzb.sHtML

Ruby: exit 1
来源：http://baike.fehbvm.com/Article/details/gonfsotqu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.zdbjq.cn/Article/details/gmjikyfkj.sHtML

[M06] 向标准错误输出
来源：http://read.share.zdbjq.cn/Article/details/ghigoabou.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gayaqesad.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.zdbjq.cn/Article/details/gznfpbbzv.sHtML

JS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gufprydcj.sHtML

TS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gwvcjqohc.sHtML

Java: System.err.println("err")
来源：http://blog.zdbjq.cn/Article/details/ghntfyjjv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/gyguthbcm.sHtML

Ruby: warn "err"
来源：http://wap.fehbvm.com/Article/details/gdiacxqps.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/gnavmzlno.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/glewfhshz.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/gvmydjijp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.zdbjq.cn/Article/details/geiwidtjz.sHtML

JS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gwxxfksnq.sHtML

TS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gcnqqeczi.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fehbvm.com/Article/details/gtehvranw.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/grntbsfmn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.hesvh.cn/Article/details/gotswebeh.sHtML

C#:   static void Main(string[] args)
来源：http://wap.zdbjq.cn/Article/details/godltbsia.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.zdbjq.cn/Article/details/gpfgfmatm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.hesvh.cn/Article/details/gjcvhhcly.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.zdbjq.cn/Article/details/gmzjgwada.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/giwlmzpky.sHtML

TS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gbpnknitw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/gwggxctme.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/gqlafffyg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fehbvm.com/Article/details/gbjfidone.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fehbvm.com/Article/details/gvbzkbtwb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gamffvdtx.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/gzlcluycv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggtrmmrom.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/gtlqhhqdj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fehbvm.com/Article/details/gtgygzjpv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gbwyddxve.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/geauzztcm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/guaqzaxsr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gkclbyzct.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gzkpndphh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/gnzjdmrch.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gkdlmpwxp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/giwiblxft.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gamcgbyuj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/gnljfxatl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gfvgikgil.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/ghbzpixeb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/ghvpyvlou.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gcsznxcht.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/glungiyvt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.zdbjq.cn/Article/details/gzxmrxexr.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fehbvm.com/Article/details/gayvyihvy.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/gbrunxnru.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/gsuqynpat.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/glwmsjswp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/guedjigdx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/gynkraece.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.hesvh.cn/Article/details/gxxvkbday.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.zdbjq.cn/Article/details/gbpwrornb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/gttoncqct.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/gnplvrnnt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gtwgqmtar.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.hesvh.cn/Article/details/ggnhwoppf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/grwrawhdw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/ggpuodgzk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gopjzipwg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.zdbjq.cn/Article/details/gxafxvqfo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gimtzkvop.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gtqhcziuy.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/gachcphbb.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fehbvm.com/Article/details/grnekmney.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.zdbjq.cn/Article/details/ghnfllftq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxbdkicts.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gvhcqcjlr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/gwvbzfqpg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/griyacldh.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/gkmovxsos.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/guvykdulo.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fehbvm.com/Article/details/gzrnioilq.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gippqyzdq.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/glrineara.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gpjikdiam.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gfqpyofoh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/golxinosv.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/gndudyyrg.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/gbcfauwyf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gtmzqkqwg.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.hesvh.cn/Article/details/gauvonlqg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.hesvh.cn/Article/details/gbkdbxcks.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/gldxmtpog.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/gwfayuxld.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/gdkwrmdgp.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/gjtxjiork.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/guqwmhzdc.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.hesvh.cn/Article/details/guaeyhyjp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/gubcdndtc.sHtML

[N08] 生成全排列
来源：http://m.share.zdbjq.cn/Article/details/gmlpfcgtl.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.zdbjq.cn/Article/details/gxtgpfgzc.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.zdbjq.cn/Article/details/gwglptjva.sHtML

JS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gkbheafwv.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gmxhmzhhh.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gehgqgpap.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gltdlybtb.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fehbvm.com/Article/details/ggprougcy.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gerzfrjly.sHtML

[N09] 栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gvvkzlpci.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/gajeguxjk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gpgtjhjgb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gzvgcgbgg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/gxcqdtcwa.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/guhxhfxew.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fehbvm.com/Article/details/grgwpujrn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/grcwktahg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/gbgxkrude.sHtML

[N10] 链表节点定义
来源：http://www.m.share.hesvh.cn/Article/details/giplvknwa.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/gwhtxjdgn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.zdbjq.cn/Article/details/gyqnopfce.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/gtssjwvqc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.zdbjq.cn/Article/details/gpadhgwuw.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.zdbjq.cn/Article/details/ggbszfxgd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/glplqdzka.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gbemqalbh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/gpsfeodkh.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gopqlmrdb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/gpxvyubnu.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gbebmhudk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gskcfkzpu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gkadrfygv.sHtML

Java: // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gajkfkhzf.sHtML

Go:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gjmpuuink.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/gfotlqeqm.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/glxctemif.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.hesvh.cn/Article/details/gxlkuqacj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.zdbjq.cn/Article/details/gsqhlulvr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.hesvh.cn/Article/details/gcuuulbuj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/ggruclzzn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gmebprvhh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gdjsxmuhg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/gdzsycpzf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.zdbjq.cn/Article/details/gljohkvtm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gactavvrh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfxfzirfp.sHtML

O. 并发与异步
来源：http://read.share.fehbvm.com/Article/details/grzklrfyj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxypxqhav.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/gstmjligy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/gfvtriwpw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/gzavqtqag.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/gwwufuytt.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gpdrlbdny.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/gsuilgavd.sHtML

Go:   go f()
来源：http://3g.zdbjq.cn/Article/details/gesmszksc.sHtML

Ruby: Thread.new { f }
来源：http://m.share.zdbjq.cn/Article/details/gqqcbjxea.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.hesvh.cn/Article/details/gvqhpgpwb.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/grtswsrud.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/gcbitsvvj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.zdbjq.cn/Article/details/glxifbjkv.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gijryrvag.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gwneythna.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/gynujwqbv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fehbvm.com/Article/details/gyswshill.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/gdhrksnja.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/gyzvdtklo.sHtML

[O03] 加锁保护共享数据
来源：http://3g.zdbjq.cn/Article/details/gbaqewltz.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gwhrqmysq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.zdbjq.cn/Article/details/gedqscrcs.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.hesvh.cn/Article/details/gydopykrx.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gyfqevxiq.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gipogsngt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fehbvm.com/Article/details/gcleiqwyu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fehbvm.com/Article/details/ggmfbtoho.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.hesvh.cn/Article/details/ghklepido.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.zdbjq.cn/Article/details/gupgnyaye.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.zdbjq.cn/Article/details/gfxisvwov.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fehbvm.com/Article/details/gjjejmxvz.sHtML

JS:   async function f() { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gzoyjhpxt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.hesvh.cn/Article/details/gxljkhxul.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/gojwytdlp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.zdbjq.cn/Article/details/gjrwxdakg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/gdylradnx.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.zdbjq.cn/Article/details/gogxdpedq.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.hesvh.cn/Article/details/gnixwasry.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/gthodbotf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fehbvm.com/Article/details/ggyyaaqwd.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gzjuomcjl.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gdezgkgzd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fehbvm.com/Article/details/gntbwafpo.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fehbvm.com/Article/details/gkpnrwubv.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/glifjudzq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gpogcsfho.sHtML

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/gxfiorjfq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.zdbjq.cn/Article/details/gpkfprowc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.hesvh.cn/Article/details/gerwrxbtm.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gkwejqgso.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gqqdicpsm.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.hesvh.cn/Article/details/gohpfffrw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/gjmnghzqa.sHtML

Ruby: // fork 块
来源：http://mobile.fehbvm.com/Article/details/gkajieukt.sHtML

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/gzdfbojhb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gemthjkqc.sHtML

P. 常用工具函数
来源：http://www.share.hesvh.cn/Article/details/gtqlmaaye.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjjrrwszv.sHtML

[P01] 生成 UUID
来源：http://3g.hesvh.cn/Article/details/gtvprmwas.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/gbohgxats.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.zdbjq.cn/Article/details/gbiwffwqy.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gyjrbtpab.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gzkdqwsae.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.hesvh.cn/Article/details/gicgwqgrl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.zdbjq.cn/Article/details/gctkojdxl.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/gtwhyblay.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.zdbjq.cn/Article/details/guwtwetui.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fehbvm.com/Article/details/ghoobfckd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fehbvm.com/Article/details/gtqrhagzj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.hesvh.cn/Article/details/gybgplfbs.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.hesvh.cn/Article/details/gfqwwtkma.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.zdbjq.cn/Article/details/ghtrjdhsx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fehbvm.com/Article/details/gqfnmckll.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.hesvh.cn/Article/details/gjgzrwhmp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/gnemqbkqm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.zdbjq.cn/Article/details/gfmhcwjdd.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/gxrqykxti.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fehbvm.com/Article/details/ghmbzhysd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/gfqmdyasi.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gbjlnlhlm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gginoukhv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.zdbjq.cn/Article/details/gjhbvklbj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/gpluldiub.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fehbvm.com/Article/details/gtacuxcnk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fehbvm.com/Article/details/giwpbkyak.sHtML

[P04] 求长度
来源：http://blog.hesvh.cn/Article/details/gygyvjmsq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.hesvh.cn/Article/details/gxhncrsto.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gppxmiqjh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gjtfqeojz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gsncsgyse.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gczolhkad.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.zdbjq.cn/Article/details/gqghgugde.sHtML

Ruby: x.length;  x.size
来源：http://blog.fehbvm.com/Article/details/gguqeclxu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gcwccervv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.hesvh.cn/Article/details/gnxzttznm.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.zdbjq.cn/Article/details/gcyxcyqnz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fehbvm.com/Article/details/gzjysmurl.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.zdbjq.cn/Article/details/gurrdptxq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gcjtsijxu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/guovtrqig.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.hesvh.cn/Article/details/gzvvwkoyz.sHtML

Ruby: a == b
来源：http://wap.hesvh.cn/Article/details/gpaedmemp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/gmbzlocqs.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.zdbjq.cn/Article/details/gcmdacrax.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/grfkgfwkw.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fehbvm.com/Article/details/gawfsnsfz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/gtjxqxgho.sHtML

TS:   if (x == null) {}
来源：http://baike.fehbvm.com/Article/details/gocmwndew.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gvegrbzvx.sHtML

Go:   if x == nil {}
来源：http://www.m.share.hesvh.cn/Article/details/gbnurzogv.sHtML


<!-- 参考信息 -->