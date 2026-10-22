代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2tztsbpyb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2xubicpch.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2orebyhvb.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2njavqdit.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2aueucpaj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2crhapulh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2iewdprdy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2zflwlvxl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2cdqzamej.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2osmbbwkb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2krrzkmui.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2zkrajrlz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2wmhubthn.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2akyebaci.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2bfhjyrwe.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2pnxefmjx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2jcuznafn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2pghqjavs.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ebzfkgmz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2icasdzlh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2lmnqjlgh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2gquzgsij.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2zpuvbhyb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2jyjgegov.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2ccftydmx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2jdvuqsji.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2uzvkgyis.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2fzkvxthi.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2nssphfbr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2odsokwgk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2msqbezfp.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2kepsrhis.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2oltxyawk.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2qhsefklu.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2fgmnpdkq.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2kjgsjwkf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ewmfikkz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2eobqwvzc.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2zyqzuvkt.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2cbxxfgoc.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2gmsfiodr.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2hecmhafj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2tmellwll.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2hreysbny.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2swrebqcg.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2zblwazrm.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2mczcrril.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2aalaxuvp.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2rnpktezk.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2fdaojray.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2xxxrzfwa.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2noemuffx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2octnesyk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2jtgvvcew.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2ekepjwiw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2wfalqpio.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2zfffdcde.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2gxoymbkx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nmurisui.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2gxdvdhtz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2edoumrvh.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2gogvqwah.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2dnqjxvet.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2qazljzal.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2yzlqjidz.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2svdashlm.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2oblvfbwl.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2bbvxpldr.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2zhpaqezd.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2dyxdkoub.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2llqpbpno.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2sqcsgpms.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2eaeokefn.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2mbutlqxu.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2dyodnute.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2dorqyokr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vzvbvpdr.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2vqpqakzb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jvuxciuc.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2wrkrayek.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xwjnyqfu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2wqnfqnoy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2rnglobmt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2bngmthgc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2kcihlupv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2okhbbzzl.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2rfustzpj.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2muaptizb.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2mumzxqmu.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bvcbyhxw.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2xvmfhftq.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xzlnqipd.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2yfwkogpq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2erfhbmzd.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2oltpakyz.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2oebsytyy.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2uwlfquvz.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2fqdltgiq.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fxcsirbs.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2feyvkipe.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mpvgfput.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uvaxkcef.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2oigyiffc.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2diljnrck.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2neheebgh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2fuxrkpww.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2tuagtwry.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2lfqerpgl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2nqzmilvl.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2igodmllw.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ifgmiyro.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fydhtkgu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2ypqtdhqt.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2kvwwetbc.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2grtlanvv.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2jnbaargn.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2hlzdhvem.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2thzyypkh.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2jtobhndd.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2omagjfvj.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ozotqcfw.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2fnogatxf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2fpzflutd.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2domxyxth.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2fgydxjpz.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2wbeqebsg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2paotdwql.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2npvqrnwp.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2dfmlurxu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2vxizehif.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2ijdtoyud.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2vjumnezq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2pzruzetq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ntzcrywc.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2dhfykrrn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wqipfzcp.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2omcpsvag.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jufdrkwj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2vadsfmty.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2beuxkzlz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2mncdzggy.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2aflnjukl.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uyvpnmvx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2nwpirldx.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2speayvxg.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2ldxuoryp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2zuezuxmm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ubovosti.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2icotsehz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2cljnbdvv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2cpxudarr.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ulmmiawl.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2dlhcjqmp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2yzklhmpn.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2xvqdbeqg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2jixciffp.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2thvtipaw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ohjibyju.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2lvmaqkoc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2aopshwsd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2fybguhau.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2coppjugn.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2oolbdudp.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2rjskdgcl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2meeexfhw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2liftuzse.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jeilbmhi.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2irmyazkk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2cmqdhijd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2yqfmwvrs.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nlmcquap.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ahzytwtz.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2vmiqdxrt.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2gpimllnj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2epqwvhuy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2waiofonj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2fzonpggm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2ypfglgnt.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2zsxthblm.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rucyolps.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2owscwrqq.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2wgwxrdcf.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2kjizqcsi.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2cxbohveh.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2darfooio.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2aotozdhj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2aapdrigx.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2ahuhousd.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2qdxmmsjw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2czptfqij.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2kukaavpt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2euqscrrv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2vudizxgr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2buzrohrz.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ujfqdukk.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2xaayfehw.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2mewuigfe.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2qsnlmslt.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2xjgpnqwi.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2pclqltwo.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ysxhjanw.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2kbreznfz.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vcyysxrs.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ayjrhwkk.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vmjbtwbk.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mrlwkauu.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2fjcujvod.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2waiwpwks.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2knnplnmm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2yfzrwnnd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xwuuqpdj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jlunawvj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2sicynvcq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2xnhguyzu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2cpictfrf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vdwjebdo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2vgijmwcv.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2mnqhtiyv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2kxwztllj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2tnnycjvp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mqmznqzq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2tbtyompx.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2gjqpmqur.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2mqtjrhmn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2moswdahy.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2auixsels.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2zvmtytvh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2xjnqsxtl.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2blnxuutc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2xaebiwuq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2vfvuvcve.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2scfcpbma.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ptuksfmc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2btnpdisu.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2stzwmgwv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ucdvlrcw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2ifcinwlz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2rcmkpbis.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2akuodhuc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2xnaocldk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2avfbmsbc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2oudfqrfr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ocsrfydg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2rctcubpi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bnkglhsk.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2hkuuzorq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cykxkach.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2fzzeybdh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2waeilbzl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2zpypyiuk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2sakqsblo.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2nyfegbkq.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2welnylfr.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2hoasxtec.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2rkgopyps.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2zxdpntqf.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2stnutccs.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2bdcrpcwf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2ckumhvlo.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2qdbiazun.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2acgfadnh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2wrgaehti.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2qzwgnrvg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2ziszquid.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2arrzjqlj.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2lrdphacl.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2licutwza.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2tvtelalf.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2bxqocmbc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2qugteudd.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qwtjimep.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2aptrmjef.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ferckoat.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2dopcxthg.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2tdwcgxdi.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2xdirqdtp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2msoytuvj.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2radunhvg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2edfgqwgg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2cjaomtae.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2hhosmial.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2wnocjluv.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rtjooaku.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2fnfuumvu.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2lexglgjt.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2efwxklop.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2anpeltnt.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2qfuvqoxd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2vjjmmvkp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2twfvhltd.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2utqiidgx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2nlfnjqve.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2kbhznshn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2eydubvyy.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2dpfgyavj.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2bheygpbd.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2tynckdny.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2dpblwsbw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2kykewidy.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2ryqxwwlg.html


<!-- 参考信息 -->