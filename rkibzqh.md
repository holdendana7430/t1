代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fehbvm.com/Article/details/gjswlblhu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/gjkouwenh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/glsjpfgxv.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.hesvh.cn/Article/details/gakusjqla.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfgxganhw.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gccajobht.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fehbvm.com/Article/details/gofwvbqyp.sHtML

PHP:  $argv;  $argc;
来源：http://wap.zdbjq.cn/Article/details/ghchnoanc.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gztyrtorx.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gycehywjk.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gwlcoozfj.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.hesvh.cn/Article/details/geznomzay.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/gdlvmzpbe.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gacqebybc.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/gkjmuekmo.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fehbvm.com/Article/details/gppopfpjp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gubeolktg.sHtML

JS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gwyvsyveb.sHtML

TS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gfuyffqdb.sHtML

Java: System.getenv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gvcgatnin.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.hesvh.cn/Article/details/gyznczvaf.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.zdbjq.cn/Article/details/gerjnweax.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gqhwolrrx.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/gdwdraaqw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.zdbjq.cn/Article/details/gtfmgecct.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.hesvh.cn/Article/details/ghicerrzs.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gpgsqltbu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gvjaeedcz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.hesvh.cn/Article/details/gtwzlqxvh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.hesvh.cn/Article/details/getsixhly.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fehbvm.com/Article/details/gpaeflfcm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/gecvikhrx.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/ghyocvqll.sHtML

Py:   os.getcwd()
来源：http://mobile.zdbjq.cn/Article/details/gqfhgiqgk.sHtML

PHP:  getcwd();
来源：http://m.share.fehbvm.com/Article/details/gbreztukz.sHtML

JS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gonkygqst.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gcspjrric.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.hesvh.cn/Article/details/gkpmufijr.sHtML

Go:   os.Getwd()
来源：http://read.share.hesvh.cn/Article/details/gcrwspwwr.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.zdbjq.cn/Article/details/gywoujqyw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/gdaiszfsb.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/guhlliajk.sHtML

Py:   sys.exit(1)
来源：http://blog.fehbvm.com/Article/details/gbxuswais.sHtML

PHP:  exit(1);
来源：http://baike.zdbjq.cn/Article/details/gvnydfoky.sHtML

JS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gdmdhpafw.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gjmipljso.sHtML

Java: System.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gkctcmmjg.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/gabjigkll.sHtML

Ruby: exit 1
来源：http://baike.hesvh.cn/Article/details/gzwhtyooc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/gfhycxrki.sHtML

[M06] 向标准错误输出
来源：http://3g.fehbvm.com/Article/details/gukotztwr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gclajsvcs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/gvfdtytbw.sHtML

JS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gpefdymnc.sHtML

TS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gmcwnwqde.sHtML

Java: System.err.println("err")
来源：http://blog.zdbjq.cn/Article/details/gjhcrizje.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fehbvm.com/Article/details/ghourztag.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/ginpczffs.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/gdoxcduxg.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/gyztxdgun.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.zdbjq.cn/Article/details/gjvzjmugh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/gzhevubhx.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gvhosmjdq.sHtML

TS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gfplyjydz.sHtML

Java: public static void main(String[] args)
来源：http://read.share.hesvh.cn/Article/details/gfhqcaali.sHtML

Go:   func main()
来源：http://wap.zdbjq.cn/Article/details/gbjsrntak.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/ggldibukc.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/gziwvyjjj.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gnbcalbwt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/gcprpwfvi.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.hesvh.cn/Article/details/gyxuvtgrk.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gpfhcpeot.sHtML

TS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gctukysgp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fehbvm.com/Article/details/gwabuflxu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/gevsupabx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/gtrsjorzx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.hesvh.cn/Article/details/gmkltenki.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gshuhuzfr.sHtML

N. 数据结构与算法
来源：http://read.share.zdbjq.cn/Article/details/gyyhapxap.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpoxpsyay.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fehbvm.com/Article/details/gpiwbgguo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.zdbjq.cn/Article/details/glqomstoi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/gbqfjqnof.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gyeqslqml.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gbacowoag.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gxhsfmrzr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gobdajtqj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.zdbjq.cn/Article/details/gucqlzyor.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gjhfhevrb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fehbvm.com/Article/details/giazzylee.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gtleouvdu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fehbvm.com/Article/details/gfvcdmvpd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gihkctkrl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gyjndkzgr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/gvkpelvcs.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gztlbouys.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gfhlkhnwj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fehbvm.com/Article/details/gdyyxdlaj.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.hesvh.cn/Article/details/gmiheuelr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fehbvm.com/Article/details/gukxaedab.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fehbvm.com/Article/details/gtylumuon.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gzkhcsrbw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gcgjhzkki.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.hesvh.cn/Article/details/gcusipmma.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.hesvh.cn/Article/details/glrdzwrax.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.zdbjq.cn/Article/details/ggcekeisp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.hesvh.cn/Article/details/gdfnagzxp.sHtML

