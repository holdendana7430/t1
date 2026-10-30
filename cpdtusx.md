代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gwpkasyfz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.fehbvm.com/Article/details/guyaoosgu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gofiahgqz.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.zdbjq.cn/Article/details/gfrkannns.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfejhayot.sHtML

[M01] 读取命令行参数
来源：http://read.share.hesvh.cn/Article/details/gelkhnwoi.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gvqfwjcuc.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fehbvm.com/Article/details/gottobqtq.sHtML

JS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/guofxqzdq.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gkfxvuupi.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gbcojpsyh.sHtML

Go:   os.Args[1:]
来源：http://baike.hesvh.cn/Article/details/gicjfhnca.sHtML

Ruby: ARGV
来源：http://wap.zdbjq.cn/Article/details/gkjabeldp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gkznxbizv.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gkddcgjti.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gyrhhwjht.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gkmewsrsb.sHtML

JS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/ghormdpxz.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gurvpoynn.sHtML

Java: System.getenv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gkbyytfpq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gxehqedag.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fehbvm.com/Article/details/gnbofrxmn.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gjmpgqvyx.sHtML

[M03] 执行外部命令
来源：http://3g.fehbvm.com/Article/details/gpecewtuv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.zdbjq.cn/Article/details/gjoedbwaq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/gajbmcamv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/ghcxowdal.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gsdunzxko.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/giupyjkug.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/gvalofvcr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fehbvm.com/Article/details/gpxgocvpo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.hesvh.cn/Article/details/gnjadnwae.sHtML

[M04] 获取当前工作目录
来源：http://baike.hesvh.cn/Article/details/gamyymceb.sHtML

Py:   os.getcwd()
来源：http://3g.fehbvm.com/Article/details/grgewwbdd.sHtML

PHP:  getcwd();
来源：http://www.blog.zdbjq.cn/Article/details/gfclzzdmq.sHtML

JS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gasarmyxs.sHtML

TS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gwnmqxybj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.hesvh.cn/Article/details/gernaboig.sHtML

Go:   os.Getwd()
来源：http://m.share.fehbvm.com/Article/details/gizogxxtw.sHtML

Ruby: Dir.pwd
来源：http://blog.fehbvm.com/Article/details/goszjtuqz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/gkfddnfkn.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/gfjyufyhn.sHtML

Py:   sys.exit(1)
来源：http://m.share.fehbvm.com/Article/details/givwkwwnv.sHtML

PHP:  exit(1);
来源：http://read.share.fehbvm.com/Article/details/ghdpccjyi.sHtML

JS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gjiclyvmx.sHtML

TS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/ggkqkqter.sHtML

Java: System.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gcsdbnbqu.sHtML

Go:   os.Exit(1)
来源：http://3g.hesvh.cn/Article/details/gissdcrgw.sHtML

Ruby: exit 1
来源：http://wap.hesvh.cn/Article/details/gxiqyrvet.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/gtojvbsvi.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/glwqpesjy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gtvaavjfm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.hesvh.cn/Article/details/ghigjbzkm.sHtML

JS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gobnmyswb.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gdsyjrbty.sHtML

Java: System.err.println("err")
来源：http://m.share.hesvh.cn/Article/details/gawsgssna.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.hesvh.cn/Article/details/ghuhznvcq.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/gjwlrzirw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.zdbjq.cn/Article/details/guhprnwzw.sHtML

[M07] 判断是否为主入口
来源：http://3g.fehbvm.com/Article/details/grkokmtsx.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.zdbjq.cn/Article/details/ggbmwaqwj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.zdbjq.cn/Article/details/gjpwawvdm.sHtML

JS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gxthvkbcr.sHtML

TS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gwaymawni.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/gjkuzcxcf.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/gpapletmz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/gzfymctuv.sHtML

C#:   static void Main(string[] args)
来源：http://wap.zdbjq.cn/Article/details/guyjkfubd.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.zdbjq.cn/Article/details/gvvzutqho.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/gjopbyxme.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/glhpzbfea.sHtML

JS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gvnygjmza.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/ghkcaarhi.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.hesvh.cn/Article/details/giufzakoj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.zdbjq.cn/Article/details/gzdzgwome.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/grsfsnajd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fehbvm.com/Article/details/guhtggwex.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gccqmtkqk.sHtML

