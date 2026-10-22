代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2mbnfbszm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2yfguerok.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2kdymujyx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2dmcuvaqx.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2xtjlndas.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2ifroacux.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2jxvgxbku.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2xgzopodu.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2qbxrjqei.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2eslzwufv.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2vicmpbth.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2jmbootgr.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2vbnxuguk.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2ouhkavne.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2zjzxhkde.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2zognjgyb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2quvhunwe.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2svpfysvm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2eftcukkw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2cbyjcegi.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2lovukxoz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mornalza.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tomfjsjp.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2blbjbvci.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xhwchoto.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2czfsnbyc.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2gnvkajwt.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2cjzlqhwv.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2mbqcddcl.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2roypcacj.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2awtuffum.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2mvtfduhx.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2cslayylm.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2jmmdperq.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2qsxyytju.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mfaqageq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2teughvgk.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2jlttxcdq.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2bnkftuqm.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ttwumcdy.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qoprvkbr.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2qbqoipcb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lwdwdbti.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2zxlfwfai.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zrzlutfd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2trmtnnxu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2pdpftqop.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2vrjucbyh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2faajvlji.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2irzzwkhd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2amcdbusx.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2mqvuddbz.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2hlrondcf.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jjvgbynq.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2yrhktdhw.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2febjgmsp.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ofzsbmbr.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2whvoptft.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2gqlbdimh.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2akscktnl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2tmemanje.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2limfceoc.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ecieqouc.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2iyugaoyr.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2miojdzcb.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zzbjatnt.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dtzeehka.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yseunvii.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2swrmgxah.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2brvmygqr.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2qdsfjepe.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2clcywuhu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2hwvrlgot.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2uuamdsqa.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2dxdjcgxw.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2znohgxgv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2kxcmfwsh.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2zzvvlanq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ondwgcyq.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2vrgieszj.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2padvssei.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2fdkwymza.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2lovwqeld.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ohwmhkuv.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2wkxmqjap.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2qejbpohy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2jrimhqmb.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2jpozthrj.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2vfmqxlvj.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2dedsvezw.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2muovnahp.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2dqxxfkfc.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2lvvvhgvj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2gvrhsuej.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2kmyrynbv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2esusxgzc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2kprhmlxu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2svgmnlpy.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2bnyivung.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jnzkwncy.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2anqnzlmu.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rgdulilb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2uogkjgnl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ortitwqq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2oqouhrjh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rgahnkmt.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tigdptso.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2zqgldfiw.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nxoubzto.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2julutasj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2fndltcoh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2baxhnuio.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2lzdrifla.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2wxayvqrw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2shloagbs.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2qdbmzyxu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2zxubyeaa.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2zeinbiib.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2knhfwwdj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2qgebmawa.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2hqvtnnxd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2mjxkoodc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2mevnquah.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2vkfnolnc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2hllvokgc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2hqvtbcaq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2unzezjaz.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2zjxissgs.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2fqemrmia.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2uhhizymt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2zxkimema.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2zyoxknnb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2zqtpetfs.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2buyfdijd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2etqthaya.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bivmgesx.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2pedfmykc.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2etlmfial.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2htjtvkzk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2gqtxljke.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2lzvejoty.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2kegkflxw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2uzsbrjzz.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2xrzworab.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2qbznoljq.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yvayfqib.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2fusubpiq.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2dsdejylo.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2assjovcq.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dqkoqntr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2wjlgusvz.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2owqrieww.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xvounnou.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2xseheakt.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2hsidgwgh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2zhsnmifh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2ztzsmakq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2vgyvmbby.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2ggmntsid.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2dtvswope.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2ouvvwsyk.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2pnmmjgmq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2nyxgyogi.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2hoghkftc.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2xrttjqik.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2zutkwohv.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mayyxiqe.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dhwxhyuv.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ovzxrpfd.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ptovydkc.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2jkbnalqd.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ziguwsco.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2zorocxws.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2tbmdmkok.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2phcwaxzu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2iafukarp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2rjykhdqu.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2fboxhjwm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2gnpohzct.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2fzqehspv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2jluhwxiz.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2ljkbfmii.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2airaigbs.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvpbvmdp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2zaesorea.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2gkktliho.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2fclgogex.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2zrxoytyf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2vyjfphzr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgyttdae.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rsqupsuh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2rmepaibu.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2tqgeilwl.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2kgcfejfu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2othpfpgi.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2qswwmbig.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2xbgxwzvy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2dunzhxel.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2tvpyyxep.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2hlfgqyqs.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2hmojiqmt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2nbiayhzl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ibigyuuo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2snkrslbv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2cuyicdql.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2qmmwdogx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2swgcsuvi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2sknasszb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tebgqjup.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2lwgfzdac.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2thksvdiq.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2mzjacmtb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2ephvrpwg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2flfnnvtz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2hvrvdwha.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2mdfjgzvf.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2xjoggkvs.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2byjhcqgr.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2ajhvuxtg.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2lqtxbngb.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2yrroodbl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2wdwlimzz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2sfzehash.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2zgusllwk.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2slbpjils.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2bwasbcue.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2jevufiqc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2qfyvqklx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2wlytmord.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2aianopab.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2crohlwrh.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2mzfwbkxh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2glqzrnre.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2keojhlyj.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2aizkxrcp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2jzaaknks.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2xkugbgqq.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2hongavvp.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2xpdlcovq.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2qhwauekg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2bxmjgmen.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iddhyjip.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2jkyvstgq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2xwpealrg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2izpfviqd.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2ulpeutnl.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cftnjnsg.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2llgvlpfk.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2alwigbdz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2cebhikyx.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2pjokmflx.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2nzsqaair.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2keeecelk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2cdeviawg.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2tnhxuhao.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2gyfmypfu.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2byspgrji.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2aivzumua.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2snbqgqzj.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2kqkudxsl.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2jgonfpnz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2viecezxi.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2zwiwqlrs.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2bbtjecow.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2fuymfraf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kwuyifcb.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2jpxalgpz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2epaosswn.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ybjrtvzb.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2nxqdaxpa.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2jnvemirs.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2tfdeogao.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2pxzxcpzx.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mkhvurms.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2qpbetghs.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2dgskuxxz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2mpmhorrx.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2nhuxberr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2yabjttcv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2fleyttpr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2jhixoxje.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2qyabnjiv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2twhpwktn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2rcekyjvp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2yvjbkbth.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2nianiccy.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2opvuhrzk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2qvlwcjzn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2hrqfcain.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kyomoivt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2tducxgpk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2dliyagpq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2gudopwrc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ruujtdtw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2ztjcpqeq.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2kqfguwlu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2wkwgffix.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2oxvdioyj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ilsdjfzr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2zxihgmcz.html


<!-- 参考信息 -->