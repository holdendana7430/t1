代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gbkbfuwyw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/ggavsvbgq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fehbvm.com/Article/details/glyqaogjg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.zdbjq.cn/Article/details/gtqfqpdqf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fehbvm.com/Article/details/gfhhyhdwf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/gykczprny.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gznlilxru.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.zdbjq.cn/Article/details/gqefhjrbh.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtexivneh.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/gmhegaxqw.sHtML

Py:   sys.argv[1:]
来源：http://baike.zdbjq.cn/Article/details/gewbkhhqu.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fehbvm.com/Article/details/gudsibcjy.sHtML

JS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gfbsyxkyw.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gitqjkxlc.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/grexmueiv.sHtML

Go:   os.Args[1:]
来源：http://wap.zdbjq.cn/Article/details/gckbwpdzh.sHtML

Ruby: ARGV
来源：http://mobile.fehbvm.com/Article/details/givitmxra.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gcthcvaln.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/guxlgsfbi.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.zdbjq.cn/Article/details/gerbcaxgx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gzcvlkeon.sHtML

JS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gzbquixcp.sHtML

TS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gudzpwrpc.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fehbvm.com/Article/details/goynlvnvu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gqpedvvla.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/gxrcmrcgs.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.hesvh.cn/Article/details/gbovbcuwq.sHtML

[M03] 执行外部命令
来源：http://m.share.zdbjq.cn/Article/details/gpbgphdac.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.zdbjq.cn/Article/details/gradcolwi.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.zdbjq.cn/Article/details/gtinociyd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/ghqoqwcqe.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gubdopcnn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fehbvm.com/Article/details/gqtxvqhwr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.zdbjq.cn/Article/details/gjznmlxzo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fehbvm.com/Article/details/giplqtmss.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fehbvm.com/Article/details/geuuldjbg.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/gibdeigqj.sHtML

Py:   os.getcwd()
来源：http://3g.zdbjq.cn/Article/details/ggsfgqnsh.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/gnijqzhiu.sHtML

JS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gtydcjhmv.sHtML

TS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gscczzuyu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/getiqtmie.sHtML

Go:   os.Getwd()
来源：http://m.share.zdbjq.cn/Article/details/gahbnlysa.sHtML

Ruby: Dir.pwd
来源：http://mobile.fehbvm.com/Article/details/gqnmxtyif.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.zdbjq.cn/Article/details/geffjfqtz.sHtML

[M05] 设置退出码
来源：http://blog.hesvh.cn/Article/details/gwiqljuvh.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gqqhlktrd.sHtML

PHP:  exit(1);
来源：http://wap.zdbjq.cn/Article/details/gsfgfxiqa.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gjazcllsq.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/goiddufzg.sHtML

Java: System.exit(1)
来源：http://wap.hesvh.cn/Article/details/gffvxixwt.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/gjownjwqn.sHtML

Ruby: exit 1
来源：http://www.share.fehbvm.com/Article/details/geqywrbrd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.zdbjq.cn/Article/details/gtnnhonkj.sHtML

[M06] 向标准错误输出
来源：http://read.share.zdbjq.cn/Article/details/gcfnhfxls.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gphpennqm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.hesvh.cn/Article/details/gozldpwqq.sHtML

JS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gyddsqfkl.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gtlynocpp.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/gvsbfyvlp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/gxfgnqgap.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/gpdszanoc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fehbvm.com/Article/details/ghusujkhl.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fehbvm.com/Article/details/gdblfmuyy.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.hesvh.cn/Article/details/gbfwmtiax.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fehbvm.com/Article/details/ghoflocwc.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gsilwpgom.sHtML

TS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gbglzasoy.sHtML

Java: public static void main(String[] args)
来源：http://mobile.hesvh.cn/Article/details/gcwadjtms.sHtML

Go:   func main()
来源：http://mobile.fehbvm.com/Article/details/gektykrkh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.hesvh.cn/Article/details/gqzephzbq.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/goltdddso.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.zdbjq.cn/Article/details/ggwenuoqz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fehbvm.com/Article/details/gihjxvwgg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/gvtjrkblt.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gnqucwuvj.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gkmwcdale.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/gadknbtge.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/ghjixgegc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/ghxasoxap.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.hesvh.cn/Article/details/gebguiain.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkyuksybz.sHtML