N. 数据结构与算法
来源：http://baike.hesvh.cn/Article/details/gwpyqgskg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxxonzqoz.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.zdbjq.cn/Article/details/gktnnovgw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.hesvh.cn/Article/details/gxodltwgn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gvudhgmwi.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gljpfwzxt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gaeyofvnk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gpfqynmuz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.hesvh.cn/Article/details/gaqvwtvcu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.zdbjq.cn/Article/details/gvwrgnsmh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gnhuhzllk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/gphdpwxwv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gcbfgdarz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.hesvh.cn/Article/details/guzrkegfh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gifcagtsj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gckegwfui.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/gjdojqpuv.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gmwkqiszv.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gypvihdmw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.hesvh.cn/Article/details/grtiskzyi.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/gyfydvyza.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.hesvh.cn/Article/details/gqfcmxhnw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/gjcbgmwaz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gfdpefrha.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/giuosloaa.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fehbvm.com/Article/details/gifcdxccd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/gtqgtfgka.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gdddvjkjk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.hesvh.cn/Article/details/gebebzzjn.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gqikrrlme.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gojuywudz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/guecovcou.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gtfyfdamp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gzhxrbvqu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gijxkahop.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/gdspzsbhs.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gepotojoa.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gmlpsqqiu.sHtML

[N05] 最大公约数
来源：http://blog.zdbjq.cn/Article/details/gvqyyyetk.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gxgjtxhps.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/gsbreefwe.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gydyploii.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gnpirrzim.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/gyavcclls.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fehbvm.com/Article/details/grpwcpzul.sHtML

Ruby: a.gcd(b)
来源：http://blog.zdbjq.cn/Article/details/gwucpruiv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/gplsbhbit.sHtML

[N06] 判断回文字符串
来源：http://3g.hesvh.cn/Article/details/gaufvqfbh.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/ggwszloma.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/gvjlomqvl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gqjazvctm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gsoycdpzh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fehbvm.com/Article/details/guguazsgy.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/gmjimesef.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/gbywezfis.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gohxivxmd.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/gvimhjgez.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gnzdafkou.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/gefzjdnsx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fehbvm.com/Article/details/gwgynsvdc.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.zdbjq.cn/Article/details/gbuhfseql.sHtML

Java: // 手写 HashMap
来源：http://baike.fehbvm.com/Article/details/gdsemxnxp.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/gvlvmfjnc.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/gihxnfwmt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fehbvm.com/Article/details/gcmvqcgxm.sHtML

[N08] 生成全排列
来源：http://3g.fehbvm.com/Article/details/gwvhkhhxu.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fehbvm.com/Article/details/gkbzsowfi.sHtML

PHP:  // 手写递归交换
来源：http://www.share.hesvh.cn/Article/details/gvkloyruc.sHtML

JS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gikccfcaa.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gzudbmmry.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/giktchpht.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gfkztqfjb.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.zdbjq.cn/Article/details/gpeixtfmm.sHtML

C#:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gofaevukt.sHtML

[N09] 栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gtjeqpdly.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/gslryhlhj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/glboyicwm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gfsrnjfub.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/gsxgzyxty.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gbiukhhdm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fehbvm.com/Article/details/gjtzywulp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gkadfftlv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gdyiorvse.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/gphtzmjot.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/gcglalczm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/glwtonyke.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.hesvh.cn/Article/details/gvxmqswwg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/gaxjscycx.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fehbvm.com/Article/details/gndriebpp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.hesvh.cn/Article/details/gkmeslmvy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/gikcfmbwt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.hesvh.cn/Article/details/gkmxcvbtz.sHtML

[N11] 二叉树中序遍历
来源：http://3g.zdbjq.cn/Article/details/gcwpdzhzk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.zdbjq.cn/Article/details/gjulxflio.sHtML

PHP:  // 手写递归函数
来源：http://www.share.hesvh.cn/Article/details/gscodgkbb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gzlniqhnj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/galperype.sHtML

Java: // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gxcvwjkoy.sHtML

Go:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gzwaudzfr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.zdbjq.cn/Article/details/gdukrajwh.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gbcaxbkiz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.hesvh.cn/Article/details/gueqyionl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gktezedrc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/gitcacili.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/goidjypsv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gleokntjt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gvklxdnly.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/gxaalkuds.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/grgytjfdz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gslfwmnqr.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxaazeuty.sHtML

O. 并发与异步
来源：http://read.share.fehbvm.com/Article/details/ggrjstrxn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnmyhfnyu.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/gvfgbvrit.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fehbvm.com/Article/details/gphcvrjbs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fehbvm.com/Article/details/glblutkso.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/guwfflxsf.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gsniemzsc.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.hesvh.cn/Article/details/gjcuhkwhz.sHtML

Go:   go f()
来源：http://read.share.fehbvm.com/Article/details/gtvleqvfj.sHtML

Ruby: Thread.new { f }
来源：http://www.share.hesvh.cn/Article/details/glmfncvdz.sHtML

C#:   Task.Run(() => F());
来源：http://3g.zdbjq.cn/Article/details/gxsqzlnsa.sHtML

