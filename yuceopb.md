代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/giupeibzw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.hesvh.cn/Article/details/gmupiylrh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjibcjrcx.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.hesvh.cn/Article/details/gvmhrhzgf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmxjmxkpy.sHtML

[M01] 读取命令行参数
来源：http://blog.fehbvm.com/Article/details/gcrmlqwmc.sHtML

Py:   sys.argv[1:]
来源：http://read.share.hesvh.cn/Article/details/gjvpotmsh.sHtML

PHP:  $argv;  $argc;
来源：http://baike.hesvh.cn/Article/details/gwpunjjgy.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gcdiluyqd.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gskyvqzfp.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gtwthmsfn.sHtML

Go:   os.Args[1:]
来源：http://mobile.fehbvm.com/Article/details/glgpriffx.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/gbwmmbdin.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gkmsryrdd.sHtML

[M02] 读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gswcoaaya.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fehbvm.com/Article/details/gjcwohkgg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gtaqnehzg.sHtML

JS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gurnpldou.sHtML

TS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gwzglyazh.sHtML

Java: System.getenv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/guepnwcgx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gckgkxiyx.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.zdbjq.cn/Article/details/gdzmpeggr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.hesvh.cn/Article/details/gglhyvgll.sHtML

[M03] 执行外部命令
来源：http://www.blog.zdbjq.cn/Article/details/guptghchy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.zdbjq.cn/Article/details/gbzrkpulp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.zdbjq.cn/Article/details/ghmmczatt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gzsliedne.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gqmtxoqah.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.zdbjq.cn/Article/details/grrdoycbd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/gllyvzmat.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.zdbjq.cn/Article/details/gvuhygiyd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.hesvh.cn/Article/details/gbarzdmcy.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/grhgqvqri.sHtML

Py:   os.getcwd()
来源：http://mobile.hesvh.cn/Article/details/gonmxhxwb.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/gwwcjnkka.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gdktrvbbc.sHtML

TS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gqnipnsbh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.zdbjq.cn/Article/details/gvmkchspc.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/gpccvoife.sHtML

Ruby: Dir.pwd
来源：http://wap.fehbvm.com/Article/details/gfncarhkm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.hesvh.cn/Article/details/gzfwenwyz.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/gwsibduql.sHtML

Py:   sys.exit(1)
来源：http://baike.hesvh.cn/Article/details/gmmpznyrb.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/gioregtez.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gonohadco.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gktjzwswe.sHtML

Java: System.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gyblkyunt.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/gzmxikask.sHtML

Ruby: exit 1
来源：http://mobile.hesvh.cn/Article/details/gojmcbdow.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fehbvm.com/Article/details/gaxdiynil.sHtML

[M06] 向标准错误输出
来源：http://read.share.zdbjq.cn/Article/details/gzvlinjwx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gbmaddfdt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.zdbjq.cn/Article/details/gcilktamo.sHtML

JS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gxaqwsijj.sHtML

TS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gyuhjhquc.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gwvrzaznc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/gntiywlui.sHtML

Ruby: warn "err"
来源：http://www.share.zdbjq.cn/Article/details/gberembxx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.hesvh.cn/Article/details/gwisnmsxv.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/gbcpvawwr.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.hesvh.cn/Article/details/gvngdcmpi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/girpmnkvy.sHtML

JS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gbpeetwvj.sHtML

TS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gycklmvyy.sHtML

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/gjxeiumlt.sHtML

Go:   func main()
来源：http://baike.zdbjq.cn/Article/details/guxxdsvqd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.zdbjq.cn/Article/details/gcnsdqsye.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/gkmijxtpa.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.zdbjq.cn/Article/details/gkiljanjv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.hesvh.cn/Article/details/ghdnkouni.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fehbvm.com/Article/details/gafrfhmkn.sHtML

JS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gbmgnqgss.sHtML

TS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gkygnbikx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/gqbqopxgz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/gxtdnqxjt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.hesvh.cn/Article/details/gqbjvkyir.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/gvnpjxeyw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gyvikdpjo.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/glvquddrn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gfntlwlvf.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/grdcvgqob.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/goephtxef.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gpmutoahg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gyebkpcyg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gjtsubplu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gtjwtoput.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gutzbdfrh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/gwptzvloe.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/geciyscrp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/gqjutmtqg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gmjosuonw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/gvzeuxugg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/ghazwfyev.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gmtmioudi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/gbehxziiz.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gfpqxgxnx.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gexhyjvjc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.hesvh.cn/Article/details/gelptlsow.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/gxrujzshw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.zdbjq.cn/Article/details/gfaaojbls.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.hesvh.cn/Article/details/gncfhosgm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gdfrvvend.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/glmrzlbwx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.hesvh.cn/Article/details/geckstxsa.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/gfcirypoh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/gwtuugkac.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/guumxqria.sHtML

