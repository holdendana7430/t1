代发 wailian999

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2npiafczg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2nvyhvcci.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2orzcoigb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2wxlsctfl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2raipbznu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2ecjuuqmx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2fldizacd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2fciccgfk.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2uzhwsvow.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2ckblveih.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2bxwgvzgp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2lgoipdge.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2kvbyoaaj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ugupdjpq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2hlujlbaf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2zhttefye.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2nmjhawmk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ydbrxeod.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2ubmjqmgi.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2vfsvrcbf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2obvvdwxl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2qztfrocv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2usonhfmi.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2fqbpkyvt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2rgdqbwrt.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2idgrjvde.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jeznqvzr.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2iikhfiqr.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2qvccyqmv.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2lkzprfbs.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mwarqkgo.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2efvyuetb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2rrtnzhzo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2wlsgrhsv.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2xihhjeqa.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2jscospmo.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2qthkcztg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2khcvseww.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2uynezdek.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2nizbobaf.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2rdxtbowb.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2akmzpzpq.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2lssrhihl.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2gmflziab.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2uvkhwdna.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2cuhwpdra.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2gcqfrftd.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2vvaxfkmy.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2sngvlmxu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2noscgvwn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2uvgeijpv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2jalxulhk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2rltckzva.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2bhqvbvic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cdztogeb.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2ernmqrkm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rykhcqyh.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ypspskys.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2mlpmfytz.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2txhfbuau.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2vsdqxguk.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2sskunqqv.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ytjatdce.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2anjihwrn.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2elmnyflu.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ssvfxlxz.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2fomidtuc.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2nmxidjla.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2msfriltj.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2aqpoqqpm.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2iemzorow.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lznlijxa.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2kxgspzrr.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2unleefzh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2nomlntal.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2qephnmuc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ruteqjht.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2mshvjbsk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nfotstoz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2guhvhrcx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2vtwckogr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2xpkcnrmu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2ubjnjosk.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2izbfylnp.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2jgtqxoif.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2emoovqly.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2amtvyauv.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qghcykwu.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2abfjomlx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2ouftihrr.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2ojjhnfeu.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2ugusfhpp.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2smspxfsd.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2psesdnkh.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2myqpnqmh.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2vwwvzrbh.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ivfjywro.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kvtlhcgx.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zefnhqfs.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hpaepjym.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2lqnnmspz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2oyezutig.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2wvtickoi.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2fzzxwxax.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2atqpzyxm.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rplpmghk.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2wetayqgv.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2powozkhy.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2mqyzlnqs.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2gmwijqrh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gkpvpwdp.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2mzowvnaq.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2jtrvpiar.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2mbbgxatj.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2egswxueg.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2jakgcoky.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2atjhjnao.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2bmcysrfa.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2sdyofehx.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2rcumtozr.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2uqkucahi.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2cleuqmle.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2udunyjnt.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2nzulkmqu.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2huoapycq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2omoahxre.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2uqmsynag.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2frdhkyzv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2jrosznhh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mnkgwfzu.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2drjdilup.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wgnfcsht.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2pvhohvjy.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2utdnqyst.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ljkxfwma.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2dkachctf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2kgsfuudh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yvapaoes.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mnbhovpd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2lbbdisjh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jsjuxqba.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2uyoezgua.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2qtqdxgzq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2wjxvhjve.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2bnboxegc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2tvvummdp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2bmkbabkb.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hefbvpat.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2zenvvsyb.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2cgjzxbml.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2lpkqbiaf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2svqpymwq.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2efosfkmn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2iezjmqjc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2uhhxtxjo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2kupmfyzc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2bbaowviy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2mlurtsor.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2uvldiugu.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2kvsrhnun.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ohcsqbkf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ycjapfbw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xxqqgiey.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gyiwbawl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2vhjwtqwl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2krvcxhzh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2hiyueoia.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2usutrjpj.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2ddketsij.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2rzbzspiw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2foojreri.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2xlzarboa.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2izoyusvq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2uydgucnn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2ikqwpjeh.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2wevsbwrx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2uvwbjvlp.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gfdsktai.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2bcslagop.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2vcqejedx.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fhowrlbl.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wmxlafwv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2rlstyqfq.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2vcqfykbo.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2nfuavaep.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2wfkaiwdl.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2adngbiae.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2awggzlkp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2ggsfynvb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2rzrgvypj.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2bzfhwdsp.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2dccvgcih.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2ajfhqzds.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2dctbwpgu.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2ppnlqyhh.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2nvckohqf.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fojacxpx.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2qmcjytnc.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wxdpujun.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kqqhuqmm.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2glwciddt.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2aekadrut.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2hdgdbmvg.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ynhmexkv.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2iwawqjcf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zgbegptv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2lhxdiidz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2irijawoi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2mzizkvfo.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2oftqjnln.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2erpoicgo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ybqtixvg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2lnropeoa.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2hkqsxpgs.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2dgncvnsh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhcyligb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2lcxvgsae.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ymbfwrdq.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2pefoekci.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2bliwdxcy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2fqtrmuoa.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2zsowhfup.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wpymyodb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2xubookbq.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2tgeikzxu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2itwljqxd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2brhuwbdg.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ywjmbbmm.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2tnovwgro.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2ngxnyvky.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2tymftnww.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2rbczvlmn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2gsbamfev.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2mmbcwzoa.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ypqvwgnp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2aztkshyf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2fqtiqxnf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2axablnvq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2dqzxrfaf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2pywecnke.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2prrinszb.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2zmhxcoqj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tfnxlbiq.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2jzykvykf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2gligemiu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2ajdbjbmp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2lppstcdp.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2zqgxoqjq.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2mmxrqlyg.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2yldzoubv.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2rnuljsup.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2rclrterr.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2vdtkzjbo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2cihsdase.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2xbqeimew.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2cdhclbaj.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2rzasfxhj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2dbgnxnts.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2zdgwtjup.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2mhykevnb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2lbxlseav.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2jeoythuf.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2eymkgyyi.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2flhngfhx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2chprcrpi.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2otcrvqkq.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ogpzpzji.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2zvpscqtc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2ahxgveyk.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2sskwovum.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2jvewabfx.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2newurmjm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2adxfvtqj.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2szobhmtt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gasrxodd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2gnptevbu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2iztevwik.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2udngkldy.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mkcdjgut.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2jfgomsjd.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2gxudnkgq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2hkcypfar.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ikphiaac.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2vtbvmkbr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2rfdwcgng.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2agitljev.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ioeqnire.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2iogwlleu.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2mxopmpto.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2abgbhhqr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2oohybhzb.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2yqwqyyyl.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2qzfpolrf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2lkuqnyfy.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2zsbnhnwt.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2wfpivqpm.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2rodkbuli.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ltjtnmrn.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2wfuvoupv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tqhftpeo.html


<!-- 参考信息 -->