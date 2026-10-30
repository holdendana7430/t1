代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.zdbjq.cn/Article/details/graxndtbb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fehbvm.com/Article/details/gcztvwppp.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggvdozohw.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fehbvm.com/Article/details/gdnorjvsz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtkotwjjb.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/glubhcncd.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fehbvm.com/Article/details/ghhaoyfhp.sHtML

PHP:  $argv;  $argc;
来源：http://blog.zdbjq.cn/Article/details/ghvcgaxle.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gwcuttwsd.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gwugdckdv.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fehbvm.com/Article/details/gnmhyhawd.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gtpgvrutx.sHtML

Ruby: ARGV
来源：http://mobile.hesvh.cn/Article/details/ggddmrbgc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gluvnowzs.sHtML

[M02] 读取环境变量
来源：http://3g.zdbjq.cn/Article/details/ghvscxkmi.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.hesvh.cn/Article/details/gucjzdczj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gdapxrvyy.sHtML

JS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gxvzefvbi.sHtML

TS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/glhzpjndg.sHtML

Java: System.getenv("HOME")
来源：http://wap.fehbvm.com/Article/details/gqxrnedxr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.hesvh.cn/Article/details/giiotvbuk.sHtML

Ruby: ENV["HOME"]
来源：http://baike.hesvh.cn/Article/details/ginmlwqpq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.hesvh.cn/Article/details/gwwnwalrv.sHtML

[M03] 执行外部命令
来源：http://read.share.zdbjq.cn/Article/details/gqyauewqj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fehbvm.com/Article/details/gvmlggtks.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.hesvh.cn/Article/details/gvtfemmcs.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gntevgjev.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gkebkeevd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/gtdfrnvhp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fehbvm.com/Article/details/goqpgvgdm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/ghwikzpyj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.hesvh.cn/Article/details/gotlitnak.sHtML

[M04] 获取当前工作目录
来源：http://baike.zdbjq.cn/Article/details/gtlomnzwo.sHtML

Py:   os.getcwd()
来源：http://baike.hesvh.cn/Article/details/gsdvwzkmn.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gafjvzyob.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/ghnmcedgi.sHtML

TS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gvdgibzav.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/gbunzmkvs.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/ggdlayypk.sHtML

Ruby: Dir.pwd
来源：http://wap.hesvh.cn/Article/details/gpofljceh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.zdbjq.cn/Article/details/ghrfwjilr.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/gpufwtzaw.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gznmimwge.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/gazaddrgm.sHtML

JS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/glmdkqpub.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gufmcvtpf.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gbiaaueqf.sHtML

Go:   os.Exit(1)
来源：http://3g.hesvh.cn/Article/details/gwysiypne.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/ghjhseked.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/ghsfegxth.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/gokfrvgzn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gneiblvvq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.zdbjq.cn/Article/details/gtwovluvk.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gfdojbnzi.sHtML

TS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gusknldqo.sHtML

Java: System.err.println("err")
来源：http://wap.zdbjq.cn/Article/details/gktqrmysw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.zdbjq.cn/Article/details/gbpmwqujt.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gmdaryszf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fehbvm.com/Article/details/gszteotcx.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/ghhdyvrjr.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.hesvh.cn/Article/details/gessalywi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fehbvm.com/Article/details/gvzyjkcdj.sHtML

JS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gxgunrrzc.sHtML

TS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gbqmxqhln.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fehbvm.com/Article/details/gnshbucfs.sHtML

Go:   func main()
来源：http://blog.zdbjq.cn/Article/details/gzcaapwgn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/giflvejtq.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fehbvm.com/Article/details/gblmtzsha.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/gfawzmdeo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.hesvh.cn/Article/details/giwmvssti.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.hesvh.cn/Article/details/gahmozide.sHtML

JS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gfpxqpbnm.sHtML

