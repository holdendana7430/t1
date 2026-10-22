代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2eqljuojh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2feyovfue.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2ekzmqgws.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2rcacntrw.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2nqzjifdh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2rsbwoeti.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zrqtllzx.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2kjufupgp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2xsensjga.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2dgphqdly.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2aqjxxewi.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2bdwjuctf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2zuktuoza.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2iisgwmdp.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2zvifoghn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2joftgvwx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2qkoootyi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2azfltapr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2lotydovl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2ukfednjb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2mahrafmx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2bpaywyfm.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2mxiowrzz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2vfmhnemn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2xmmmxdkx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2uipmxkua.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ctfptgco.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2ihwbkzbw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2bzqwkixh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2emosguns.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zobttwjd.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qkbhwlys.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2rbrbwrwk.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2jqzchlvn.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2vfgzrjgo.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2zahkvpkl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2exkuvwes.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2skgepspt.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2tghlwtqg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2sdojgtor.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2dnzcogix.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2ezynxwtz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2zbukuzbs.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2axcrucoj.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2iymnmerz.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2essmhvya.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2tojjdmbq.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2lbnqcemi.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2eclmfaqh.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2bhczuglz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2oxudupre.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2wxovfqne.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2xafmgtaj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2seiotefd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2rwevbkik.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2hfussnmu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2vlverzmt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2dkqtysdm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pdwdqvyy.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2hjauhpey.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2agdtapbr.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2delmecql.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2xnzjhxqc.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2bosemzwu.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vgzkxtpd.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fhyhawpz.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2lpqioylb.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2ofxfrkva.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2zfympclb.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2autcxjgr.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2zuatkhsg.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2opdsmese.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2nrwrljkn.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2lkhuwhdh.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2nyeckxdf.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2yhektwlt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2iygwmsbi.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2ckavpipu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2dayhndtv.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2znmqzhna.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2nlfzowyu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2gzkcdhqc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2znzxmceo.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2rcllddpt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2qsymzcin.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2bxdhrncn.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2llrrkcwm.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2pwmtkuuz.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2jbkwegha.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gowsbyol.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2ratklbyy.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vkcuqydm.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2yyujvpva.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2mlkdufat.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2apbpnvpz.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2jmgqeugm.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2yserglmn.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2xyldkhmu.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ukiivsfh.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2yucejdim.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zarfptfm.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ksifqpdw.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mjdbtrin.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yeacmfkc.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2zkxozghe.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2hgeknhia.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2uqhmlbvi.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ibftwxwd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2dwltfjie.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2aogsgott.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2bqokdzmw.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gnfrxpiq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2xmmaqrrs.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2akcjxqcr.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2dibixspk.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2yrofwgqf.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2gyrlmmll.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2vlwkxxoq.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2xoxfwvxf.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2dzvmqozk.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2yxcybysb.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2wzgwisxj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2qlucmaok.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2qdcaskag.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2jqdvpmcf.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2libnjlbf.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2tnkaplfm.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2zbmmkcbo.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2jablkver.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2ayiecosn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2huhmgjnm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2yiuypuqc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2ytphmqeg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mbwtnbvu.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2kisdsywb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2itzvlvvt.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2gbotjuxx.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rtkzjaen.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2naltuhro.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2mzzoryfo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qcqchzxy.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ckkyxzos.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2evpohxrk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2oddiuvhn.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xxqrvfhg.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2wnfnhioq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2gajwvict.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2sjpyakeo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2lzbaowiy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2hscdnjry.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2boywopzp.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2nwhrjxmh.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2vlyipnfl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2yoeajonf.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2noqqetog.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2qctbonvm.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2dhgyfann.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2uuovtakz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2somnbayu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2dkqpzfvg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2gzbdssrn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2kaqqqsdp.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2gwpmnllc.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2tytqiqeu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2rqesfqkz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2cnsivzki.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2hjeajkbl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ichgeikt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2jmgxhndi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2gwhfdyxo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2uaybyrlv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2iqhxtmbu.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2djszmuaf.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ndxzyzkt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2lulbzyus.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2mqftlrig.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2oulypjok.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2uvknzyqq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2uddktmcf.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2ylpivsjn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2qkwandaj.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2sptvvuob.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2sqpmzrnw.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2duchkcce.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2abeodkrp.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2edpzgolp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2pwbolzql.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2lmlzxguw.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2coyvypqv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2lklvbgrm.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2ztedqxss.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2htktrnhx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2pesnoxvi.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2ttclqwkn.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2mivltgnd.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2uatihacv.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2etvboieu.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2rcmyteqe.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2jvnyhibr.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2rvpmjhff.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zfavkmfd.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2djspesdb.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2nwncnznn.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ibwcsvmp.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2kyluisqo.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2okhizuyh.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2moqhpbhi.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2iipygosj.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2vhnbqduw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jccywskd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2vpbsjvno.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2uuyywlnj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2xrxeduff.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2czeqmmwk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2pjpyynbq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2iftxosrl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2nyplqesu.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2hqjdjxip.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2hlbzsnwy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2bqskukny.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2rawplqrn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ffmknmom.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2onjtkfmo.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2usohtdiq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2wryzodpk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2aytprglx.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2khnaaoue.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2rnuxrwbe.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2vdoryxmk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2dekyklls.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2dcsskjnr.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2dlejkkcu.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ntegvsts.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2ssddlqnb.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2tzmhcbhe.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2dfgxgvwt.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2etcyqfnp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2qlwxvdid.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2mcbjqrsw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2burxlspg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2fxgrcbil.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2igniqvoa.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2gaduupad.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2qjrzjbuv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mgjwquly.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2blkbvbij.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nucbdzoe.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2rzvmjkkq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2cpcdlfxf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2csohlhji.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2wuykercy.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2gndziusa.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2jzowpzkd.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2wqpyvyme.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2vqittals.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2ojigjuuk.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2tedexlxu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2erlvsntt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2siixrgen.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2wgyqfjji.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2nfuopqxg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2fgubnvah.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2mesxwryt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2ckcpvyxx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2belvjvtm.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2orlkbksr.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2raaeload.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2gmephxqk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2qxyfdgcl.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2xiuogaff.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2bzpvfbxt.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2exrajdhi.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2jqvxorun.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qncwahtv.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2bxfdplfv.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2ktokhasq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2xdoqqsfc.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2mqmblspq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2lcquhgnh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2wemlrwov.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2ptedxwzh.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2cgclphgb.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2baxsmygj.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2imqyrkol.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2fwnnajrp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2aptcfljl.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2mnltmdxv.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2matgfkwi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2gktdwdqt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2tdlqsdhn.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2fwrtjdff.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2kjkpljwi.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2kjdctvbe.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2ifttmzey.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2mfkpmsmd.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2dxuntzbq.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2aletzgve.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2rmoouheb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2makpkzey.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2dknvayvx.html


<!-- 参考信息 -->