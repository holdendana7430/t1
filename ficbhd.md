代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2qwofdlxz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2ghgprqni.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2guhgifjt.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2amhmqwfz.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2chdpckdm.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2jelxhsok.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2sysxuiiy.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2cvpsgtio.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ibqahzzz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2pxuqekwo.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2woixxqbg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2vghisszd.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2sbsmcqby.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2lxxkplkp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2juldkhri.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2xqxsftgt.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2nhzpykky.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2pgzalyhr.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2fcuytvnc.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2nianbglc.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2udvwedff.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2fnkfjniz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2ezlupxgg.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2rrmgyhvq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2weckngae.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vduokrif.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2jhxtkjrn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2jqgsfism.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2bdurqwjr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2mhbactor.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uluqlmbs.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2hredrgbx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uldxerjs.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2yzztyzsl.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2bgmpxxnt.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2zyvyamnt.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2kujkeegh.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ykfjwqsm.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ewdyzrpg.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2guunzyiq.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2zaifwvjn.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2uxbvtbrv.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ucvdjfvk.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wocjknmi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2akzrnjzh.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2icqdtafc.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2iqppzzmw.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2oaqxsixp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2bwcfttho.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2cfnvhben.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2tcjmogxm.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2eoidyrnk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2hvuxwqxt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2xgvvacqd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2svztzlqj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2xsiazdgm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2jinwoyxp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2uetbphph.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2wabvgfdz.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2aiwlkstb.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2daugecxx.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2thjtcugp.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2nlxohkwu.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2johywuym.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xxytnlec.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2tfhaayja.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2lohdnjkk.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2tpqlpthn.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2mxhplapq.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2rebccnfy.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ycfksost.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2dlnfnyjy.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rfspgmyq.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nwfddyjj.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lcberyxz.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xtwcidrm.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2jgrngiba.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2jsiruiun.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2fbarisrn.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2bexudmac.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2qzwuuqyb.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2rdevsody.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2foafprpr.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2nmuvoikg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2tiuezmpj.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2jxideyfa.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2agddibbz.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2ukzpivho.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2gajjnkll.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2uqowonus.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2nzdiokey.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2tjxokytc.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2hoipkiid.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2pezqkubs.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2fhkqjsae.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2kppzrckq.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2jamnftyq.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2ohcrtexu.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2gsnvxxqw.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2nwfrzzzq.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2lkggqnci.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2ieguhvgn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2qxkvmnud.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2lfykilef.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2pkvhfdpe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yczyfyoj.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2scizvesx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zykboewp.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2swibsdyg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ukdkexir.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2dvlamzet.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2vmsckjiu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2mpdcjmeb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ctjjyjkb.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xvjyxwrj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2ttveyzxj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2msafvitl.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2mwtmsfnk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2bqekuiwp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2poahhmle.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2hyspveor.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2lojitfmh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2fricsoug.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2codgfqzx.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2faurmxgz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2drpycqwg.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2whtgudsc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2suqntkhu.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2izustvgf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2uiwnlmdw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2cedauvmr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2lkavtqvx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2ivxsdrta.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2haqovlwm.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2dbrnbzno.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2xdhvqkbb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rsplsaxs.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2tqnulpwa.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2iacixbci.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2zlezqwli.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2vwccxymo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2ynaotcdf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cwrrxogi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ptcixhoa.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2cojnqybv.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2nlpybhpp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2jvbgkirw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqxxylcp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbqofoty.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2bxrivbpl.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2dnmcwkld.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2ljhhwrge.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2luecrdoa.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lsygiywd.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2wnodjjkd.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2vquitavg.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2awgmogaj.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jbxogmsi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2cfbgtivg.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2bmgkqqmh.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2jolhsaps.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ypotlutb.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2igvxppoq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2xuxjmxzd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2uirucjca.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2ntylupgq.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2gbdzghui.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2qdvjrlih.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2jlxcctwq.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2crqybaje.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2rdhxffam.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2hqkpdvme.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eqsipaeb.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2bbcwaoow.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2eyiphnoa.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2cmsrutvu.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2srzxxsck.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bngxdind.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2nqpfgajs.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2utitande.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2gfgbbwxh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2fzqcqmll.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2kgdqsdfq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2nauwxphz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2uuuwnhoi.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2pbyslese.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2lxzcknvi.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2fottdxxk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2jfnjseoa.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2jcysoprx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2okdykubc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqlqykog.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ldgyotgv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2taqifsuh.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ohzrupnn.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2fexfntbz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2wnlnhqcq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2kyyozqhu.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2hgsqnfcq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2docmxmip.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2jtvuhoky.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2zbixhbgw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2cxlknlfg.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2uzluwmzb.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2mxvzqmhu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2rmtmubzx.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ikzsfruc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2dxxxrlyj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2wwdrqytp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2qhcjhqci.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2zmlzdqrq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2yhqlmqfl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2dkqynxnr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2rnrvtywq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2bwdzguuc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2uxkqvbik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2otzorida.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2mocaksgq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eezjknzk.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2bsathzmg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2egbegska.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2tgegocta.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2cdsgxyaz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2cwpxpuud.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2clnbursx.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2vuzggxkn.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2gujonkng.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2rgcmzuxl.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mcxqffae.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2dbrnknik.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2ihtgwsst.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2tkvxfmyu.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2skujwkhi.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2fjjdizus.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2nuvpdwtk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2eyifmnji.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2szgfkzpx.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2jrcescdq.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2pxagptvh.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2dgqjsbfj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2fnvsiopj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2bludsafg.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2acsvqwid.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2drivplja.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2edydutbf.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tcjxohpp.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2msyfxyyd.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2vqjwplnx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2patibwwq.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2kdvmebjn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ysbksdxe.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2utmzdare.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2lvcokjvg.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2bpkvfytn.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sqauzmjp.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2rhdcnecn.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2izqqjscb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2nntfjfwe.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2uqvusowm.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2kinvuphm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2ifhladqb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2oymrtcxg.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2oibgkrjt.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2kedornxa.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2xntfrico.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2gehgqymt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2ogjpieol.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2yhrpxkuv.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2jjmfvobb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2wmdawkcp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2pcdyljag.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2chekuhaq.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2mzxcmtad.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sjsskdrd.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2jkhhypcs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ifsxtsln.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2wfqnsxwp.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2dkigssyn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2xywmbffg.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2fgepbsqw.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2nbazvyhf.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2hxiywkij.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2fxmlzyuw.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2hxhshtbj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2oeesykhy.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2nsopucjt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2oygcdtno.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hnxhzujy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2mmdzcwml.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2aloscdwr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2phiunqml.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2adrmgebd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2etophgzx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2szcpzgcl.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2rmmspaeg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2btaqnquf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2jyjfujav.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2billrkge.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ytibbyvj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2ulcmzvol.html


<!-- 参考信息 -->