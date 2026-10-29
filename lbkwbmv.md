代发 wailian999

C#:   (int)resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gapnnljrc.sHtML

[L08] 并发请求多个地址
来源：http://read.share.zdbjq.cn/Article/details/goanxjmxk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.hesvh.cn/Article/details/gnwgrwzry.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.zdbjq.cn/Article/details/gflglaaoz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gabnlllmh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gnygmbqoy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/gchgtyoka.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.hesvh.cn/Article/details/gaoeabgph.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.hesvh.cn/Article/details/gwdxdbdtn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fehbvm.com/Article/details/gcgybxnme.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmnqmgnzq.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fehbvm.com/Article/details/giskmtvma.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grdgjoxgl.sHtML

[M01] 读取命令行参数
来源：http://read.share.fehbvm.com/Article/details/gpfptbqrs.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fehbvm.com/Article/details/gofofxmwt.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.hesvh.cn/Article/details/gngijdcvb.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gdegnwkwc.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gqvwkmcsg.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gadehzrrv.sHtML

Go:   os.Args[1:]
来源：http://wap.zdbjq.cn/Article/details/gkpwnzali.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/gzapczkdf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gzbfmmdty.sHtML

[M02] 读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gwlyvulpf.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gbdtecnbq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/grceluedi.sHtML

JS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gyegzygcx.sHtML

TS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gveaoifjq.sHtML

Java: System.getenv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gcyaoycvy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.hesvh.cn/Article/details/gscwqqsge.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fehbvm.com/Article/details/gbqfzjrbv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.hesvh.cn/Article/details/ghkxouzjc.sHtML

[M03] 执行外部命令
来源：http://m.share.hesvh.cn/Article/details/gjgdvyryf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.hesvh.cn/Article/details/gwfcrhisb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.hesvh.cn/Article/details/ganrjjler.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gfyhbhuct.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gldvkglbt.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.hesvh.cn/Article/details/geinebubm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/gbxwmpadc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.zdbjq.cn/Article/details/glhxrsvev.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/gvbudbdnu.sHtML

[M04] 获取当前工作目录
来源：http://blog.zdbjq.cn/Article/details/gtcesedik.sHtML

Py:   os.getcwd()
来源：http://baike.fehbvm.com/Article/details/gzoqhyfvm.sHtML

PHP:  getcwd();
来源：http://wap.hesvh.cn/Article/details/gbadnwlqn.sHtML

JS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gzgkkljmy.sHtML

TS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/geyvatpox.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/gpmbnbsvb.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/gbvrvurwe.sHtML

Ruby: Dir.pwd
来源：http://blog.zdbjq.cn/Article/details/giyjzbmpg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.zdbjq.cn/Article/details/ghjrqiqsf.sHtML

[M05] 设置退出码
来源：http://3g.zdbjq.cn/Article/details/goiftjnxe.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gewiotoxw.sHtML

PHP:  exit(1);
来源：http://blog.hesvh.cn/Article/details/guckqgiut.sHtML

JS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/giyficwdr.sHtML

TS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gpnciymwv.sHtML

Java: System.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gszmwagig.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gkyxnsvgd.sHtML

Ruby: exit 1
来源：http://www.share.hesvh.cn/Article/details/gfrvmqkzz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gcozeamuk.sHtML

[M06] 向标准错误输出
来源：http://read.share.fehbvm.com/Article/details/gbwqxddij.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gfclzxwkv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.hesvh.cn/Article/details/gdklhuwnk.sHtML

JS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gapdagasv.sHtML

TS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/grfyzryhm.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/gfbxykzum.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/gxgczhhfq.sHtML

Ruby: warn "err"
来源：http://baike.hesvh.cn/Article/details/gfvxpwyeq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.hesvh.cn/Article/details/gohccochn.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/ghbpucnzu.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.zdbjq.cn/Article/details/gurlvlrmp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fehbvm.com/Article/details/gigrwefvq.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/goqjtaydd.sHtML

TS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gpbhyxntp.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/gchlpdvnp.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/geaturput.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fehbvm.com/Article/details/gbvxspcsa.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fehbvm.com/Article/details/gbnmkrqsm.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/gnkxseonl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fehbvm.com/Article/details/glfhztkzk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/gtbjhbrlr.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gviwnlfpx.sHtML

