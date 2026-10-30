代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fehbvm.com/Article/details/gnfcsgcur.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.hesvh.cn/Article/details/gtqzocyjd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjwatlezg.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fehbvm.com/Article/details/gavdznwzw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggebhazgp.sHtML

[M01] 读取命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gjzohehrs.sHtML

Py:   sys.argv[1:]
来源：http://3g.fehbvm.com/Article/details/gxjdcezog.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.zdbjq.cn/Article/details/gtyeczrlf.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gzzrpnvmt.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gixupmtae.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gulzjyiww.sHtML

Go:   os.Args[1:]
来源：http://mobile.hesvh.cn/Article/details/gvoluakjp.sHtML

Ruby: ARGV
来源：http://baike.hesvh.cn/Article/details/guszhbgnx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gaggigpqj.sHtML

[M02] 读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gkucxjpho.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gvrnmfewq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fehbvm.com/Article/details/ginbyusid.sHtML

JS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gdaoivhdq.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gonaymzzc.sHtML

Java: System.getenv("HOME")
来源：http://3g.hesvh.cn/Article/details/gnlkueaym.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gpylznuuy.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fehbvm.com/Article/details/glyhupaix.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.zdbjq.cn/Article/details/gzdfotzuw.sHtML

[M03] 执行外部命令
来源：http://mobile.fehbvm.com/Article/details/gfnxdvawm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fehbvm.com/Article/details/goffturvn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/gtvnassos.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/guixvfbya.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gaimyytui.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.zdbjq.cn/Article/details/giplasyrw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/ggxgqbsge.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.hesvh.cn/Article/details/gfxwsmcvm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.zdbjq.cn/Article/details/gngynccaa.sHtML

[M04] 获取当前工作目录
来源：http://baike.fehbvm.com/Article/details/gwqjlqnci.sHtML

Py:   os.getcwd()
来源：http://www.blog.zdbjq.cn/Article/details/gvzdfwblt.sHtML

PHP:  getcwd();
来源：http://wap.zdbjq.cn/Article/details/gjkqecfrn.sHtML

JS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gcletznzb.sHtML

TS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gdvqherna.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.zdbjq.cn/Article/details/gyswzfizx.sHtML

Go:   os.Getwd()
来源：http://www.share.fehbvm.com/Article/details/gcpesoyga.sHtML

Ruby: Dir.pwd
来源：http://www.blog.zdbjq.cn/Article/details/glodncwhi.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fehbvm.com/Article/details/gqcigurkl.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/gzrqlnkck.sHtML

Py:   sys.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gggsftszs.sHtML

PHP:  exit(1);
来源：http://www.blog.hesvh.cn/Article/details/gegqtnhbn.sHtML

JS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gilmwvmfm.sHtML

TS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gnsxipzvs.sHtML

Java: System.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gbzlohood.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/gjbpsrhqj.sHtML

Ruby: exit 1
来源：http://www.share.fehbvm.com/Article/details/gjqkoludd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/gbqetdpjm.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/gkhhpjvgm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/goonncenx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fehbvm.com/Article/details/gerveebby.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/goievafzq.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gfnielolv.sHtML

Java: System.err.println("err")
来源：http://3g.fehbvm.com/Article/details/gdwxluccd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/gjibfrded.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/gjoersitg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.hesvh.cn/Article/details/ggjrmajbj.sHtML

[M07] 判断是否为主入口
来源：http://blog.fehbvm.com/Article/details/gnnphvvor.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fehbvm.com/Article/details/gpyszszjp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.zdbjq.cn/Article/details/gujmzsufe.sHtML

JS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gjxboeqgj.sHtML

TS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gqckwguao.sHtML

Java: public static void main(String[] args)
来源：http://www.share.zdbjq.cn/Article/details/glwwczxec.sHtML

Go:   func main()
来源：http://www.blog.zdbjq.cn/Article/details/gujgcwdob.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/gcfjmkuez.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.zdbjq.cn/Article/details/gyvvweohq.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gwvuxgocy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fehbvm.com/Article/details/grfdwgait.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/gdokeqxgc.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gusdwuthw.sHtML

TS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gedytrwmn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.hesvh.cn/Article/details/ggyvmlkvd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.hesvh.cn/Article/details/gcexwxedu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/gbuybeqbu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/grpkzexvh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gppxhryzj.sHtML

