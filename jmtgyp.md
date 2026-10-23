代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3wyldglrh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3wmfzdtyh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3lgredabp.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3viqquchf.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3thvczvdb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3ehwzchji.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3zgwvycez.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ifgylhbw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3rcqsrbrq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3jlkfslhb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3vwsekfkz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3kmvzjivm.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3dleabzia.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3wydmnzqt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qkgqpixz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3jzhkgbry.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3wmgacqmz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3upsobpvp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3bdzuwlea.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3glaiwkhg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3rmeymspe.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3bptxcvqg.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3ofejomud.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3jjhrjdhl.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3hwfieqaa.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3mhgzlktc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3lmlnbnex.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3ehhsxovq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3vjsidkwl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3upsytmxj.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3zxlhpjtf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3nbjdaacc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3dhncikdx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3bkwbmkpn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ywtweuhi.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3enssxyjm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3radsiwjk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3bojydhot.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gnrlrlcz.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3mqpekjzn.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3zpzuihhm.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3phzwdzmo.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3pzgirrgk.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ttovewdf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3lmuziwgn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3nieaszqe.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3jeolvdau.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3ddbeqszb.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3yazvekpl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3qgorbxwm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3vekoignq.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3fydgppmv.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3xrkgkxos.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3ldbolave.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3nojznhgj.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3praqsvjn.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3culabfro.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3mwcsomqg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3frhgqsjg.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3lnwotgqu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3zrvszhkj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3pnzdisrm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3wvggjklv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3yjcuobkf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ypdhivwo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3zabdssxq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uhqjtgzx.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3cbluaifr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uexzduly.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3sbujmthi.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3tmxwmacj.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3uddduqlj.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3icygppdq.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3wpwzdcql.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3yiekrqyo.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3yhrxqsel.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3xhgganzv.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ahkbnovy.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3yavtmqpf.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3kwzbxnek.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3trvwavtl.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3qyhjxppf.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ktmbbszw.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3vijitpfg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tfgypwtv.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3plaiwkqa.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hhbsapzx.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3ijzorrzo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3iampmilu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3dtqifwdk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3qqhtzibw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3grdvutbh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3nzpsvspt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3aqyeuryo.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3jjxvhaih.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3wqayvbbu.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3eblhhwmb.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3ornmgfah.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3cricslmu.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3xerfxhxl.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3cvfydnbr.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3otgaumnl.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3nietyfje.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3uzibekfq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3wchhokwg.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3ibdithid.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tnjfpsgp.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3ooylgiju.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hjaxyfie.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3aabniqeq.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nteantmi.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eiixkyjy.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3ejdgllkm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3bsxrqpen.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3ljqupgap.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ajkwshrw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3plnrffem.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3xkwoxzaq.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3retqukby.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3nhasxsrj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3tixbhebr.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3pfgiqkyp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3hhvorvmc.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3lbwjpkbb.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3ffsqgcgh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3cmmqlshi.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ktboivhi.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3oridksxw.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3geapwauw.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3tivyrgfw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3mjhrxemj.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3gfifwdpf.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3hislynbc.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3dgldbmjf.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3opgrruil.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3oqkpfzrs.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3zxwspydj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3oeirdjdh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3supbsiaa.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3lnjzaidh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3awmhjhtf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yuarkhov.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3ifpqipyu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3agkcvrot.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3plqdxehj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3casvepgw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3pedhciyr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ewwdmwdl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3mgqssknd.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hxzibjyj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3accrbfkn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3iyuuwhtd.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bsbwcdho.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3npvlpfvd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3dvscbapv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3tauefixe.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3imctgftg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3jiwelsfj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ixijelgu.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3khcnenyg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3oegotekl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3dvvibwii.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3aeislbbb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3qzfjfatw.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3mrdexzgh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3smobbbfy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3tvmrpdts.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3hurkxjga.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3odlmvzxd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3eyjgllfy.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3kaqtuqbd.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3mslqwacm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ytfjznka.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ymqrbpei.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hcqzibzg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3krfajxfk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3pnbkbhxq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3ttmcdxwp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kseifooh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3wwqcfrbi.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3ddlvfoen.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3rblzwbve.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3konutwmh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3mextfpar.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3najgrvjv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3pvnhugel.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3ghyojkyx.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hkiadimz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3enjiluok.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gposkdya.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3tuewidfo.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3aishbejd.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3yxknddde.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xsrinbuu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3heppkzyv.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3xgzqvsed.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lowqebxt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3zfopddui.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3tklmrxew.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3qzmrcaef.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3aftleclv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3qeunahha.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3cpelzotr.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3efuveoks.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3pljhntlq.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3wapmmarm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3iforeiii.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3frsfbmzp.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3qsjuwnoh.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3atqbemmq.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fkflxvrh.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hicprsxa.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fpxqqbly.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xojirmra.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3qdqrzofr.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wsnprrwj.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3jzqwyffg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bejyumbp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3idppytzp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vczcvjbu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3mklzfqlm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3awtpkrzg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3azndbsxd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wwqvudfi.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3wuqpvxql.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3fzlcoexu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3ehkdjpca.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3gvtzfpfu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3ssokmjwt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ohkeqoya.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3izgqblyu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3fzygqdab.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3fwyvjtwv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3yblrfrpy.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3jedwhbpk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3zvjdghtc.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3klfhuyob.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3jkrafhzf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3cppwdvcc.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3jneoswmi.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3tjxmvlhy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3xpuqmgbl.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3dssfbgqx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3qlputsgk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3jlqxqiug.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3zpqkwwkn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3kfacrhsi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ouslrdmo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3znvfubmi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3fmpmrkia.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3tfphhwod.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3grhslcra.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zcexlvru.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3rkaultof.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pwveteai.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3vuecstfb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3efuljxbr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3bvwicrrf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3ryccectx.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3tjlnrwnf.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3mqqibkxm.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3unvgohlc.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3tjqwqcno.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3cikmdxla.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3fxiuomjo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3huqalrih.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3dnxpubzb.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ibiwimew.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3naivhwbi.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3osqtrqvq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3wdvlpgil.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3dyglooyl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3pmgersuz.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3cxrudpkf.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3askctwje.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3lyajkzvy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3prhmxskw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3stefohvy.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3yhvzbzwd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3srenxfdg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3jqdksfbr.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3yzqprzlz.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3xhsmyauy.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3xebpduja.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3ohesrnir.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kulumjmj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qnitzidn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3axohgrdc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3qgemfsrz.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3xnbmsylg.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3zpfzxzag.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3wdraoruh.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3fhplkwud.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3gulvqoqv.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3svitgmia.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3klrmjfoo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3innwrbjt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3hzhjjekg.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3pecicric.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3feugnoau.html


<!-- 参考信息 -->