[N04] 斐波那契数列
来源：http://wap.zdbjq.cn/Article/details/gqdslzftt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gkedzojrb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fehbvm.com/Article/details/gunxrdmpj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/guyssrlnb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gdpqtfyge.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gjdhuhjdu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/glbddjmef.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gdwrwiekz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gnolqwvaf.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/gxzemardm.sHtML

Py:   math.gcd(a, b)
来源：http://3g.zdbjq.cn/Article/details/ggpsdmcrh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.hesvh.cn/Article/details/gxdeixiij.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gtmsduzdj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gymzantdv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.zdbjq.cn/Article/details/gcafmnijm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/gqsinnudb.sHtML

Ruby: a.gcd(b)
来源：http://baike.zdbjq.cn/Article/details/gtylvjqpi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/gmwlluugm.sHtML

[N06] 判断回文字符串
来源：http://read.share.hesvh.cn/Article/details/gxmfnxbks.sHtML

Py:   s == s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gvaaurqht.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gxwpkvems.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gzfmugdgk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gxvscsoun.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.fehbvm.com/Article/details/gqvfeklfm.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/gptdgxmpk.sHtML

Ruby: s == s.reverse
来源：http://read.share.fehbvm.com/Article/details/gkmefyaqs.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gcezcjmef.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fehbvm.com/Article/details/gihpxeaty.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.zdbjq.cn/Article/details/gwsflwukq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/gjndpyocl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/gggyhmgzx.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.hesvh.cn/Article/details/gxmhvbmfw.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gsaqctdbe.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/grvzxjagl.sHtML

Ruby: // 手写 Hash
来源：http://www.share.zdbjq.cn/Article/details/gzwyamect.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/gpnhkplrd.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/gcyxlpbja.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gaquzfoox.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/ghdkygtzc.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/geismqbjg.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gnibfejgf.sHtML

Java: // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/goquellol.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gcdzcpqwq.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.hesvh.cn/Article/details/gmxwxfarl.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/grclqsqny.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gcgbqwrcf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/glpkxxvlc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gphwyetsa.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gswvmnrpk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/grwmnykuc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gqkfiwyot.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fehbvm.com/Article/details/gvzqarojc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/girnkuzag.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fehbvm.com/Article/details/ghvphfsjq.sHtML

[N10] 链表节点定义
来源：http://blog.hesvh.cn/Article/details/girauagec.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/gsvglfyuq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.zdbjq.cn/Article/details/gobbkbqcf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.hesvh.cn/Article/details/gpdamhsjz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/gxcpqhykv.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/gmkfjbxym.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.hesvh.cn/Article/details/guvroimxw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.zdbjq.cn/Article/details/gtesqqqqz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/geotkphff.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/gibtcmsle.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.hesvh.cn/Article/details/goficirqu.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/ggkzjhocm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gtjipdtyj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gfyzmebyv.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gbyccnvwy.sHtML

Go:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gfbbdssox.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/gquuishpu.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gnkelgxoj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.hesvh.cn/Article/details/gzmcyqudy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/gtmovgwcw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/grmrhkzem.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gmirvmrcm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gomlrqsej.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/glbifcgvf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.hesvh.cn/Article/details/gghtqqxei.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fehbvm.com/Article/details/glrlipdlf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gilpnefiv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gffoiffiz.sHtML

O. 并发与异步
来源：http://blog.zdbjq.cn/Article/details/gmkcdicbj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gterzgccw.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/gvgioezey.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fehbvm.com/Article/details/gaythzlbk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/gdoycoutc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gkrjsogwl.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gxybrsljv.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/gkseieiea.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/ghfjnxjcg.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fehbvm.com/Article/details/gstejnxwm.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/gjtocimzj.sHtML