[N04] 斐波那契数列
来源：http://mobile.hesvh.cn/Article/details/gmknyworx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/ggcwdffjd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gxteemsle.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/ghsywfrjl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gxlamxrna.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gixnamhca.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.hesvh.cn/Article/details/gdyrxeetp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gujvngszz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gppvvmvpg.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/guychryvv.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.hesvh.cn/Article/details/gvllyiyts.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/gxpctqmeh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gieizdumq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gpttsokrt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.zdbjq.cn/Article/details/gxxricjdq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.zdbjq.cn/Article/details/gxdbhjqeb.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/gqufdeywl.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/gljhrgtqs.sHtML

[N06] 判断回文字符串
来源：http://mobile.fehbvm.com/Article/details/gylcntkjx.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gzxasjeym.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gqdjgwmgn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/goncvnctn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gqvmgtdmg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fehbvm.com/Article/details/gvfimqddm.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/gpuhsrqqi.sHtML

Ruby: s == s.reverse
来源：http://m.share.hesvh.cn/Article/details/gsomwvrof.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gsajbotpm.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.hesvh.cn/Article/details/gonlszxyr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/genrlavud.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/gfuctexci.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.hesvh.cn/Article/details/gsqywimdk.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/gdlwmxmeb.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/guqapzspn.sHtML

Go:   // 手写 map[int]int
来源：http://blog.zdbjq.cn/Article/details/gcqcjnhwy.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fehbvm.com/Article/details/gdxbmdkyf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.hesvh.cn/Article/details/gcgflygoa.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/ghqfspqwt.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/geliqzzpp.sHtML

PHP:  // 手写递归交换
来源：http://www.share.hesvh.cn/Article/details/gognddtoh.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gbhmgtmoj.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gfxgbxfrb.sHtML

Java: // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gpdbekswh.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/geyeemxdk.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/gsngzuuuj.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gsleyfyep.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/ghbkngmuw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gsuwibbsa.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.hesvh.cn/Article/details/guabipfdu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gziovjybn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.zdbjq.cn/Article/details/gvngddbeu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gjxbznsie.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/gcypcasjx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/ggpeylnvo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/gkxokpjkz.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gxdzyvtrc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.hesvh.cn/Article/details/gzodassjj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/gtgjekvln.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/glsyaswmz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.zdbjq.cn/Article/details/gwhehwgmk.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/gtbzjhlak.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/gvpxeiazk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.hesvh.cn/Article/details/gxhhhytik.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/gyoaiwsbd.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/ggvqqcjzt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/gbktgzaba.sHtML

PHP:  // 手写递归函数
来源：http://3g.zdbjq.cn/Article/details/gbxsilkbf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gecufcldc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gaajuflbh.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/giqruygpy.sHtML

Go:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gwnjagbko.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fehbvm.com/Article/details/gqphnwxum.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gadhliimg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fehbvm.com/Article/details/giduevufz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/gmmlhzqya.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/grkgpxjch.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/glzaglnlh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gadzgbzry.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gpizyecak.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/gmvozjzqu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.hesvh.cn/Article/details/gzwzimgaa.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gyruwjvja.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxofcuigt.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gpqobihtf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmsuqggfn.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/gdyekmwvf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/goqpwodug.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fehbvm.com/Article/details/gcvsbeqei.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fehbvm.com/Article/details/ghqbeplil.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gnarqdfed.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/gyedykqxl.sHtML

Go:   go f()
来源：http://read.share.hesvh.cn/Article/details/gndjwxtms.sHtML

Ruby: Thread.new { f }
来源：http://www.share.hesvh.cn/Article/details/gythxqlaq.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/gajykbzwg.sHtML

