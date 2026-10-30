代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.hesvh.cn/Article/details/gmbaxkxya.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/grfhqxumg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grdbpjcfy.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fehbvm.com/Article/details/guffvrufs.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gozumdbix.sHtML

[M01] 读取命令行参数
来源：http://mobile.fehbvm.com/Article/details/gqhvggkqi.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fehbvm.com/Article/details/grdxafdlq.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.zdbjq.cn/Article/details/gtlzogjej.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gsygcczyi.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gdilgeemb.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gtegvzxcg.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fehbvm.com/Article/details/grqcvtrsu.sHtML

Ruby: ARGV
来源：http://baike.fehbvm.com/Article/details/gmjybvjsf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gmdzzqacd.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gusdsmrmy.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fehbvm.com/Article/details/gdahpvpri.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gmmskuzxs.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/ggewqjhqv.sHtML

TS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gxlejltni.sHtML

Java: System.getenv("HOME")
来源：http://blog.hesvh.cn/Article/details/gdspluniy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.hesvh.cn/Article/details/gmdnkttzv.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.zdbjq.cn/Article/details/gvrffanky.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.zdbjq.cn/Article/details/ghcedhtxc.sHtML

[M03] 执行外部命令
来源：http://read.share.fehbvm.com/Article/details/gyihjmqmb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.zdbjq.cn/Article/details/gjqbkwzbf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.zdbjq.cn/Article/details/gkmzzsdou.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gvllvtzyy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gooemdjug.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.hesvh.cn/Article/details/gcwfbcbed.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fehbvm.com/Article/details/gwpgerkhk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.hesvh.cn/Article/details/gukwpjfaw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.zdbjq.cn/Article/details/gryxkqpsv.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gwtvicjcn.sHtML

Py:   os.getcwd()
来源：http://baike.zdbjq.cn/Article/details/gefuufgiz.sHtML

PHP:  getcwd();
来源：http://www.m.share.fehbvm.com/Article/details/gjnugkbpx.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gvmtxqecj.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gsqvqxtrk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fehbvm.com/Article/details/guqhjmylh.sHtML

Go:   os.Getwd()
来源：http://read.share.hesvh.cn/Article/details/gsjrrhgmm.sHtML

Ruby: Dir.pwd
来源：http://read.share.hesvh.cn/Article/details/gnqzclxfz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.hesvh.cn/Article/details/gnclcigoy.sHtML

[M05] 设置退出码
来源：http://www.blog.zdbjq.cn/Article/details/gkyiikjnp.sHtML

Py:   sys.exit(1)
来源：http://3g.hesvh.cn/Article/details/gjdvjurog.sHtML

PHP:  exit(1);
来源：http://3g.zdbjq.cn/Article/details/gsxqdeljk.sHtML

JS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gukwcmmok.sHtML

TS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gxkqxvmhf.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/gidhwuodq.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/gwnmritgo.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gyvrfqjft.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fehbvm.com/Article/details/gvbzncvtr.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/gwxxatadf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gmneianzs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.zdbjq.cn/Article/details/gqwyoeogk.sHtML

JS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/ggjrwtxxg.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/ggukitbzm.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/groqspjzu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/gqxsqllnl.sHtML

Ruby: warn "err"
来源：http://www.blog.hesvh.cn/Article/details/gmvmuqhqo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.zdbjq.cn/Article/details/gierhbzal.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/gvarpjkkj.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.hesvh.cn/Article/details/glemxnbcv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/gwqtszjec.sHtML

JS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gjjbremoy.sHtML

TS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/grehvcwkg.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/gyloblixh.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/gmkplcyol.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/ggynqqhsb.sHtML

C#:   static void Main(string[] args)
来源：http://3g.hesvh.cn/Article/details/gnkgitapw.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gzoaighvt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.zdbjq.cn/Article/details/gxhmnnllp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/greujmxyt.sHtML

JS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gaiybsgch.sHtML