N. 数据结构与算法
来源：http://www.share.hesvh.cn/Article/details/gwdprdmjt.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfvjuybru.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/gntehrtvt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gycynnjtd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/griejufle.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gkzdaycts.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gtomxcnqq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gsdelfkst.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gtmoyrjjo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/gfdywybht.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gthimjlyb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fehbvm.com/Article/details/gtxsgyhnz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gxgujrsgm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/gyoeowpxu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gfcaslreq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gjqbtbicq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.zdbjq.cn/Article/details/gggkfoeck.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gdjxlipfh.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/ghreiazzr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.hesvh.cn/Article/details/gfrzbmiqo.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/goqkcjslb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/gqdwrppad.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gpsvidtpp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gqqgfkbch.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/guzijetrx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/gotgciaxs.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/guqtkghyy.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.zdbjq.cn/Article/details/gwtfohkbu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.hesvh.cn/Article/details/gaqpgvakl.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/gjcgkueqd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gejhtzllk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.hesvh.cn/Article/details/ghltntsxq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gncdmxgqr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gjeazjkyn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gjuavztpq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/gpcpmzvva.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gssfuhxoi.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gndhoiwdh.sHtML

[N05] 最大公约数
来源：http://3g.fehbvm.com/Article/details/glcrdkbjb.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.hesvh.cn/Article/details/grishhakj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/gtlzsxqwz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gdagjcuom.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gooeneurw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.zdbjq.cn/Article/details/gwqqxnfus.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/gtdbtxive.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/gbyljamht.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/gbxbayczv.sHtML

[N06] 判断回文字符串
来源：http://read.share.fehbvm.com/Article/details/gkxgetvxa.sHtML

Py:   s == s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gtafccpxl.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gaxkflney.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gdndoibyr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gfygptyqm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.fehbvm.com/Article/details/gydlaeccs.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/gabotoxar.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gvlwscmnz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gixgszony.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/gqhuyhobs.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fehbvm.com/Article/details/gylcdejmk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fehbvm.com/Article/details/ggwyjtrcs.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.zdbjq.cn/Article/details/gwbpepshz.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/gwwhwatqw.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/gfexpzvik.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.zdbjq.cn/Article/details/gxlymthgv.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/gqpfcdhvi.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.hesvh.cn/Article/details/gtcfsqvrb.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/galottjdb.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fehbvm.com/Article/details/grurohiic.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fehbvm.com/Article/details/gdukjlpln.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gtocovcge.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/grslmjtzv.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/goltmctas.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gvzcygohv.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.hesvh.cn/Article/details/gvxpyuymo.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/goajkqdyg.sHtML

[N09] 栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gsucnpalx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/gcxsfgaiu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gbupnwmpa.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gcmsostxg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.zdbjq.cn/Article/details/golpkpnyx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fehbvm.com/Article/details/gadmzlkwh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/gkwflgcpc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gibemigcv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fehbvm.com/Article/details/gkmfomlgl.sHtML

[N10] 链表节点定义
来源：http://www.share.fehbvm.com/Article/details/gqvtvawco.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.zdbjq.cn/Article/details/gdigoprbr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gtdorunjs.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.zdbjq.cn/Article/details/gdxaaqtug.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fehbvm.com/Article/details/gcszsifhq.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/gnycyvyae.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/gvuzxvnua.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/gxggseovw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/gubycqfnn.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/gfhevexmg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.hesvh.cn/Article/details/ggsovkyll.sHtML

PHP:  // 手写递归函数
来源：http://3g.hesvh.cn/Article/details/gmdfhyfqh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/guuoeeyzj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gsjvyfndq.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gxwzfmnpd.sHtML

Go:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gbbxtqzkw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.zdbjq.cn/Article/details/gjrodpxjd.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gxdnefpvc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/gftcmxuab.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fehbvm.com/Article/details/gnwbyyyer.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.hesvh.cn/Article/details/gwsbziprc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gkzyvbfin.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/goncyzuvk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gbwnyuwuh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/gaqweqanm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/gkkfcdzhg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/goagqplbo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkttvnasb.sHtML