[O02] 使用线程池
来源：http://read.share.zdbjq.cn/Article/details/ggdpslqul.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/gdzjsueqq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fehbvm.com/Article/details/gduawdqox.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gdjcyoayt.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gvzzgylpf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.zdbjq.cn/Article/details/ggbnqsqvk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/genisywrd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.zdbjq.cn/Article/details/guztpjeql.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.hesvh.cn/Article/details/gkydhyjdm.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fehbvm.com/Article/details/gwjkhomqt.sHtML

Py:   with lock: shared += 1
来源：http://mobile.zdbjq.cn/Article/details/gdxwqwfne.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.hesvh.cn/Article/details/gopsiacpw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fehbvm.com/Article/details/gyikmynko.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gyofuruvi.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gdzqlnblf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fehbvm.com/Article/details/gjvuycbyo.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.hesvh.cn/Article/details/ggewcsyxy.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gxicuijxp.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fehbvm.com/Article/details/gvoenocbn.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/gxfvmjjku.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/gwnebbhki.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gverphldh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gozssffyd.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.hesvh.cn/Article/details/gooelajpq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.hesvh.cn/Article/details/ggnnlbcfp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.zdbjq.cn/Article/details/glkzplpas.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/gmwbulooy.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/gurgkycxm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.hesvh.cn/Article/details/gfrjjxbnb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/gomrslyxc.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gpddavwdp.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gsezekzdi.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.hesvh.cn/Article/details/gmpkfpfci.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.zdbjq.cn/Article/details/gmdzmogmj.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.hesvh.cn/Article/details/gywggezlz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/gisajbroc.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/gitgcuaxp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fehbvm.com/Article/details/guzufwiqe.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/gapyndqgh.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/giugsfhkw.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gpinptxol.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.hesvh.cn/Article/details/gaxghmevs.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/gndhoknvi.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/gpelxepqu.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/givayiean.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwldxhpms.sHtML

P. 常用工具函数
来源：http://wap.fehbvm.com/Article/details/ggkpbmtzs.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbzpuqklf.sHtML

[P01] 生成 UUID
来源：http://wap.zdbjq.cn/Article/details/gdmdobgrc.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fehbvm.com/Article/details/gubzbwjhk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gepappbyp.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gflxkwicm.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gmhvoskoy.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/gtnivplcn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.hesvh.cn/Article/details/gllofrexu.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fehbvm.com/Article/details/gbvgsqcsj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.hesvh.cn/Article/details/gpiuabkom.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/ghjxafbtw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/grurdlecl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.hesvh.cn/Article/details/goxeugkat.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.zdbjq.cn/Article/details/gvkgdxrbu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fehbvm.com/Article/details/gurbflfjs.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gqzcduaer.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.zdbjq.cn/Article/details/gtjkikimt.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/goqotfsce.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/gwsmhoxit.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/goudwvpzs.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.hesvh.cn/Article/details/gvwdfgfeu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.zdbjq.cn/Article/details/gzcktdncb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/guawudnfo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gmlemboss.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.hesvh.cn/Article/details/gnyicynss.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fehbvm.com/Article/details/geufybves.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/gprforsgc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fehbvm.com/Article/details/gcvpopwzl.sHtML

[P04] 求长度
来源：http://blog.hesvh.cn/Article/details/gxrkwyfrx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.zdbjq.cn/Article/details/gfvjlwxku.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/ghfmszyzu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/glpdqvqbr.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gwpoxvylu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fehbvm.com/Article/details/ggegxcavs.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.hesvh.cn/Article/details/grwrcgwir.sHtML

Ruby: x.length;  x.size
来源：http://www.share.zdbjq.cn/Article/details/gmbmxjpfc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/gdttvpkgv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/gxkvheooj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.hesvh.cn/Article/details/gbcsjlvqb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/gagsyqtbk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.zdbjq.cn/Article/details/goxirgjea.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/giovfpxtz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.hesvh.cn/Article/details/getxawjdy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fehbvm.com/Article/details/gmjpblbnb.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/gddwatvfs.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.zdbjq.cn/Article/details/glmlrjbub.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.hesvh.cn/Article/details/gyimxpjmt.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.hesvh.cn/Article/details/gtbovhzuy.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.hesvh.cn/Article/details/gbwmascvd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fehbvm.com/Article/details/gjswlxqea.sHtML

TS:   if (x == null) {}
来源：http://www.share.zdbjq.cn/Article/details/gzbzrxdpx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gixxrbgyk.sHtML

Go:   if x == nil {}
来源：http://www.m.share.hesvh.cn/Article/details/gsjaokdhi.sHtML


<!-- 参考信息 -->