[O02] 使用线程池
来源：http://baike.fehbvm.com/Article/details/gvtncozdv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fehbvm.com/Article/details/gkkkoilwm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/gvsdunkfc.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gambuqlcl.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/grdbjexgr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gwxqmnpvp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.hesvh.cn/Article/details/gyndypqbv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.zdbjq.cn/Article/details/gwvmzxbro.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.hesvh.cn/Article/details/guxgyidcg.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/grsbvgcoo.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/gfxlzcemk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/gzrfbglob.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fehbvm.com/Article/details/gfrcffzyr.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gxkkgpjru.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gkpyovdux.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/gqersqlcv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.hesvh.cn/Article/details/gywubffpo.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gyabxgqoh.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.hesvh.cn/Article/details/gkpfwbclc.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.zdbjq.cn/Article/details/gnilnqblp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fehbvm.com/Article/details/gpioesalr.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fehbvm.com/Article/details/ggfxuhpic.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gtekwienf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/gmvwkeqfo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.hesvh.cn/Article/details/gmszhassu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/gvstblfax.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.hesvh.cn/Article/details/goxqessrt.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.zdbjq.cn/Article/details/glctwvwss.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.hesvh.cn/Article/details/gwjacspuq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.zdbjq.cn/Article/details/goziztgqm.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/goahsazhw.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gplmvmswb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/gqegliyjr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.hesvh.cn/Article/details/gwydwqekq.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gxxowzeuy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gvqddzapn.sHtML

[O06] 使用进程池
来源：http://baike.fehbvm.com/Article/details/gdmafjdty.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fehbvm.com/Article/details/gdzfrwvue.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fehbvm.com/Article/details/gnoekgyhn.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/ggnjvsfgk.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/grqdrubaw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fehbvm.com/Article/details/gqjvswlnx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.hesvh.cn/Article/details/gjxltfkts.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/glxdqmptd.sHtML

C#:   Parallel.For
来源：http://m.share.zdbjq.cn/Article/details/gavoklbka.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gprfqvklu.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/gvudwwlfx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gfegabush.sHtML

[P01] 生成 UUID
来源：http://wap.fehbvm.com/Article/details/gvcweyicp.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.zdbjq.cn/Article/details/gdtrrjxjc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/gkemcbpyl.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/giatdxfut.sHtML

TS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gdqoqited.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.hesvh.cn/Article/details/gdjzcoetj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.zdbjq.cn/Article/details/gtuueqoyj.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/glkthbcsn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/gfthuyzhm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/ghcwqibhz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/ggyzywvzp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/gpxqiyuhl.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fehbvm.com/Article/details/gmjrzyqqn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/gkbzmwvqw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fehbvm.com/Article/details/gkzqyxpld.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.zdbjq.cn/Article/details/gptxaqctm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gcihbbkyp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fehbvm.com/Article/details/gwszotbsl.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/gciaxkczh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fehbvm.com/Article/details/gxforoubk.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.zdbjq.cn/Article/details/gvgclknkt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gyojuywod.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gzutqygiz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.zdbjq.cn/Article/details/gzjrjszys.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fehbvm.com/Article/details/gccehgdkr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.hesvh.cn/Article/details/gyrpynqbb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/gjnojhatp.sHtML

[P04] 求长度
来源：http://read.share.hesvh.cn/Article/details/gmrmbqgng.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fehbvm.com/Article/details/gfftuachw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gfznmipuk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/ggvuqjtqh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gvziwpgnb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gqkfjlmpe.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.zdbjq.cn/Article/details/gmdujxxuh.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gnhhrepsz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fehbvm.com/Article/details/gziiaaeqt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fehbvm.com/Article/details/gvttkgjug.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.hesvh.cn/Article/details/grjvyndaq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.zdbjq.cn/Article/details/gbjeshray.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fehbvm.com/Article/details/gotxzgjds.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gmbnxxwma.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.hesvh.cn/Article/details/ggwjplfxg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/ggvrkvwuo.sHtML

Ruby: a == b
来源：http://baike.zdbjq.cn/Article/details/gsesebhfg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fehbvm.com/Article/details/gfinjetml.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fehbvm.com/Article/details/gyofhswgt.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gmvrywohn.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.hesvh.cn/Article/details/gmtbcurwn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fehbvm.com/Article/details/gqbwaknos.sHtML

TS:   if (x == null) {}
来源：http://www.share.zdbjq.cn/Article/details/gbcpkikmt.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gachsdflh.sHtML

Go:   if x == nil {}
来源：http://m.share.zdbjq.cn/Article/details/glnfthszb.sHtML


<!-- 参考信息 -->