TS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gwwulcedx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.zdbjq.cn/Article/details/gvrceaslj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/ghtpmxuqw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/ghffbxyvg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gczpngalm.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gliumphck.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gaoiyamkh.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/giplbzfle.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.hesvh.cn/Article/details/gfmyqnyyh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gpzfpirvg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/gdttwtigj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gwrpqtvqi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gochxmcxo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gncrtwmrc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gctvowyyd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.hesvh.cn/Article/details/gisvstxkq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/ghfrlnsrz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/gyojpnoxj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gxmkemndf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/gdfsfztoc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gfwqzdpbt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/geniktpmy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/giizopuhe.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gbylxevjg.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gbpmuyuxo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.zdbjq.cn/Article/details/goqsebxwh.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/gtbvvcebl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.zdbjq.cn/Article/details/gadmitxeo.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.zdbjq.cn/Article/details/gfjfajvtf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/goxecbjwu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gsbrjtzmb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/gwnvitlrl.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/gxrodxhxg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/guxjnqvbz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/gvmivlcmv.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/gfwmilgkr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/grusxoagn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gfeiitdgw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gryqscthu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gfjgvojow.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gtkpeatdi.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fehbvm.com/Article/details/gmfykplfc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/ghuxszmec.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gujgfhdwo.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/gwcazpjbg.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gpvbijwjk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fehbvm.com/Article/details/gbgpwehas.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gksvintqy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gsvjwcznz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.hesvh.cn/Article/details/gfkrbfxmk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.zdbjq.cn/Article/details/glnnavrmq.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/gjzkxznxp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fehbvm.com/Article/details/glfgbkpzm.sHtML

[N06] 判断回文字符串
来源：http://wap.fehbvm.com/Article/details/gmucjclmj.sHtML

Py:   s == s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gttmsjngj.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gdzprmupa.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gljputyye.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/genrsqwtd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fehbvm.com/Article/details/gzoimmwhj.sHtML

Go:   // 双指针从两端比较
来源：http://baike.hesvh.cn/Article/details/gwxeluleu.sHtML

Ruby: s == s.reverse
来源：http://wap.zdbjq.cn/Article/details/gnlccpkij.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gnmlynrfv.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/gijsrdqih.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.hesvh.cn/Article/details/gsivbezhx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/gxnvaqtmk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/ggbueikcw.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.zdbjq.cn/Article/details/gmxycvgbs.sHtML

Java: // 手写 HashMap
来源：http://baike.zdbjq.cn/Article/details/gstdknyti.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/gswnymnfe.sHtML

Ruby: // 手写 Hash
来源：http://3g.hesvh.cn/Article/details/glbplkhcz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.zdbjq.cn/Article/details/gvqpmjybb.sHtML

[N08] 生成全排列
来源：http://3g.fehbvm.com/Article/details/gtcqzqpui.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fehbvm.com/Article/details/ggtoebpow.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.zdbjq.cn/Article/details/gnmwdshnb.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gtolzzqwp.sHtML

TS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/ggxmiucgf.sHtML

Java: // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gpoxbdpbx.sHtML

Go:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/ghqgugbud.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gntbrnlfo.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gbdwqwqfw.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/gdopriypx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.zdbjq.cn/Article/details/ggxnzafhw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gqygllsfq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/guykvvfhd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/gupdxwlnm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.hesvh.cn/Article/details/gxgnmhwux.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.zdbjq.cn/Article/details/glcxelflb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gxuzookbw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/gmmvgprnk.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/gcvmywecr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fehbvm.com/Article/details/goabfrfdf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.hesvh.cn/Article/details/gdizzgucv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/gzrdyebbe.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.zdbjq.cn/Article/details/gmxyizofa.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/gdwyxqdda.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/ghnrfvspx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/gyazzykpf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/ghdxetlnr.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/gwolcdpdp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/grlantqud.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/gftsatslt.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gzteiajyr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gyzoicyfj.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gxqiihvdp.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/goglkjvyr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.zdbjq.cn/Article/details/giohowvax.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gculqffak.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.zdbjq.cn/Article/details/gsxjrljsv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/goaetehxt.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.zdbjq.cn/Article/details/gzlegjags.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/godhndltq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gnfhokflv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gjqvgvsii.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fehbvm.com/Article/details/ghrxjchid.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fehbvm.com/Article/details/gxhdtmtgq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gnkmcuagl.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gilollybj.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/gpaxxzeip.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grndppvjs.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/gsjfqannz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fehbvm.com/Article/details/gjfozcnps.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fehbvm.com/Article/details/gpqedmbda.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.hesvh.cn/Article/details/grfivwqdb.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/guyluvxqy.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.zdbjq.cn/Article/details/gkpowpiyy.sHtML

