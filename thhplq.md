代发 wailian999

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3ohlfltrn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3wmgahpjh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3nxthhrth.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3zcxmmknm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3bjbskiyr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3gyfusopf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3sexmqypz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3zmbyeswh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3rlptlcmd.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3kxymwono.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3cmqxnass.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3obqrmcew.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3qppxgoul.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3fcsvwwxk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3hjxvxzmf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3zeompbzs.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3bwsymztb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3ldcbqnjq.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3hpmznkgp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3cifuryci.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3rrgucblb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3awddiwuv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3mqveazgf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3psidumnx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3vvhawzjj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3thryabjo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fhujnwtv.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3eayqqtpn.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3spxtyirk.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3rtyknaub.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3rafjuzvk.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3sqlvjlxq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3lucyalzx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3gesszajc.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3qserbvwz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3onsdcmbw.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3pzfzvkau.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3wochszrh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3fupyvcrf.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3utjrolwv.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3wahoffrk.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3tzpqvymi.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3stafxrvh.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3rjsbegvh.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3haenecwv.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3mjztgqyd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3tpdnxwtl.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3xrbjlvbc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3lsltmfic.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3sjavnwoj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3zfvnxope.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3votvplox.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3bxnvcaaj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3fqmdnnsn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zjbqrrjh.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3vevqclrk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3awjyftmf.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ppzzrlde.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3trgkohin.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3gjpgtvmn.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3idtkvnxf.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3aviikvhy.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3qonzaoeb.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3zfakgato.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3bsgwyjew.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3prxvqqqr.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3dythgean.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3gapenqgf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3zmnpwozt.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3dspsnzxg.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3phoaelbx.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ynamkruj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3lmkcrstd.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3fagbeoyc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mercuibf.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3xxetwblg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hhjpocea.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3qdlclggp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3eazidbuk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jhougmow.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3mjoekmqz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3lwlsgqoo.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3uzwhsdfz.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3uztxuget.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3poqirrie.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3kiqpuzbc.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3boolvcpj.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3wejmxxjr.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3wdthvrst.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3evorhipj.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3pigdnsak.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3sijlihvz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3exkfsxve.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3vvtghmsj.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zdxuycaa.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3wiblazwj.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3viohqfrn.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gmshlcyo.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ozzmobhr.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cffthkab.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3gbwmylhq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3ejukspbu.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3potkqjys.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3swxoczuq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3hrwebymg.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3eveqpcxb.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lmhjcyjy.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3nbcnfxxu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3qlpwjqsb.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3jaoqiygr.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fuvbvszu.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3thjmsixj.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3etzpgykr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3elabgoxx.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ymheowjv.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3hlwtskop.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3wmxgpemt.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3btrcwxtx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3jselthcm.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3okewmqqc.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3gdowkbzp.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3yjzdloxr.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3haqylnhx.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3yubyihnj.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3yiokvrwp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3uxbqqjox.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3onxkkcqc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3wdacntpm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3kvxhecfv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vduanccv.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3cpsgnpjy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lfuqkjmg.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3gvttkpji.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3sstvmmjw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3utxeioxp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3vovhfmyi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3kcprtbik.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3piicuird.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3akkmiitp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3kikjulya.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tmfuqcfq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3rixiddvz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3abcphnpy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3qlsiitaw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3dpuuomly.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3mmqgchcw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3einnzbmg.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xgqjkfuo.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qnlyhqgm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3gbmwzdya.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3fjekqhwu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3sfoawvya.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3mxpilqji.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3qntmpvrg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3abksjsfr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3xrcyolgb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3khmgkfon.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3byeqvion.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3taciiqkc.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ghstigre.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cruipave.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ovltborm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3csuoaiig.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vtczooye.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3hzofhfee.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3uoxylala.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gfvrjxkw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3gozrcbpc.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3ofrwckrg.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ndltplpl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jzalpdjh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ycxibbdq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gczcofof.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3wvmphloc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3jvwcqlwb.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jwogrerz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3dbczmyqw.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3xduucain.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ukplrlfk.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rjrzpfba.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pqeskyfb.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fbvyekvx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3wqekjahm.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3vxwcakbc.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3kysaevpt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3lafhsisc.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3adrjlmac.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3hhwbllen.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3vqfpqnoe.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3lwzwyguv.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3wzzeyemx.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3ytztfwkb.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3dxiesmms.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3pbgdltei.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3mnzzvcyc.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3ysxatlag.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3obsiwlyp.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3udfwkbpm.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3iyojdhkc.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wpnejumr.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gnuqhemo.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lqkkllml.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3qgisymiz.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gjwckcqw.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3vyrltbxt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3dwcgreiw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ngqzizyp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3xozidyuk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3dfakmuil.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3emaflllx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3lfazibzs.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3mjnugeyx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3wxpyrixq.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3kreakwdd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3wbmzkxns.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3gwjhcsis.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fzgeyfok.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3basonhqu.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3iqkqeysp.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3vndhbujb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3jftcadkg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3vhwwduwo.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pvgofcfd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3ycfskipf.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3gzwhzbaj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3hfnngemi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3iryxfavs.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3bidgoryv.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3cytnzxuc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3derlnjkx.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3caipikyp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3ukzwbbiu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3kqopwrye.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3cixzmssu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3sahmobit.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3neaureuk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3uhrxznku.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3loioorii.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3lsxnnluy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3psgxcpbe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zjqzkvld.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3vdvhxdrn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jdgnqlmt.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3rgzmmxno.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3hwbnjjxd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3pjytglzy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3unlcpbrs.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3qhpvdwxm.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3llcccxdi.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3ijlzwjoh.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3abjvndyl.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3yjfnhmww.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3whteoubb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3ewgzcyll.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3nvlrmvlv.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3okhihfkq.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3lbfozgpe.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3qfdzqqns.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3kbqyejiv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3vhqhgplc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3wqpajtbi.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3odbzweba.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3lizynwjs.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3wbyudiqv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3obvqtyok.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3oobleeop.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ugnceqqv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3dnkwllqg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3pmcreeqi.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xcqenjuh.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3ewvxvdxn.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3ahmkmofj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3vhyytfck.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3dmvfzgsl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ssbmkwyh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3cedhwgef.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3hwqxsrkk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3fjdovzqr.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3xwglakia.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3mgnyeqdy.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3wnzsrsje.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3oxgwzoqf.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3gjgzxlbm.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3pcnnytqy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3nqycvlqo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3nxfgswcp.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3xuzxgtry.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3zcchhyjy.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3pturllto.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3bnbwwqnc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3zsuefkfk.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ayejgvax.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3oxnxmixu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3mznxhevg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3boztfagc.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3lebnjoec.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3ebxsbnnh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ewisyjab.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3bhhslrwu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3colrywve.html


<!-- 参考信息 -->