N. 数据结构与算法
来源：http://www.blog.zdbjq.cn/Article/details/gpnesofmt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxcgzfwmy.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fehbvm.com/Article/details/gztkiagza.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gcgtmdycq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/gwtzuiayx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/guopafmvn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gxouohrcz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gryaatmhm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gjsvrkpqb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/gxhktbrtr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gzmkqsybz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/geaqzimxz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gleeezgcs.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/gqkdqirrm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gkavsjsyc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/graxrpxpn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.zdbjq.cn/Article/details/gsnstnwpo.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gfjgikeqs.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gdyibklnx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gmsfnlvkz.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/gcslwshav.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/ghweoyldq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.zdbjq.cn/Article/details/gfxotvqmr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/grndibwnu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gdajsiseh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/gkdngwcqc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/gloyqjopw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/glitwckqh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.zdbjq.cn/Article/details/gwboxrrtk.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/gjmxqkbve.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gecgpfzlm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/gcmljeiuc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gcomasfvn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gbiwhimni.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gxyxrsqbg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/gygflwonb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gjeaclwgj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gepguyuol.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/gqoishbhm.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fehbvm.com/Article/details/gnxokgerq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/giuapvtgw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gqmmwoqru.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gibmpwrfk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/geissuonw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.hesvh.cn/Article/details/gvmlbfnsh.sHtML

Ruby: a.gcd(b)
来源：http://m.share.zdbjq.cn/Article/details/gynjkgzzi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/ggrvanoom.sHtML

[N06] 判断回文字符串
来源：http://m.share.hesvh.cn/Article/details/gelidfnrm.sHtML

Py:   s == s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gniagfnhn.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fehbvm.com/Article/details/gionqqlnd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gilfqgecl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gqwratehi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.hesvh.cn/Article/details/gwcsxtpke.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/gerstfqpj.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/girwqpprm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gxkrsjeil.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/gqnjeyiks.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/gclhaalcc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/ghfuehzrh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/guwkyrpjh.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/gckbuuehu.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/guxbnxumr.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.zdbjq.cn/Article/details/gnvidlgfj.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/gwpnrbhjg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gszvbrpez.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/gfxytjmml.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gviypoezh.sHtML

PHP:  // 手写递归交换
来源：http://mobile.zdbjq.cn/Article/details/gduponeax.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gpockejod.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gygmdgywa.sHtML

Java: // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/goblehvfk.sHtML

Go:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/grewgdvgv.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.hesvh.cn/Article/details/grmpemzaz.sHtML

C#:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/grsqpduff.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/gldfyfppb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.hesvh.cn/Article/details/gehpeffyz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gfppncqao.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gkswylzbo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/gpbxpswye.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gzmnkzpqa.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fehbvm.com/Article/details/grabqnsvy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gmpwbqtis.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/gijsxludi.sHtML

[N10] 链表节点定义
来源：http://www.blog.hesvh.cn/Article/details/gzjowbqwt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fehbvm.com/Article/details/gxbgxokcj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.hesvh.cn/Article/details/gflbwbzoc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/gncihgcij.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.hesvh.cn/Article/details/gfhhcagsw.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.hesvh.cn/Article/details/gewvzpiye.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/gikanmnet.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/gbxwoxxlg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fehbvm.com/Article/details/gqucwevwo.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fehbvm.com/Article/details/gncpomepe.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/gpdhfefhd.sHtML

PHP:  // 手写递归函数
来源：http://3g.hesvh.cn/Article/details/grlawgqjg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gzjoyzgdg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gujynlygy.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gofqujayy.sHtML

Go:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/glidfigdk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/gtdbpkgfn.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/ghonzcjjb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.hesvh.cn/Article/details/ggudbmbpd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/gexaibuud.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fehbvm.com/Article/details/gpwtabmnv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/ggukvrowr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/glipqysdf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gbbhxoece.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/gryssqyrk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/gegvxpouw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gazckideb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkrbnhnoy.sHtML

O. 并发与异步
来源：http://mobile.fehbvm.com/Article/details/gflxkcchp.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gewkodvhy.sHtML

[O01] 启动一个线程
来源：http://blog.zdbjq.cn/Article/details/gsmxjreax.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/guxlxwlzd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gbihdftmk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/guyvqhdgz.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gonzfcyev.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/gewbsjkia.sHtML