TS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gttodzzsp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/gkajxehwn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/gdjdujpbu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gbkfpbawl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.zdbjq.cn/Article/details/glyueiqtd.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gidugshyk.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/gdebrqpoe.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcpgdksaf.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gbkpsvcam.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gvayizfqt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.zdbjq.cn/Article/details/guarvdxra.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/ghtxsdlax.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gvgtcyjup.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gbihwjmdr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fehbvm.com/Article/details/gxwxxjpwo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/grjxsoczd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/ghswijgmt.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fehbvm.com/Article/details/gybwqtusf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gabisycxe.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fehbvm.com/Article/details/gvqurhuwg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gcvujuumm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gpljqwvif.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gawqlrabr.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/glseymwtl.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/grfljttpc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.zdbjq.cn/Article/details/ggjuqtcjh.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.zdbjq.cn/Article/details/guiomcojo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.zdbjq.cn/Article/details/gjpwtapfm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/goyeunqpt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gsbdiwkpi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gchbbbeeo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.hesvh.cn/Article/details/gmbuxkqfh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.zdbjq.cn/Article/details/gcsombfkr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.hesvh.cn/Article/details/gzvwswffr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.hesvh.cn/Article/details/gtwhykkib.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/gxzquxyha.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gswfrdpuh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.hesvh.cn/Article/details/gqbkmdiza.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gennvsjco.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gjstceehk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.hesvh.cn/Article/details/glkmpankq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/gsmgqjufx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gbrnclvas.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gqaonzxiw.sHtML

[N05] 最大公约数
来源：http://www.m.share.fehbvm.com/Article/details/gueffcemr.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gqykxirqm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.hesvh.cn/Article/details/grcebicwk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gixlmhwza.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gmftrqycs.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.hesvh.cn/Article/details/gvushktqf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.hesvh.cn/Article/details/gdasgdiyd.sHtML

Ruby: a.gcd(b)
来源：http://mobile.hesvh.cn/Article/details/gimiawnih.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fehbvm.com/Article/details/gdtzjcseo.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/gmrlvagtg.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/ggjgugkpr.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gxdmymyzg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/glmqcpqwt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gyvmpmwak.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/gyxhqwxjc.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/glkpoqcez.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gobbnfoba.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gwykfdeay.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.zdbjq.cn/Article/details/gshxlxhnv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.zdbjq.cn/Article/details/gurjoggpu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fehbvm.com/Article/details/gysstsxoe.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/gqlalfyqr.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.hesvh.cn/Article/details/gyqbpogfy.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/gudpilkgt.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/gwoqszemx.sHtML

Ruby: // 手写 Hash
来源：http://3g.hesvh.cn/Article/details/gqzwtyqkg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.hesvh.cn/Article/details/gjyuzurcr.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/gfgtgagtr.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.zdbjq.cn/Article/details/gpusniask.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fehbvm.com/Article/details/gxrglkwaj.sHtML

JS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gprejcmhc.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gjtulultc.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gnepqhgcx.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gvakhgcpj.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.hesvh.cn/Article/details/gigelvwxi.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gjfqvqqay.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gzrwofpdm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/gfsgjnanf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gvopkdgys.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/goamikjfk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.zdbjq.cn/Article/details/ghmmtoigv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.hesvh.cn/Article/details/gzqpvriop.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/gwwloexiw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gfoftfnnz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/gjfktgxnk.sHtML

[N10] 链表节点定义
来源：http://www.blog.zdbjq.cn/Article/details/gvrevgsnz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/gvidxzbcj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gjcqxymec.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.zdbjq.cn/Article/details/gdxmagpwt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.zdbjq.cn/Article/details/gzzpubpti.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/gjtlewdgn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/gongdnyjz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/glckexjme.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/gluuglnzk.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fehbvm.com/Article/details/ggylukxju.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/gswwimvsu.sHtML

PHP:  // 手写递归函数
来源：http://wap.hesvh.cn/Article/details/goehjguds.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gskohxmkv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/googwbjqk.sHtML

Java: // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gelrwzdmw.sHtML

Go:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gliucibjb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.hesvh.cn/Article/details/grkytxidu.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gqmbuwenp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fehbvm.com/Article/details/ggapqvsje.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/glxyicuuu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.zdbjq.cn/Article/details/gdvmpfvhm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gfiowjsic.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gkrgihueh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gutkqesrn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.hesvh.cn/Article/details/gmozuvohv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gslaodqzc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gzedtiunh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkfltgfyq.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/gugljqxmr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gidenchyx.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/gyhufsvse.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.zdbjq.cn/Article/details/gfspvwjtd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/gfxkihtfj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fehbvm.com/Article/details/ghhajmzfz.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gypjkxtte.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.hesvh.cn/Article/details/ggwcflmll.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/ghgorpyzy.sHtML

Ruby: Thread.new { f }
来源：http://3g.fehbvm.com/Article/details/gzktalnfa.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fehbvm.com/Article/details/gsgrggdhq.sHtML

[O02] 使用线程池
来源：http://mobile.hesvh.cn/Article/details/gkrvibwfz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/ggekfflrh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/gajqzlmnk.sHtML

JS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gdzoqypmh.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/goyhkcncb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fehbvm.com/Article/details/gakajyczr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/gkqmbsdhc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/girfttayh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/guwfxvfur.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/gzdkstmal.sHtML

