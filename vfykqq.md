代发 wailian999

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ezdgkgsm.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2tjcgfovs.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2lylhkjwy.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2gdpowtfm.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2lpkobwtp.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2lcnreadv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2pvuhnmge.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2ogtnensn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2afflppwm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2hdppcmem.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2tokepfxj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2gudksqns.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2zzbnrpwt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2lnoqvgls.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kdwciimy.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2kzspohvu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ljrcmuse.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2nftyhmjh.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ltqcqopp.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2gojpodpr.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2iooucyrk.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2zzgxeuqg.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2fpuycqft.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2tazccnmt.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2lwseqjgn.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2maxyrnvl.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2lyxlqegy.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ildgcruz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ynwwikig.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2cdnaeedn.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2epuhxvee.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2pqqksqpt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2dcolzuyq.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2knoazxwj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2fmolhpao.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2hrawnpbu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qvsoyvah.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2uosfymvd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wrnxpmmx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xcvgzqdx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2javzdoqi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2kplqiyij.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2niowkolg.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2xdizuath.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2dtsjhuug.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2tqhzottf.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2sxvxitwj.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2fvookaeq.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vcumoawm.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2gffpcqom.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2dzzdyzvs.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2tdjppcap.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2omgxphjc.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2wivdqknn.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wgjvnkca.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2teqyorrq.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tumwfnox.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lnjirlvb.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2unsvdljs.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rscpxyvc.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2djrsgcow.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2zrlpswoa.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2oiharffr.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2gczgtkyl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2acngmhhd.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2rysmzyus.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2aizcrldj.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2atasewoa.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2sijmifjh.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2ykafpayi.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2bqzgvodm.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2gucigtkn.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2lsbqhkoi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2azvvamgy.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2omkunxnb.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2eawfstcb.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ozywgldh.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2butrmkve.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2axofhdih.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2settsypw.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2anrstzsx.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2gzhogqxi.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2kwzypetg.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2cnutzvpo.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2kizwteme.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2hpozyoje.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2piircxrw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2zaoafqbm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2ilsmoose.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vafaptui.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2wjpbmgsn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xdufavul.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2szocmznj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yiniurww.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2lxxjonmn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2nkvvbhlh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2srwvdmez.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lwvfamua.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bezllxlq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2buozwtuq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nubwmekj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2dgfdajmo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2phpjfwpy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2torxyazq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2lsdscpcg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2rxomzkxz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2fsjdjszb.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2zpayoent.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2sagjqpye.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jkdyqikn.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2tydqfisy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2vzmktwhl.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2hkldgprc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2rncfrrlb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2vuqcwstd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2nydkjfjc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2ffeqxwtv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2rktutfuy.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2mltsirpk.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2aruhduuz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2urhcjzzw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2mcdirqdn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2dbsyqkgk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dnfidswz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2igxokvwb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2ciugswtf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2shngpvtx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kevtdpyy.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2egkeqrrk.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2vekoekgy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xibcngve.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2govcelrs.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2agcoggcd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2oqgstxwj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2fzplqens.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2dvnaaexj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2ynvqimxt.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2metiqocr.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2sfbyinxq.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2odyrqred.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dotgcuhx.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qamwesbg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2lxjofmwl.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2rynohtbs.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2udkfuenq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2zwgiowhq.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2urogachg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2jbqythdo.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2epjlojkc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2vbpahawl.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2prgcppzw.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2gpgxkmzy.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2skxpswlb.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2zqnzhepg.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2yttyyeol.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2tptytwhq.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2gbssmsor.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2syyrufzq.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tfaxobjm.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kdfjvgcv.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rgtgkkyl.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zkjcrjzu.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2mzpyxwfb.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2sxjsskvz.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2nyiwxupa.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2jjqodllv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2tciimrbo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2oyfzoifa.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2tttxrfbm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2kxpvwswt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2slyjdqdr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2juurbfjr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2jqsofkvr.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2ndexcnjm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2zgkmfsgo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2hidsqfdj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2osymiquh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2uvrfcfmc.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2awcncwcy.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2dworrndt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2okxugfrk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2doqdonwc.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2jpfjwred.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2qmvwmfpy.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2yvjsdilq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2dxtmljst.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2gknpdnji.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2wtzrjvna.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2iydnoaxf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2mufkhgtg.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2gmblotxm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2cjpusjok.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2ktvjisnv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2vsraoeik.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2cpyoqntw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2gywftivz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2urlvloli.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2lvxchaza.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2chkavwif.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2soubbaic.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ajhfzggr.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2vyrblour.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nxdglzgu.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2xrkhodts.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2wudroctj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2fwhcqspd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2gfrxtaiq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xklgqpoz.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2ravmvzxi.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2dsbgmbjv.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2qlrognsz.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2czwlveub.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2blwyulms.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2boimpcxs.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2fvxsawnt.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2koujvcfd.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2zrttrvzu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2eciuyump.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2ewlztzon.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2sxqevgbr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2vroilmul.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2fdaqsumu.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2ezmqusdn.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2orpjigfj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2rblgkniu.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2mqcjntff.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bilmxgvd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2czyjmwix.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2azaxjzct.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2zhtgfjvc.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2gujwnpqj.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2hygdtune.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2freavnwc.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2xvdvinlu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jabpuien.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2gfjdqytb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2iobodwyi.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2vdndaojl.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2pcrjadmm.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2gdyumqia.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2vhgazwtr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2nbtevlzj.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2fabjvnkf.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2mjelxzse.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2olqhttyq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2vvcrkppk.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2kdpdwsth.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2kzwshcpb.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2qihbpovp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2kfyrfkrj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2ysoshosd.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2akijbtsy.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ycmgoioc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2ovngozna.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2zmwamrob.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2paradtoj.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2gbjlnhsi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hiquygcr.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2zuzhmssz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tduaazxh.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2cgpurgeg.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2ptlgwfhn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2xjtwbjra.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2xvzmqpne.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2zanjkyuo.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2tynvtzra.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2nzdstvkf.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ntmdmatg.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2foligapm.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2iuxhbpnp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2wlxhkjef.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lwvzuelr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2bgjgjxtb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2tbozcblj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2zelrrkcb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2kndrqnsi.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2gzxmylrv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2gtgrxkwh.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2swvluinm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2vacoqspz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2yqdlkbsa.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xerquxac.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2rrpjxwfs.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jkmmtsnv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2iqtgekbg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2awbrfwms.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2lrzndrpe.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2lfmmipsv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2bakcvzyu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2nczfacgq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2bxucggwh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2fnephoam.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2kfddykkp.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2ibzfnshh.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2aashnktv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2vexrhshi.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2awsaokyd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2zqkbcfeg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2iqypvqsu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2xaibvzyg.html


<!-- 参考信息 -->