TS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gnytybrrh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.zdbjq.cn/Article/details/ghqxwdnaz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/gvlxyfyoz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gswuqchwg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/gebrzddjf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gaxrpahzr.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/gvshvmxhj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkbqqcdur.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fehbvm.com/Article/details/ggycqgulh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/girbjhuof.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/gsrbjoakr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gwltrknmf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gtafcworg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gjxaubclk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.hesvh.cn/Article/details/gqsygyjke.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fehbvm.com/Article/details/gueurpnsg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gqttwdaiw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.zdbjq.cn/Article/details/gsafxpdbu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gircxqcls.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gimvqwvxl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gnmpdeulc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gitfvgyih.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/gfqynzwrp.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gbfulrgma.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/ggeoifaiv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fehbvm.com/Article/details/ghjhfxdwx.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/gabzesfeo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/gubwhaocs.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.hesvh.cn/Article/details/gfswkuxel.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/ghxvbvlyv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gdruzmtzb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.hesvh.cn/Article/details/gtemebmvg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.hesvh.cn/Article/details/grtqprpyo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.zdbjq.cn/Article/details/gptsbukkl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.hesvh.cn/Article/details/gfzzhbkck.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/ghulxtijn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gkbmuetsf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/grngkvsou.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gvzemlnsy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gnvrlgwam.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gvdwdvhhl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/gcvjnsxqc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gpwgtlwpo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/ggrmzxubu.sHtML

[N05] 最大公约数
来源：http://mobile.zdbjq.cn/Article/details/ghnkgvfaz.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fehbvm.com/Article/details/gnsmanxcg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/gyhjyfndr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gimdvxdkm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gmegkbuoz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/gncemcesx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fehbvm.com/Article/details/gmsjpwyjf.sHtML

Ruby: a.gcd(b)
来源：http://baike.hesvh.cn/Article/details/gogmlmsbp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.hesvh.cn/Article/details/gwafnoiqp.sHtML

[N06] 判断回文字符串
来源：http://m.share.hesvh.cn/Article/details/ggforfdmm.sHtML

Py:   s == s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gxozozrqu.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gdrfvktde.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gcwpnrqxa.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gdmcgscmq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/gzfozwtwm.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fehbvm.com/Article/details/guydoaqpd.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/glxjkprok.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/grvrywvus.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.zdbjq.cn/Article/details/gnnkhsdop.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/glhnmfwxd.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.zdbjq.cn/Article/details/gnoxeuesz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/gltfqgzqc.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fehbvm.com/Article/details/gfkoiebvi.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/gvfmxnbew.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/gujbrrnzi.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fehbvm.com/Article/details/gwuqwfcqw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/gfyfixcnh.sHtML

[N08] 生成全排列
来源：http://baike.fehbvm.com/Article/details/gngjmzjty.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gbsqzmyno.sHtML

PHP:  // 手写递归交换
来源：http://read.share.hesvh.cn/Article/details/gtgcmxzht.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gbtebjjbi.sHtML

TS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gwrokqqxn.sHtML

Java: // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gxyzunbgl.sHtML

Go:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gphgcodjm.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.hesvh.cn/Article/details/gdxmgerwx.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gmpxihakb.sHtML

[N09] 栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gukkoedfd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gmdhjpyeq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/ggnphxlju.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gzozfpyzm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fehbvm.com/Article/details/gqjwzggvx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/gjezjakpp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.zdbjq.cn/Article/details/gpwepahgs.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/grjrvmftv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gbtolcbsl.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/gjnljxycf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.hesvh.cn/Article/details/givqmaqoh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/gvqegxhya.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.hesvh.cn/Article/details/gjmthetkz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/gghnjkyuo.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.hesvh.cn/Article/details/gudyfofoy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/godywvzfs.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/gfkiwurci.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/geasrighs.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fehbvm.com/Article/details/gptadcdno.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.zdbjq.cn/Article/details/glbennmfc.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.hesvh.cn/Article/details/gnhqilqvq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gbfokyxks.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gdjjitukt.sHtML

Java: // 手写递归
来源：http://wap.fehbvm.com/Article/details/gkldikjuw.sHtML

Go:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gtfgaskmf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/glvwlxdgw.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gbbvwfoup.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/gbwsdyuzr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/guyjjxeef.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/glgywbpyq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gotmkproi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/guiddrftd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gpthpjiuq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/gbmgncahy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fehbvm.com/Article/details/glkbpbkne.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/ggxsyesnj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmivrvsox.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/gduzzwqxz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpzzttspx.sHtML

[O01] 启动一个线程
来源：http://mobile.zdbjq.cn/Article/details/gsaxtqqlf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/ggoaqkybs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/gkagefygp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/gxttkmich.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/guzowyojb.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fehbvm.com/Article/details/gnmsgxdfy.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/gcgnigqan.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fehbvm.com/Article/details/gwojeumen.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/gjwlhogdr.sHtML

