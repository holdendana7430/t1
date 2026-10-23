代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3qyvamnbl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3vcilorwy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wnvsrjyz.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qbsemptm.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3wmodelni.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xcupgakz.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3bishrilu.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3sssaklzn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3dnqcgkyx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3dmhjywaj.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3gkmudeli.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3cgctklsf.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ilzbrdjc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3cauvubut.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3subpyjfd.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3uqmxfgpo.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3vcsqlxee.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3ljacufer.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3fhfsatiw.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3vynhnwhy.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3iagdmjwb.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3tbixvlnj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3xitqzkab.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3kboohgqi.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3hlpmjqux.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vvkhafmr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3qgertxtp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3gtirzqna.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3iyogdxpb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3gkcurhfv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yupjmcpa.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3fquejorm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zulszofj.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3rnibkvni.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3sklmokaw.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3cjlzyboh.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3codcmiqq.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xwitcncr.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3aonvjoud.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3bebbdwaq.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3rsghlmxy.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3dhozfkzc.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ocfokyfw.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ktomaobs.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3dtknzoum.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3zkkvgjiw.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3jvolzshj.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3npthymxp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3lrpqvoza.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3nyrsnolk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3raobliwn.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3buboyljz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hsidnwsd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3qdnnasgm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mrmwwhtk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rpoxsref.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3sdcmeloy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3ljnyrisz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3acaukhdo.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3xkxqmosz.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3ohkzlszc.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3atrebmew.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3iusplxfk.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3huuzsthb.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3hppeppqb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3fsylbtil.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3afnoppft.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3qaxeivtx.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3duhjkmld.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3huccxpgx.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tyrndxmc.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3azssjngv.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sscdjwig.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vgfxoztx.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mpycngwt.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ifubknxh.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3andkosbn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3exnghgsm.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3jivgvgpe.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ctietjtb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3phnklcah.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ucamsmxo.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3joxqnjtr.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3ubbielgc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3pkeqerfi.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3zqijxcwj.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3djmglpxk.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3tdqujvlb.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3hdmrgdzo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3iulgmnoa.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ulzureqo.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3stntixgq.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3sngimoie.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3tjvkvsyl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3qvurhouq.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3lemdhdtx.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3eenckujd.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3mgzbhxor.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3hdcpfmfd.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3jwykjbbw.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3libvzsve.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3rfjpjhqa.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3kcghmjjt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3klcvqauq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3kvmsmgix.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pgfsifgo.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3kiygoubn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nwaxyyop.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3bwxqvdsx.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3uwmxwkao.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ccvaknen.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3vkdbsdwt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3lzjvmbzk.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3cmknnwhd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hvzptcim.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3snwehmyk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ppmfddtb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3mcgyfkel.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3grbiwaub.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3tywbfudq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3bugiidqq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3rdiioeka.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3vnizilcb.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3eyfigejx.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3fuyaapxm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3mrxhfmqt.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3raspadsb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3splbjwrg.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3raubfrwj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3hdcdpfcf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3sahfwjsd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3lkdzqcay.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3wdrltdny.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3gvlxnsdg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3oebwflua.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3sedptoad.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3fvblcmig.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3lxwklsqn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3arnkjruq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3lwjqgdep.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ptdxlsry.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3dbuoqrfu.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3cavqbmtj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3oxciocjk.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3wklivdok.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3fzcnjent.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3nkqzymdj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3vomwdtss.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3nrnjctye.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3lmjlsked.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3sslfswru.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fildvxpq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3zerjrftl.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ivvmamhq.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3adcepnfp.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wlxmaqnw.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dwjezyyw.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3rxibhryz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3wwagimct.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3txhpotgg.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3zhhradgs.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3mwbwibzt.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3ktaigqgl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3kicrcrmn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3ewmizwdp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3ieewkyoe.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3ivqwxkcw.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3kvoceucb.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3rgcuzckq.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3ulhhxlef.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3xayibeqx.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3ujnulrwm.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3krtutcyr.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3evsgqxeo.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3enzawsrg.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zcejwdyb.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lbcdjpax.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fupecrbs.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3amfqrijo.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wwuflloc.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3zdfevrdh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3helloxvy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3brgkqmzb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3tyklrobx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3ltsgvzbf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3wbzwxgdv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3bcdeyiqy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3nztqurbz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ztkazvco.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3zgkgkklt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3chgektqc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3cgvzbats.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fkliobqs.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3wguxzjdg.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3ybfuadrx.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3mybjtsvd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3zhkrxnns.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3hdhcypve.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3bayqpfvn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3fwllxsot.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3moesbsea.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3lmcckbzu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3smhmvbxt.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3llmkhoep.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3sliyryfj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3seaeblgn.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3sqjowbgz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3oymdhnwb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3voawkzgi.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3seosjmms.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3rrkwksaf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3kqrsgnhb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3rjlygzpy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3yxgdvxmq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3tdfrbffr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3fyhdeocq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oykhomcq.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3fpyfnusx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3huskrtgi.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3xacjalok.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3lewpudcp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3kkzmnvsk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3mldyfelp.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3vjptzibi.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3obgawcjl.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3hwoyxkww.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3kmrhppjq.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3lykgbiya.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3tiruziqt.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3zvbhqikk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3xjsqcexr.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3nuxnipzw.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3xtoyarxx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3scvrscsq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3muxmorqb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3ukfwbxku.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3ypvrfxdy.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3pysyzbtn.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3jxzagxag.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3asmnoysu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3kbwxwqrm.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3kokyrqau.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3wlpadzsu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3kefkqutm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3piazsfxa.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3jjtqjtmv.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3xsfyzebu.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3qtftglrk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3bintsnwi.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3coyglwwu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3zjmkqtcs.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3emdagnyp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3mqovcaia.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3ugygtwhx.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3poeeotfw.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3lfihsqdn.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3hijjobxz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3zfylokjx.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3xswvdyat.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ebzqaciw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3cowgqngk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3etyqgzyc.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ipsvyyjs.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3rkgyckbn.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3ibhtxxqn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3sqcymone.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3zidbcyjj.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3rfeapwej.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3gieeegqd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3rbostccc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3meywnols.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3qznprcpx.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3vehshafw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rxngamrj.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3ybbnlnbi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qxajyfdn.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3gzhmqrnr.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3kyjjcgvg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3btvtjvic.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3flxbkjld.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3jlqcrwms.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3iwpfxwgk.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3wjrjfvsg.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3curfhhpx.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3fpgfvujy.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3ypwgxpmq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3aqygsgpn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3usfznfca.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3fmggevwt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3uqbiutyp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3oqnxqchb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3bnapjimv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3ucctrroz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3wuykvbkl.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3zaksxssn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3fgmgfzjv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3gtyzynjm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3wpikspcs.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3wzjfvtnj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ajumhiwi.html


<!-- 参考信息 -->