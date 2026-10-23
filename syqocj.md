代发 wailian999

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3stjdsjeo.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3uxniigot.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3cwgbpggu.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3rcgmtnef.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3aytdakzw.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3qnukpklj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3hssnabeq.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3ychuykxi.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3kuembbxa.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3kfgavzfz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3klqpifcj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3ptqcjlrp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3akloduse.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qmydfkbt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ophbohhn.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3waudvipm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3plzvhpxk.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3vimjyhcn.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3nqidaboz.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3siiaauty.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3eeaijung.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rdyrkaht.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3jrwbowty.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3csuinirr.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3kuxpfggq.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ybzstsao.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3akdwjsfe.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ayexcgjy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3bbvycdac.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3bfujljgk.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3vsppwjfe.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3nkkrcfsu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3nekpsmte.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3hmbyimoe.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3bmkhovhd.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3rytlqjsw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3kvisdtef.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3xjzwlmfp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3skyiunit.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3gdiukmvy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3fgmuxnlz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3zdbogqiy.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3rkseihos.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3txfqpqsf.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3fksjvedh.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3fzkkmkpt.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3byqgnydz.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3mihpgbdb.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3xndwflnu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3noyqofgp.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ctihxjqb.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3xkjsitci.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3bozlyfti.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3zlfazukp.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lacifjly.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3uqqrocbj.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bsfokrgv.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vsoptzxe.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tqswhlck.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zpksiecy.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3criqtzmz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3nuvkttlb.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3mbwxuqtb.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3izyymfvf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3sjpxachw.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3vgwrrivq.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3qurdqhzq.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3rxrnumwv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3bqlhuebg.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3xvoviuzv.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zmswmcea.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3yhbthlvt.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3sdunjfjs.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3mqqascnc.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ulvopiez.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3naqszhky.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3sxaxeeyy.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3orptgpje.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3hkcjezls.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3rmjphxsz.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3xmkpepyy.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3dofugkpp.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3ibusgdmm.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3gjpaltbd.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3cgnnvprg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3gnprxhyf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3zclukthx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3heidlbit.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3sqdrshnf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fzxcvgmd.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3cvnhzgho.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eutqtbgh.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3wkfrdvvn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3uahkkjsi.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3oyejyeys.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ohoycgna.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3vrkdpugj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3yjxuwywf.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ibpqzrdq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3ygpvozye.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3emvobdvs.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3gflgbdyk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3oijeciqz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3syjzefzm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3afcwlpsj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3jpquksnz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3byayhlct.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ntsrsfed.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3xvhmtdjl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3lwoelkge.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3niaozimz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3tmetbzsp.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3atlifmwq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3luvloeor.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3pfqelaet.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3xcqxrhiz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3avjxgvkh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3hvueltab.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3oiwsofrw.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3bqdfdhnu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3pahoyycd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3qgdtegvx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wwqcwqqj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3eezkmjga.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3kamwdjel.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3alhagmck.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nfeujjht.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yfjigkkg.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3gklmwzwx.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3yqcyrqlx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3uekxviwy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3cqewliec.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3sntfkagq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3ddkavmdf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3azrhbmcu.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3awcyzwla.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3stpitype.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3conoogab.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3fujsrgkn.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fmprpilo.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3uoafvrdh.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3gvdbphkv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3oujzizbo.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3fhwrcgln.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3zhedxgju.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3exgchdld.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3cscljlmm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3qehpkubk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3zfpsusra.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3ggmwjbom.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3pumlimod.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3hqwbqtlx.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3dcqsbudi.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3hjtkioti.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3moaemrvu.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3mmigbzox.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3ddkufyun.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3pgtpuwce.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rrazuhyq.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3alyreofu.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3kizwfqas.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3urjttgpb.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3lgbwwnpz.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3delmicwa.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3fahyhofr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3mmfhhdqo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ocunebaf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3qyurkbtz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3fyetzghx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3uwumnwxf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3whrrtgzu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3skuiukya.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3xinjmomh.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3hkgoaauu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3bvodhpsr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3gxfsvggw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3lhfrkqoe.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3klcglchs.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3drwbcpis.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3onholsjs.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3odlqscvb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ucjijflx.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3oyuhbzcx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3awmddpno.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3qzlqfwiq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3furxipmq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3tummdcjv.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3wcloxeba.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3azubfbyj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3hgwkmqug.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3injkpbmi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3jehqmwpr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3oasntkyz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3gwwwrifq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3nsamxbun.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3uhzugmdz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ppzujemp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3sarioedk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3hrktkwmq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3nraobsyh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kegbumis.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3wnwrvtba.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nqxszydo.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3zcntpxjc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ewdaiksb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3qoqotuai.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3ntrcpxgz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3cpfcodwy.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ksfqebpz.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3usgshiaj.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3rukriyut.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3lkpooimr.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3frblkmis.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3qanimlxl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3taxfvlno.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3wnitofgw.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3aunydtwh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3nqcpurhn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3vjiygemy.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3divjbfvk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3sehzvzgu.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3sqzoifrm.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3bloorojh.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3sxibpvrl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3lbzxeltk.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3mldysysb.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3bfqjjrrh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3vmmvhxhc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3zdcrxidl.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3itynmcpj.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3djoyjrva.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3unzbozeg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3yomqrjge.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3vlasgveq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3qaglrmjb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3kqokmtkx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3cxektqfl.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3knvodcba.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uhbtqoar.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3apypszbr.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3nocshupg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3nscacjxv.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3dwvnkrxy.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3keramrxg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3cmjczegh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3fsxexfuo.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ywqavxam.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3zhjlflvu.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3joyrpoib.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3iejlejsy.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3owkcdwgo.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3tgobtdbf.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3wjkdxgtd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3bciaiuem.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3maswwtgt.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3kkedhrlt.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3oqrymeww.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ejsbxwum.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3yahxddlo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3loxfsxaq.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ictnibqs.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3rcsbhbcq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ldxdhdgg.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3bktjedyj.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ybwwmfwb.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vbvagfpa.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3wymbrpsa.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3rqchrjlj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3oforerqd.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3tkamitjt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3pxhrgpex.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3yziqtaxp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3dnshhnlr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3zbodywmk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3kgxhajdr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3qdnpmjjs.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cvmktnds.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3uxmznpuf.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3psdytzjn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3obacyyvf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3awjrshig.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3oywozsxb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3gvovfsag.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3norxcrpb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3bdxueyzu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3pspmvoid.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3zrgnyepy.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3qnbgtqbg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3udysslhh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3gjlxpinz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3orbkeoxv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3lhlrnhjd.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ytpqgpcy.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3iibicvhe.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3tzrwqeeu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3orrzxgvt.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3wqwekcsx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3xisuhemt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3izgsrcwo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3qjconiec.html


<!-- 参考信息 -->