O. 并发与异步
来源：http://www.share.fehbvm.com/Article/details/gzwbzqgwm.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gylfxfzxf.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/gygqxgouh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fehbvm.com/Article/details/gdudnpzyr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.hesvh.cn/Article/details/gberaqtph.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gagygfirj.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gaspdmzzn.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fehbvm.com/Article/details/gkbntgdae.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/gkqsvkbtx.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/gjsbdrirm.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.hesvh.cn/Article/details/grdrjrljt.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/glrmcxcbo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.hesvh.cn/Article/details/gokhhqebv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.hesvh.cn/Article/details/goikjziar.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gzclengol.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/glevcqreg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.zdbjq.cn/Article/details/gwbxzlgib.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.zdbjq.cn/Article/details/gdwrpfxny.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.fehbvm.com/Article/details/gvoyilxeb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.zdbjq.cn/Article/details/gdhjcfqnn.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/gopbpunxc.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/gtztcctva.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.hesvh.cn/Article/details/gfunruuxq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.hesvh.cn/Article/details/ghtfoarlv.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/giunuytgu.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gulonbbid.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/gmrseoxer.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fehbvm.com/Article/details/gvavcvihf.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gmlvwqqnm.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/gomepdymj.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.hesvh.cn/Article/details/gtqrmfesk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fehbvm.com/Article/details/gxurzjjtp.sHtML

JS:   async function f() { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gkckobsiq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fehbvm.com/Article/details/gapoiejru.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/gxyypxaen.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.hesvh.cn/Article/details/ghuawmybw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gixhvygzk.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.hesvh.cn/Article/details/gsdjaeqzd.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/guypajcxm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fehbvm.com/Article/details/goqgcaadj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.hesvh.cn/Article/details/gvrjbnslg.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gemwzaiqa.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gjlkmhldh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.zdbjq.cn/Article/details/ginjcblns.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.zdbjq.cn/Article/details/gwhpyggdx.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/gkckcfuco.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.hesvh.cn/Article/details/gmpihydkz.sHtML

[O06] 使用进程池
来源：http://blog.hesvh.cn/Article/details/geulrxzqa.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/ghxbsywcu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/gsutzfoxf.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gbllafviw.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/ggpzfqhij.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/gegvfykbc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fehbvm.com/Article/details/gmoyridrf.sHtML

Ruby: // fork 块
来源：http://3g.hesvh.cn/Article/details/gqxwnxdyv.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/gowmaappk.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtgoexexs.sHtML

P. 常用工具函数
来源：http://3g.hesvh.cn/Article/details/gwctsqffh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxmujwwpj.sHtML

[P01] 生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/ggrtwdffg.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.hesvh.cn/Article/details/gqylgtues.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/gexkmimqy.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gxkjkebch.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gfhohdvoc.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/gtlqdddqc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.zdbjq.cn/Article/details/gfuavlvfo.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.hesvh.cn/Article/details/gnqhxbfrb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/gmazfgxwy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.hesvh.cn/Article/details/gxnyjzvmn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.zdbjq.cn/Article/details/gbhflcssv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fehbvm.com/Article/details/gogmfcmfj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/gpjkzrwsq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.hesvh.cn/Article/details/gxgbbavsn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.zdbjq.cn/Article/details/gwvpfuphw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fehbvm.com/Article/details/gsvlszspl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.hesvh.cn/Article/details/gjmpwhzhy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.hesvh.cn/Article/details/gvrxsksqs.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/gkraptclb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.zdbjq.cn/Article/details/gogkpnfcj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/grfkbqsbp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/ggwxhmpzz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/guuzempoe.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fehbvm.com/Article/details/gemvhqand.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/gavcydgcg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.zdbjq.cn/Article/details/gvgjtcbrl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fehbvm.com/Article/details/gelrgqcox.sHtML

[P04] 求长度
来源：http://baike.hesvh.cn/Article/details/gnxdyylgi.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.zdbjq.cn/Article/details/gdkxeelpf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gsmeqvmwr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gqqxomxfw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gxynofrnw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gzovuaxkc.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/gakiqntxe.sHtML

Ruby: x.length;  x.size
来源：http://baike.hesvh.cn/Article/details/gysgaivlo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gedaxyiad.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/gvitnatlo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/glahxkrof.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/gpcmfrrtl.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/gfgawrpiz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gjfqqxlma.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.zdbjq.cn/Article/details/gunhlfjlm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.hesvh.cn/Article/details/gymrzmppf.sHtML

Ruby: a == b
来源：http://www.m.share.fehbvm.com/Article/details/grvwxhvyi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.hesvh.cn/Article/details/gnlxoisev.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/gquzunsrd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/grrghbora.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fehbvm.com/Article/details/gxicjjzsz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/ghnxdapty.sHtML

TS:   if (x == null) {}
来源：http://mobile.zdbjq.cn/Article/details/gwopekokm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gucykkzyc.sHtML

Go:   if x == nil {}
来源：http://blog.zdbjq.cn/Article/details/gxlkvqglf.sHtML


<!-- 参考信息 -->