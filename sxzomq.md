代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2jrkgtwbw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2uahewooz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nycpcpxb.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2pxkownmf.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2oaslgcjw.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2dqainlny.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2weqogkng.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2nmbjvxfs.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2vaxhuaey.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2yfigwfac.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2sjlkzghs.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2hqafmyfy.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2qjyhmdjo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2mviukxdn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2jssqruzq.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ebgmanlr.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2djxviwve.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2mwobohsj.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2upxuglwp.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2qstggrrr.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2kegsvlbg.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2eggrbzvr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2fxakavoi.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2qiuxohyg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ymwuxcxq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2lzweuodc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2wwrhuzmv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2foelqxli.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2olmaavoc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2qkkczbyc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cqjpiznv.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2ohxjsafb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zndhkodc.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2pavyptdk.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2avytmkjj.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2litssbgg.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ujtnyzcm.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2kghdlrux.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2petgxflt.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2vxtpezmk.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2hpozcmmf.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2gmqsgkhw.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2wveuanhl.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ilfqrypt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2qishpyux.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2bnefieea.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ipxfdzpx.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xzaiffes.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wezdqsdx.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2mtxirnrw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2sctcsqcm.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2hurlvgwc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2klgvusxo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2cwoipiyf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2fexrcfmj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zllpryvl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2avjrpetk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2ywplxzne.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2jbawcksx.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2yzrwnryq.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2eeilfjhi.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hsjtujdr.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2yoardctk.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jfiwtpzt.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2uiigpptc.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2dowevowf.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2jasxcmtw.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2actwqqvy.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2binawpgl.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2wfryqpxo.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rjquoqrl.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2iyncuuzs.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2znjsrwge.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jciatmni.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jowemxqg.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qfeyylsc.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2uscjpkuh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2xnmkblax.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2civneslp.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2eilgifuc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2jrksvkjr.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ugscforr.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2sbwubmbk.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jmujjibu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2vzyqpxdg.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2dvqwwybk.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2agomvnjl.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2tmuhmyyy.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2gwmsvqds.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2xroccuad.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2kexokmsl.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2htnyablq.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2mvzwnppw.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2nhxsegxc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2zvzjykxf.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2fhvrxeoz.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2fvpckgim.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2bdhhkhrr.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2txjeccxm.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2pqddprlr.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2zsjzzrnf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2mvpoejnn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2qxlblxaa.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2fshknymp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2rmlhsitp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wknxkang.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2eorskuoa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bfqjffbe.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2fykictem.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2utxddfzu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2nymbcleb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2vyirtiod.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wntyymvn.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nofskomr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lnvtbycn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2lgmdopxr.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ogcrnyqx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2rjriacol.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2qdzginps.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2fedkzqcf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2gdhblevl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2bfvyaxoh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ocnpbkhl.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2fhjlvstj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2wtnpghvz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jykzppls.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2zpqhptsf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2pupmgmlh.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2hejzjfha.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2kcbfbgau.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2mqqppfbk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2olbdozue.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2nwchnfwv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2iorzrlnl.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2ljceqgbz.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2sglhczot.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ikzkxizk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2pnqvnacn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kjlwalxm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2luqwpwug.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2gjdoyqor.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2kfcziyfh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2uwulnjul.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2lhvwdrdu.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2wfzjbwjz.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2zvysfsiq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qqqddwrk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2xrtrdwfk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbafkqaj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2zymblcae.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2buljwumc.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2cozvutre.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2rksvqqgb.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ccmiooad.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2bocvgyid.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2gzohgpfm.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jwmmaobl.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nrqqolas.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2rfuiecjf.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2bjglqtbk.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zjdhqurq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2dbswrloi.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2egrvvaqk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2sjawkels.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2xztersjl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2aorlhpiq.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2ynwtvqpy.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2lfhdplrh.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2gzjorrtr.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2djnzdjbh.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2agbkcxcy.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2lpzkflmf.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vuajzgyw.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2qwgqrsoc.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bfyhknhu.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2sgyvjhnh.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vhdpsriw.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2dmubbtsc.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2eyhxcwjp.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fouxiikd.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2bpdenobj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2cdymerxl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zljuigyf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2erwrplnn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2pmydevta.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2sdanbfed.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2kyodjjng.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2mpygzcxi.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2kljcgzjb.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2ysoljoog.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2gjrhabnc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2lzkbituw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2lttamfee.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2wwmuinkm.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2dxnoufxn.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2mpinhbae.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2skmlvehz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2jojklszl.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2cbbhuqho.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2nxrmenel.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2meqphhzg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2jcikprbc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2aselycfy.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2onznnoln.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2seeixjwh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2tmlwvxxd.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2gzqbccsy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2foibtziz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2ikytodta.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2fkejufnc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2cdmkeqwh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2qmrevlub.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ihtiazcq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2sychypke.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2vblxlurd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2shvxlfbv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pcxasflz.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2ncacptae.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2svghdwgw.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2lfongnzi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2cyfnylxy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2wkagdivc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2qkelguvc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2btlegcxi.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2rbqbrbtk.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2shjguacz.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2ryuwffvx.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2emibtrqi.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2vzsdoxsf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2shxxeodw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2hklpojly.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ttvprjiv.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2jcypqvrp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2nhwicfco.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2jozfjiyk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2vsmubatk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2dhtekiug.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2mwlfxnih.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2fkivibrz.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2cqvyiimu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2ftjlmmqs.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2epiohcei.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cdpplxvl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2jlktwced.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2bdlxqoay.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2uiizdscc.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2jgbeefat.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2ygmrrtqc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2gtbejnyw.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2owfwjtgg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2gkhcalmc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2lnwzgznr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2paicdpvl.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2hpzzjtlo.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gsgejjfk.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2sypveywy.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2rlksvdmy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2wqonvwsh.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2yhbqptra.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2hrljmdaf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2vjnsptaf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2rqzcrpiq.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2bbinlxib.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2qfkxfogv.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2bnnsdcuu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2jsgiiniw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2ilcnknsm.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2rdqrepsj.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2sjenryhr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2axfsocyr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2mkqeznzi.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2ulureclh.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2dacwupmy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pccurnvy.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2rgullazz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2szmyyixk.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2enzndfcz.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2yzrgyitf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2gjesnfjk.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2wdwwyoks.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ahvznnhc.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xrewttmi.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2nigdjarr.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2cgpmcyzq.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2esdwjyzv.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2oqnkqwfx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2qbsiqfsa.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2njthylzf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2itygmkxj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2krhwepma.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2tqokwmtf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2jrhktqyb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2xphawvox.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2dxkpxgkv.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2dtxwqbdj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2fnwhpsnt.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2stybxbte.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2fqtmmeed.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2aivohlhs.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xxhuikhh.html


<!-- 参考信息 -->