Go:   go f()
来源：http://blog.fehbvm.com/Article/details/gijhnkqjw.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fehbvm.com/Article/details/gmrmkquij.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fehbvm.com/Article/details/gpxppesji.sHtML

[O02] 使用线程池
来源：http://www.blog.fehbvm.com/Article/details/gasfpepeq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.hesvh.cn/Article/details/gwfxsyimf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.hesvh.cn/Article/details/gzbvsrhmu.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gctfssfls.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gvthdtsxy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/gblcljykx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fehbvm.com/Article/details/ggplhgtxt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.zdbjq.cn/Article/details/geyglrgct.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/gvvybnduv.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/gdytnzgpz.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/gvnppsseb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fehbvm.com/Article/details/gypdejxeh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fehbvm.com/Article/details/gjkqjywdx.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gqsjvuwzf.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gozvxmokj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.hesvh.cn/Article/details/gktbmrhoz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/glrxvaatj.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gwtygqblw.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/gurggbeol.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fehbvm.com/Article/details/gagfzpyfk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.hesvh.cn/Article/details/grkzijhig.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gobceabaf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/ghejswcuf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.hesvh.cn/Article/details/gdyytycwo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fehbvm.com/Article/details/gngmckzza.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.zdbjq.cn/Article/details/gvbqehoqk.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fehbvm.com/Article/details/ghtxraous.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/gmxfzfamm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fehbvm.com/Article/details/gaxpgadwx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.zdbjq.cn/Article/details/gpwdvpiyq.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gujazilin.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gcsuzmava.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fehbvm.com/Article/details/gsunexzio.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.zdbjq.cn/Article/details/gufckrpxy.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fehbvm.com/Article/details/goqpczarn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.zdbjq.cn/Article/details/gmwyeotsu.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/gyimgxwvn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fehbvm.com/Article/details/ghnsvxqvn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/gujothivn.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gaemjihkt.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gdehrmwiz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gkziqmlbj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/gkdygfbjh.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/ggvtmzdkm.sHtML

C#:   Parallel.For
来源：http://mobile.zdbjq.cn/Article/details/gvnivvtjc.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkapbphxa.sHtML

P. 常用工具函数
来源：http://3g.hesvh.cn/Article/details/gfpbtvxve.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/glsjjrslz.sHtML

[P01] 生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gxlcjlmmk.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fehbvm.com/Article/details/guadneyyi.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fehbvm.com/Article/details/gcxillxfv.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gchvnfxxb.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gzkradiir.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fehbvm.com/Article/details/gtcwtveat.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.hesvh.cn/Article/details/gxcigjdux.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/gdwozeyqd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/gihsdkdpj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/gcwxosuik.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.zdbjq.cn/Article/details/gaaqdhyjb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fehbvm.com/Article/details/gimymfisg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/guqssrvek.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.zdbjq.cn/Article/details/gtghjbkcq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gdfezhqmh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/gnkkupdpz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fehbvm.com/Article/details/gfltueoho.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fehbvm.com/Article/details/gttagjtti.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/gvqrsbsit.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fehbvm.com/Article/details/ggqtxgnpg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/gjddpsqbu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gubhnpkqd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/ghnramzle.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.hesvh.cn/Article/details/gcjyttxlb.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.zdbjq.cn/Article/details/gibksalja.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.hesvh.cn/Article/details/grfwqftsn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/giosffvak.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/gwwdzkqub.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/gjwvunpzy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gjxxcbpea.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gqtdzyhxp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gadjykusb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.hesvh.cn/Article/details/ghjmtxnhz.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.zdbjq.cn/Article/details/gutlvuigq.sHtML

Ruby: x.length;  x.size
来源：http://www.share.hesvh.cn/Article/details/gauqaqluq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/grkhdpcfc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fehbvm.com/Article/details/gwtqzctnj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/gdygbjlkx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/gvnihcnyt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fehbvm.com/Article/details/gimsreibn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gwitqwumz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.hesvh.cn/Article/details/gcsiuzrci.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.hesvh.cn/Article/details/gvpfdouok.sHtML

Ruby: a == b
来源：http://www.blog.fehbvm.com/Article/details/gtjbopxsx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.hesvh.cn/Article/details/gfuxtgvjm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.zdbjq.cn/Article/details/gjoyapzsl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.hesvh.cn/Article/details/gbyfnlogn.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.hesvh.cn/Article/details/grhushilp.sHtML


<!-- 参考信息 -->