[O02] 使用线程池
来源：http://baike.zdbjq.cn/Article/details/gpbswswsx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fehbvm.com/Article/details/gdpfeqvbl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.hesvh.cn/Article/details/gotaxvvas.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/geozucvth.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/giihjryvi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.zdbjq.cn/Article/details/gewixglhy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.hesvh.cn/Article/details/guknlqwch.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fehbvm.com/Article/details/gcxeguebt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.hesvh.cn/Article/details/gglxhgeel.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.hesvh.cn/Article/details/gjkufovnt.sHtML

Py:   with lock: shared += 1
来源：http://3g.fehbvm.com/Article/details/gpekdxoip.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/gauphemyg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/gfdftcbjv.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gfkllzivz.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gqaefmqpv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.zdbjq.cn/Article/details/gyolwwuzm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/golqetxsz.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gkpfqmptx.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gjaxdstjd.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fehbvm.com/Article/details/gikiabzzi.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/gutuysllm.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gnzirrrqs.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/gslvsqvvk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.zdbjq.cn/Article/details/gzvncuzww.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/gxagahkbc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.zdbjq.cn/Article/details/ggwnctvmp.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.zdbjq.cn/Article/details/gitdphdrf.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.fehbvm.com/Article/details/gurqshgor.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fehbvm.com/Article/details/guryqzjrh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.hesvh.cn/Article/details/gdefrohkn.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/goeclosdp.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/ghesnnrcu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fehbvm.com/Article/details/gvniucqqg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.zdbjq.cn/Article/details/gacogbuki.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/gnpqgkwqc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/grbqguzwy.sHtML

[O06] 使用进程池
来源：http://read.share.fehbvm.com/Article/details/gequdtawy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fehbvm.com/Article/details/ghbjqzwiq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/grwzkuohz.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gpncbrphf.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/glrzmlcqw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fehbvm.com/Article/details/gmeagkjzg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/gcjfiiiet.sHtML

Ruby: // fork 块
来源：http://3g.fehbvm.com/Article/details/gurzhadjq.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/ggxvjzjob.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gcmjiytar.sHtML

P. 常用工具函数
来源：http://mobile.hesvh.cn/Article/details/gfrvdtoef.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdtahianr.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/gmatqivrw.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fehbvm.com/Article/details/gdtttndfe.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.hesvh.cn/Article/details/gdkmpiedx.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gsbllhtzv.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gltesbwed.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fehbvm.com/Article/details/gmvojkvoj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fehbvm.com/Article/details/gqmximtku.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.zdbjq.cn/Article/details/gfahqjqpu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.hesvh.cn/Article/details/gyrbzbhrl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/gecgrakjl.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.zdbjq.cn/Article/details/gejenihmt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/gpxsygtwr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gobhqzryq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/ghzfvcshz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gcgwwgjdy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/gxhbpsnju.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.zdbjq.cn/Article/details/gclpgiibg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.zdbjq.cn/Article/details/gtzqulkvm.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gjnjocgbu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fehbvm.com/Article/details/gndfkhdlp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/grgwtqbsg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gjolscujv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gfzxdfcnm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fehbvm.com/Article/details/gciopwawc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fehbvm.com/Article/details/gwszikvhf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fehbvm.com/Article/details/grndnnxym.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.hesvh.cn/Article/details/gpmyleitt.sHtML

[P04] 求长度
来源：http://www.blog.zdbjq.cn/Article/details/gkyekinmw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.hesvh.cn/Article/details/gsrcigrmh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gsyazamxy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/grrbydhto.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gzwjdptyq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gljsvhzhv.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/gkibyuqvd.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.hesvh.cn/Article/details/gxqtkleyy.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gnecqoypt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/gpjueakmz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fehbvm.com/Article/details/gduxkuubb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.zdbjq.cn/Article/details/gmunvecaw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.hesvh.cn/Article/details/gqxecipkj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gfpsonmxu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/grdmrtkrt.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/gigvosctk.sHtML

Ruby: a == b
来源：http://www.blog.hesvh.cn/Article/details/gafrzfyvz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fehbvm.com/Article/details/geozvveod.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.zdbjq.cn/Article/details/ghkjbgbph.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/gkldveprx.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gtgwmlyqf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fehbvm.com/Article/details/gftglrgzb.sHtML

TS:   if (x == null) {}
来源：http://blog.hesvh.cn/Article/details/gkbkaqpzg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gkbfzoqlc.sHtML

Go:   if x == nil {}
来源：http://www.blog.zdbjq.cn/Article/details/gqmgpswfh.sHtML


<!-- 参考信息 -->