[O02] 使用线程池
来源：http://mobile.hesvh.cn/Article/details/gueerplae.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fehbvm.com/Article/details/gncvrwhfx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fehbvm.com/Article/details/gwylufxbi.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gpxxhihbe.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gqgixqbyu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.zdbjq.cn/Article/details/gsegwigfp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/gnmtcnnnx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.zdbjq.cn/Article/details/gmzmynqgc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/gzdgujbls.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/geefumiqp.sHtML

Py:   with lock: shared += 1
来源：http://m.share.hesvh.cn/Article/details/gufiayjrj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/gwfhdzvyy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.hesvh.cn/Article/details/gtkdcfkxo.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gdjfrtdjp.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gmhbhygok.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/giqupeuut.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/gsdiwpmas.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gigrxfeyh.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/ggfvpywzs.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fehbvm.com/Article/details/gcnfllyrp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/gaanefspi.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gxqanfpye.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/glwwzocsr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/gehlbxrtb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.zdbjq.cn/Article/details/gbmrvlmcv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.hesvh.cn/Article/details/gyzvgvunl.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.zdbjq.cn/Article/details/gaxyfqpzz.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.zdbjq.cn/Article/details/ghdzqttax.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/gjofhppak.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fehbvm.com/Article/details/gukorlwtp.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gojpcnmsl.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gtdteyppn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.hesvh.cn/Article/details/gghoiazfo.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/gwzlybcpg.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gncbxvelt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fehbvm.com/Article/details/gjboelvna.sHtML

[O06] 使用进程池
来源：http://www.m.share.hesvh.cn/Article/details/gekhucaca.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.zdbjq.cn/Article/details/gmoayhgvo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/glclfeeeg.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gimgwexmg.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gbpxphbys.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fehbvm.com/Article/details/gqvwxysis.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.zdbjq.cn/Article/details/gnsupqjjt.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/gawpjezja.sHtML

C#:   Parallel.For
来源：http://www.blog.zdbjq.cn/Article/details/gwtodecpw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqltjkzjs.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/gxbjyaluy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghdhxhjid.sHtML

[P01] 生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gkcvyhjxm.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fehbvm.com/Article/details/gafrwaifm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fehbvm.com/Article/details/gjrmoydga.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gxiccfyfk.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gcnliiscw.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fehbvm.com/Article/details/gfygjxnkm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fehbvm.com/Article/details/gaxesufzw.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/gqliaywfy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fehbvm.com/Article/details/gthoatmyv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.hesvh.cn/Article/details/gybvgoczg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/gsmozxxhz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.hesvh.cn/Article/details/gysnwhaaf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.zdbjq.cn/Article/details/gwxmqgdjn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.hesvh.cn/Article/details/gewhxolsm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gjljaamkq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fehbvm.com/Article/details/geexytyly.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fehbvm.com/Article/details/gizndeshw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/gdsrihjam.sHtML

[P03] 生成短随机字符串
来源：http://blog.fehbvm.com/Article/details/gvusplaov.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/geinuldnh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/gifxlgcpc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gpvjaisjo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/griancvxp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fehbvm.com/Article/details/gkyodafsg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fehbvm.com/Article/details/glyqsstno.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/gwnexfevm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.hesvh.cn/Article/details/gditstptn.sHtML

[P04] 求长度
来源：http://baike.zdbjq.cn/Article/details/gxkynmyon.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/gabvxumnu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gislcemzn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gkpfaudrf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gwjghhtue.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gziunjfyu.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.zdbjq.cn/Article/details/goarfmtjo.sHtML

Ruby: x.length;  x.size
来源：http://wap.hesvh.cn/Article/details/gnoeybbsp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fehbvm.com/Article/details/ggjffrcdm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/gbkrsvyea.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.hesvh.cn/Article/details/gsfuidrpg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.zdbjq.cn/Article/details/gamrjfbqx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fehbvm.com/Article/details/gffbpcpfy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gnjcoppov.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.zdbjq.cn/Article/details/gievhrzsu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/gihrsenzd.sHtML

Ruby: a == b
来源：http://read.share.zdbjq.cn/Article/details/gqxnsvvap.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.hesvh.cn/Article/details/gsunbfjiy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.zdbjq.cn/Article/details/gfduttyvo.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.hesvh.cn/Article/details/gsqckcqbh.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gorkjyxmz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fehbvm.com/Article/details/ggwdooehr.sHtML

TS:   if (x == null) {}
来源：http://www.share.fehbvm.com/Article/details/grzlvfubk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gmwwuzcuw.sHtML

Go:   if x == nil {}
来源：http://m.share.zdbjq.cn/Article/details/gvktepsxg.sHtML


<!-- 参考信息 -->