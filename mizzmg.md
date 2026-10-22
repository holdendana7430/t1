代发 wailian999

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2uznzvrmo.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2eczcfkah.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2uosnvrbw.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2aoaymisx.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ezojncmv.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2wmniejcb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2sqskgcsm.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2otccsehb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rrwtxuog.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2idmewrsj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2tzcepeai.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2rpvlrsai.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2neswzrcw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2cifouzrp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kkfqptxh.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2etuygxpj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qlypujpn.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2imypfxtk.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2kfnsqhne.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2uykmokja.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2lciadgoj.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2quwmspzw.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ihsdpgoq.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2xsdrrlcu.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2xprzfrqz.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2hxvafltn.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2pxlhprhg.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wkywfkhx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2vdjolzhm.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2qtdsbwed.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2tjigzlsm.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ujfmulbm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mflybbil.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2vzmlupcp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2yebvylep.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2uqjktchi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wysznerl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2datxchok.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2wtpawcmt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ekupjydg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2hxrmnnvp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2yaxjhshd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2uhytbcww.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2pcjvolcs.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2vwjzzqev.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fqmmtgqw.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2dutdllsy.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2pjbswcwx.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2baqxdgaf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2chtlthzx.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2xodijxub.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2sztcvujm.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2ouztjmot.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2xcbhggcy.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jyqihqmo.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2fgxsrflz.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yxyybksr.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nnnaciux.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mhgsblby.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ctychsei.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2hperrdlz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2refjoxkw.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2tnwqcdsu.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2zgdqouut.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2kpowsqxt.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2wawcseub.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fjedydax.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2kqynqjmr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2ditxpwlv.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2dcikiwkt.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2azdmeosh.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2ubwxzkni.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2cemvakfz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2klchscqk.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2myfmnpwb.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2mrwhlope.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2sbfhfuwv.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2btzwwyjj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2oxbscywc.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2gidhswkg.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2vozysmiz.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2mkohqcoq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2tppbjwyj.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2jhrsgzqi.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2bskeifzx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2xiielulj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2mdydvvfv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2icnodvik.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2rulkewpu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2riczkodi.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2cgxcwyhf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xmpodekz.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2umccyqjf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cuqlvcbx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2uxdhvcrh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2unseskbf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2jmjvrbkz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bvjbcefa.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bhrokvbt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2yblztrjn.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kkpiduow.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2xidmnyxz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2jdfpgbyy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2voimawtr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2jugiykyw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2nlwikhzm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ysjprlqg.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2mfikmptl.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2fizlmvkk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2kaeaqfdt.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2ubwggwjy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2wlqjontj.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2yxambpnv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2niycgdzg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2wbouceyj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2xaigrqjf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2izjwmprf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2gzlouzll.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2wpougcji.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2vdumlltl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ouxlmckx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2mjnyvuge.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ybwvlkxb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zbvsgvxx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2dvunwvku.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2mnptbfjl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sayssabm.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2tbmdikzg.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2lnbycczw.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ngimsdjs.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jljkyjmo.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2chbmzckk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ckktijcf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2zagvkqgq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2klntcssj.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2eoncmzsv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2vdpybyok.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oxspwpjd.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2nxhbghod.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2lvecbptb.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2htdnpkzm.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gasawxyl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2eqbhsvzd.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2hzrerpkp.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2iayteptg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2btzrqwts.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2mzedrsea.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2hwvmmvaj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2qzparcmv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2mdeaquye.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2yeqtsaze.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2zjanyixx.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2zcwhtflq.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2uuopfgqq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2kasexgdy.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2xoyyrgiu.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2ezmxzwqh.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2nkjywphy.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vpeegwax.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mqsrvuto.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wfyiazsl.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wlsnytfr.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2qbhxhpaf.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nspdjfde.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2kuvyfakg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2rtxiaufy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2lktrlnag.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2drggdarv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2vnhgkrzb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2suqwrwyd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2dasyfhtm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2aljuxuos.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2uwzitkcq.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2kyvbtigx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2rmcgbtiz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2rahalazl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2admgscbx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2acldjvjy.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2shexeshk.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2cwonqebv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2fucujgez.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2xrnjunqu.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mpipwbdo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2juageeqh.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2opwcikma.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2bpwqrqxk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2jihdbkgt.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2zqbcoiym.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zikgcyga.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2sagiloqc.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2vbhgrqas.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2epwsqewl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2btihdwng.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2ojfqwzru.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2thkghsup.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2cxnrlmuz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2wtploxsz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2bckbckng.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2zjotxgdz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2iwvgaxry.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ndwplwkt.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2lnxibhxk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ppbpikmp.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2wvgeigbq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2dtvpxodx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2rgpypseo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2iomlfhaw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2saqgjlzk.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2yibfsbya.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2osbxqwpb.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2puowicvl.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2mlpljxcl.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2vmgaklgk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2yfjoauyf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2uwyzypsk.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ronxohsx.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2cofroqov.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2plqowgap.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2qqjeryas.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2yzyqlrys.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2vsylblge.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2cufpctfj.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2fguersyj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2gzmghriw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2whfeglbe.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2tzwdqcuq.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2qqwqjpmp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2etmlbuem.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2zsnfkodr.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvuufigg.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2zirhlciw.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2baxgbrdj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2tnhgxuws.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2lqsgtpwj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2scodkovw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2rejrmtce.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2wxzurfae.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2xfcpuych.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2abnptlad.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2bcsqagqn.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2bbkpdjwz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2dtchiliy.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2xseadbov.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ljhhcalq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2asmqyzgc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2khgznufa.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2xrznvvuz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2wxybcdlp.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2vswfslld.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2hwfkwnqc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2hxjgohkz.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ibeoltna.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ggkamwdm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2lsgwkqgr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2zbnhptol.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2xcpbjwfo.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2kqibvwrf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wflzrdsm.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2lhoavkto.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gymqnerg.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2kewksexa.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2yezngivp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ieyrhteb.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2eyqpvibk.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2arwuprtg.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2jknmicth.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2xtvdcdaj.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2oslqqedz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2kbuptjjx.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2hrismqhk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2kdvabowf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2subvqvqg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2kpfpjgid.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2ygpzmgts.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ybzbgqqe.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2qtmrldlw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2prbssasp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2mcgyfjth.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2aoowrnip.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2eraforez.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2nknupxkk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dmmtziup.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bjtjakjv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2uzbomcsj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2zicswamv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2jirkkkgs.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2jlzlzrtj.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2sfuabkib.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2srwlklrn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2dkatyyrs.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2xsocvtbd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2mjlxcrur.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2kdcwikqu.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2ofljcxjr.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2cadxnedh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2zpsuilwr.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2akcxuazd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2reyplkao.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2ggqvhrny.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2bxaxaxtz.html


<!-- 参考信息 -->