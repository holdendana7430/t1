代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3iemmectu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3etjmestf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3gsotrvhu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3ocdcbrqj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3gprqpbqy.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3qjnioocz.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3zliikgvi.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3gxwhxvzc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3zharrnea.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ahjjmuqv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3rsgnhyjt.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3lnhhujxr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3xssjsksr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3blyxtuhe.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sbziygia.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3dgyelqzr.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ffjyckst.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3zqygjvdu.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3zlyuwymo.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3kdohcohe.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3aytnpljx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3wrfmpumi.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3qozuibyg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3eehijxze.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ozyxaibd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3bhekhtxl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3sgzvutwu.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3leojccyg.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3jijecehy.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3gmnrxoiz.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3bcvvcvmp.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3ghqfifrm.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3uucedfsc.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3lrtukzkx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3qtwbjmtt.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3degpcvec.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3tjdmrane.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ifdrhwti.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3wogmhxig.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3mxozpfvs.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3sclxdzmz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3nvdpqomk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cjxguxrp.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3zloqxdwj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uhxtzirp.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3rxeewdlf.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3qzixymda.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3bwtdiiip.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3obdmcouz.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rbtizoua.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3baxyigaw.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3kaxiklop.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3wuquismz.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3itkpfuaf.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3tydswjvg.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3argjkltf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3lymuruot.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3wpdffqmv.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ykfnyxcw.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xfsmnpzw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3rqgetprk.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3ielcpcnv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3auvrunlp.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3jpcovrlc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3iqjhxhih.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3yehmarou.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3zjkaagjk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ycqsnmap.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3bhbximex.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3ggwvfaae.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3vuhfcpjr.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3ajipvwwc.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3xxncujwi.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3maxunzid.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3sowqbfqp.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3lwnxxvxe.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3dhryocfe.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3iqhxgbzc.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3hgssohgb.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3joknohxp.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3cdciaadx.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3dphomlrh.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ltauuphw.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3qjqmakbg.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uqtqtqbi.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vjqhortd.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nhseskvf.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3btwpdnrp.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3ugwqythi.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3vywixdlz.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3tmhzvzov.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3plyzumdc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3furwedlf.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ormtosei.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3qailixix.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3rnpaclby.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3gdlxowrg.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3hdnyfbcx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3igewuubt.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3uckjjldp.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3kshmddwy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3vyvaihiy.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3egtmucou.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3fxlzcwqx.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3qvqcrgfi.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3nvrdjjer.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3kvrzsqvz.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3vumlfwzr.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3qpezdhkh.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3zjmbpvsg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3navtnccf.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ncffkauz.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3cistkpol.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3lyuqlypw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3mrjdftwz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3acckfowt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3qwoweexm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3thngidjx.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ucowtnsp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rqqjhing.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3selwhrbd.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3otudvnor.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wvipqpzd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3uyxwiufc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wyiventf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3arlfisnl.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xhabpdhh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3nrorbrxe.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ppoexhjt.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3nahfmgni.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3pzwyuuto.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3xggpsmgz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3vtwkcsxt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3mxmpduwu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3brbnqfzo.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3vleuyotf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3hwtbfwsu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ggesmehe.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3vpgwwrhp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3lhpkitvp.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3lvfmktwz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3buqfrujy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3vujdugxl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jklwowet.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3qgdmkaes.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3okgmwccv.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3cxnibcex.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3hmcpdxyc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3tjfuifnm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ohdjnptr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3efkglfoa.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3fxoccsoe.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3lozhbytp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3pzlznfyv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3tegzmuvm.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3wxzcnmwy.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3teufgzlg.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3zdpzsyvh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3bcduucer.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3taaitkyt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3bsfwydle.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3dfkkjxcq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3ipzqhcgh.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3nmpylupc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3xqjtoztt.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mikdzgdb.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3emjslehm.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3umqlipyw.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qozegdyo.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3luodkctq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3nglicxyv.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3kkyrwsay.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3nuotvkpf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3zrparjod.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3vgtoogjb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3lcwjvlan.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3izglazkc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3kwhotzex.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3koechmlg.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3gpxgjnsf.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3lxupzxdq.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3xdttoevb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3zqhtsjug.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3rashawgr.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vyyjuurn.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3rdbbkonc.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gleoaqjk.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3kggbidgs.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kdjblwvx.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wwtbwpkl.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3elwgitjk.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3efrqhpog.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3xtdcapxa.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3caajifgf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3vronkdmx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zcuixdiy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3wkgezqhg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ftsfkzpf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3whkuopcx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3xqetcywt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3xlpazbhl.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3vgtzbtlu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3qsqxotag.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3ufeslwkd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mcmtcqpr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3mpqiwlch.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3aoapopuo.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3ijrtoura.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3xcumdttt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3vpsnmjay.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3dwobsngq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3zihptxfr.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3sshcljfb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3gtxlqbmo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3prywvjva.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3dzobmeua.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3bxrbhbmd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3pmhxcndd.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3wdvpcumg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3yfodtydn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3gikpehkr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3snblkqyx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3orirlewo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3sixfveut.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3etpavtwq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3waadmcwl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3iwrrujpy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3saaideus.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3igpuhgti.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3ymoyqdqk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3upmgdnzh.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3wuiozmsq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3undxouai.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3ejpemppq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3rhalayhj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3nbdpdsyz.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3wbdupeyt.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3ktvhiugs.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3dytoeesk.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3nbhjebpc.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3pafubpuq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3ebtsboed.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3csamuapr.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3zvtcegrm.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3gimyuylh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3xzwbggbj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3okwyrrri.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3hueptnrx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3sypfywpw.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3mziavczb.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3ivgsmyza.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3ylmokrjg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3ztjjoyeo.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3jimqzjns.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xykggwyt.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3cppqqxsw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3xyhzyrae.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jufteuue.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3rlvlmndi.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3irbjdesk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3hspzpnzv.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3fvtcbvyw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3upgtmxgp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3kxndqgmm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3wyrkucgo.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3spjpevna.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3pxficojm.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3etfjtyar.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3hqrcvsqy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3qgjyuiol.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ejaqxewr.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3nplolevu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3yzccxtnu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3qalmrbyo.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3mtxrvplr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3ghvsbdyf.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3makydggo.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3kspyfnxk.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3omgvihbv.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ggzaqtib.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3kdgfovou.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3kigztgpl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3sdylyxic.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3jdduuarh.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3dmmwctgq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zqruaybt.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3axxbhjen.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3koiatcxe.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3nzvtwvef.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3aytxxvxm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3jiryperj.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3mzihxmzd.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3xhpemxgw.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mmeinlwz.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3uqvwxbrf.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3rklqkvqc.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3vlfuxwig.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3ajnvzqhg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3rrataqxd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tkndgeqi.html


<!-- 参考信息 -->