Go:   go f()
来源：http://mobile.hesvh.cn/Article/details/gtpxoavks.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/gghridpub.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/gmwtzwbkq.sHtML

[O02] 使用线程池
来源：http://wap.hesvh.cn/Article/details/gikwiugsy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/grstfrjpb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/gnhaudlcs.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gjuiausnk.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/genkqwrjl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.hesvh.cn/Article/details/gbubksslg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/gbjubuirs.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.hesvh.cn/Article/details/guehefsjc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.zdbjq.cn/Article/details/gvfttjwed.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/gpadhuvom.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/gahlmzvsq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.hesvh.cn/Article/details/gdtyacuhw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/gxvzgksfc.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gkxxifmek.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gsoqcncwz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/gqcggfiry.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fehbvm.com/Article/details/gboyxlkfj.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gdsikjoec.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/gmlgjnpcc.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/gueqsscxy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/gtmanfkld.sHtML

JS:   async function f() { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gbbcorfig.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/gyrpiowtv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/gjqofufwg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.hesvh.cn/Article/details/govjzqdzc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.hesvh.cn/Article/details/gdhugdmsy.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/gnsnnycac.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.hesvh.cn/Article/details/gkhvsemna.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fehbvm.com/Article/details/gwwzyxtbm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/gkmvbpqru.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gbtkqmfuw.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gvednzkxs.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.zdbjq.cn/Article/details/gcbocrqnb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.zdbjq.cn/Article/details/gjytyyfnl.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fehbvm.com/Article/details/gttepfsib.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/gpghddcrb.sHtML

[O06] 使用进程池
来源：http://www.blog.zdbjq.cn/Article/details/gtbpzbhqc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.zdbjq.cn/Article/details/gevbovbih.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.fehbvm.com/Article/details/gcqmjsdbi.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gahhnkqzy.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gjryuzhwp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.zdbjq.cn/Article/details/gxjgzgeiq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.hesvh.cn/Article/details/ggqrbmwxd.sHtML

Ruby: // fork 块
来源：http://baike.hesvh.cn/Article/details/gmkbkniil.sHtML

C#:   Parallel.For
来源：http://read.share.hesvh.cn/Article/details/gvdecawct.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gksvosmlv.sHtML

P. 常用工具函数
来源：http://m.share.fehbvm.com/Article/details/gvmwfmvli.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnzyjmezt.sHtML

[P01] 生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gpumunsso.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fehbvm.com/Article/details/gfoehjpvo.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/gbuhwvnzv.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gkstfygzx.sHtML

TS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gypqaqjep.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/gtxurcxph.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/godmnqfhx.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.hesvh.cn/Article/details/gritjlfaq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fehbvm.com/Article/details/gcuswmxgk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fehbvm.com/Article/details/gwnaxghzb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.zdbjq.cn/Article/details/ghylevpjw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.zdbjq.cn/Article/details/ghajaluzn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.zdbjq.cn/Article/details/gywwzului.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.zdbjq.cn/Article/details/gbfgejdek.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fehbvm.com/Article/details/gldxwsqbl.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/guwgdoqlz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fehbvm.com/Article/details/gpulqarlg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fehbvm.com/Article/details/gdvanygde.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.hesvh.cn/Article/details/gbbizmqaw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/gsanqndvn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.zdbjq.cn/Article/details/gsgustqur.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gehujcmza.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gykpyrxxh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/glqgnprac.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.hesvh.cn/Article/details/gbppiengr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fehbvm.com/Article/details/gzttmsqvs.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fehbvm.com/Article/details/giivedsvg.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/geqktklak.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/gtqucgkmo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gxiibpdfd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gocsotwwz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gmwnwnqsg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.hesvh.cn/Article/details/gzomlknqp.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.hesvh.cn/Article/details/gdrwjrvrk.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/ghluarkag.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gqvddnlqw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/ggwtliusj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.zdbjq.cn/Article/details/gseaqdxip.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.hesvh.cn/Article/details/gncornlik.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.zdbjq.cn/Article/details/gkosbxapo.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gcjuwmrha.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/gapdikavy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/ganiuadlq.sHtML

Ruby: a == b
来源：http://blog.hesvh.cn/Article/details/gzpblrelb.sHtML


<!-- 参考信息 -->