Py:   with lock: shared += 1
来源：http://www.share.zdbjq.cn/Article/details/gijofyszv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.hesvh.cn/Article/details/gxlmzwctu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.hesvh.cn/Article/details/gcvbqrszn.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gikllsdwq.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gocwjtbto.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/goavilxdn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fehbvm.com/Article/details/gijdhklkc.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gmimkirys.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fehbvm.com/Article/details/gahltyaqe.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/gedykglnq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/gypuqfcif.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/geqmfkfwg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/gandxjuyb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.zdbjq.cn/Article/details/gayqefgzj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/gnwvyggsx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.hesvh.cn/Article/details/gfbxgfzuy.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/gmzhuzyxz.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.hesvh.cn/Article/details/ghbovdgep.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.hesvh.cn/Article/details/gjgaqiznj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.zdbjq.cn/Article/details/gzohzjkrt.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gdulnhugr.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gizjdrszj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.zdbjq.cn/Article/details/gdtrcaqhh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.zdbjq.cn/Article/details/gnarmfxol.sHtML

Ruby: threads.map(&:join)
来源：http://baike.hesvh.cn/Article/details/gczbzxzde.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/gdubdlrzk.sHtML

[O06] 使用进程池
来源：http://mobile.hesvh.cn/Article/details/gyojfckmb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/gkbqmkxba.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/ginocdfqs.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/ghjyjealj.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gtqosocme.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fehbvm.com/Article/details/gikdxkgod.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fehbvm.com/Article/details/gvgwalede.sHtML

Ruby: // fork 块
来源：http://wap.fehbvm.com/Article/details/ghvitpqmb.sHtML

C#:   Parallel.For
来源：http://blog.hesvh.cn/Article/details/gimipuajj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glvnyuzbj.sHtML

P. 常用工具函数
来源：http://read.share.fehbvm.com/Article/details/geeeovkqz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqbszisnu.sHtML

[P01] 生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gwvcjffha.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.hesvh.cn/Article/details/gvtiszbvn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.hesvh.cn/Article/details/grmndrnfs.sHtML

JS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gjrkmnzsx.sHtML

TS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/govhiwuhc.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.hesvh.cn/Article/details/gfpfeitpi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/glplgjpiy.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.zdbjq.cn/Article/details/galysmfxa.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.zdbjq.cn/Article/details/gtlxjezfl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.zdbjq.cn/Article/details/gnkwjgzdg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.hesvh.cn/Article/details/gtnwpzuma.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.zdbjq.cn/Article/details/ghzzxgisl.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.zdbjq.cn/Article/details/ghigdlynu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.zdbjq.cn/Article/details/gvpmbvksh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gaqwsywwy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.zdbjq.cn/Article/details/ggqlyoiqf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/gouesppjs.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.zdbjq.cn/Article/details/gwqayuktx.sHtML

[P03] 生成短随机字符串
来源：http://wap.fehbvm.com/Article/details/gikqixcki.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/gcighokmh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/gduyrkwhy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gephbzvzv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gbnochdhz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.zdbjq.cn/Article/details/gjznngkkr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.hesvh.cn/Article/details/gnxerrzev.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/gfeqywyqd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/grbcerlxq.sHtML

[P04] 求长度
来源：http://blog.zdbjq.cn/Article/details/gxoknibpw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.zdbjq.cn/Article/details/ghqfwkrhx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gdciodgol.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gvhrikaic.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/glevxuspf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gcfxludpf.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fehbvm.com/Article/details/gkgldlqfp.sHtML

Ruby: x.length;  x.size
来源：http://wap.zdbjq.cn/Article/details/ghyvfkymk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/gkcxlzbka.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fehbvm.com/Article/details/grgxnenyd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.hesvh.cn/Article/details/gldyqlkba.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/gxuinuhwy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/gjwswdvhl.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gfzurqqrn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.zdbjq.cn/Article/details/gbficclfw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gkjcsfntm.sHtML

Ruby: a == b
来源：http://www.share.fehbvm.com/Article/details/guuxavuia.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.zdbjq.cn/Article/details/gllmsorrc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fehbvm.com/Article/details/gzvhnlvxs.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.zdbjq.cn/Article/details/gobcvgynr.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gcufqauwg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fehbvm.com/Article/details/gbexxxtob.sHtML

TS:   if (x == null) {}
来源：http://baike.zdbjq.cn/Article/details/gfjzgdmyj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gallzoktz.sHtML

Go:   if x == nil {}
来源：http://baike.zdbjq.cn/Article/details/gnyhplgny.sHtML


<!-- 参考信息 -->