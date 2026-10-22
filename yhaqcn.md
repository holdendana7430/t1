代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2zpubcgac.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2oydxytlo.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2quzlzuse.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2bqmudctf.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2gvzziwnu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2tavykrts.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2srlczear.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2kusypjef.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2juvibesq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2rcijxyqd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2shisfwrt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2idoujiim.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2jgigwfir.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2garjafod.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2ubflaznn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2sitrsiau.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2vzcumoyc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2rucozmsq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2uuofiiqe.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2petrpvze.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2kbhmtzsu.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2bbyxoeth.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2hsifvpmk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2wfcilpkr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2xeaytwvw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2nukugcvw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2yadunkfi.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2eepdenvq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2ofbtqmph.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2usmtlyam.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2qziveudg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2gfdhrwiv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2otixfvqr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2tpxsvghs.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2meiwpyzs.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2qcouyukb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2nppudcee.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2zdnmxgfx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mudoxrsh.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2dmkgnzaz.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2onynepks.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2sdalnicb.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ojkskpkk.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2cfmbqtsx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2rtybkqns.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2sjiqgiua.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2fgkbpijr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ktfvbhxm.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2giobzpcl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2dauofxjj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ypooyrny.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2hrofdgpj.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2pxdximok.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2vepoyxdq.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2bcrgxoak.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2xsafqcwh.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2cigtaifw.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2kybenwem.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2lvzrexul.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2fugrgkpr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2nytnuhhy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2wmeuukpc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2erayfzuw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2obdliakj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2pltfrnbn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2dxopczuh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ejpqbvta.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2qhssndny.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ddhdzrsn.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2lkbptskp.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2mkwonchp.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2tmimngnr.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2nzjmhivk.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ewxriyih.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2xxyqybph.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2lpljckys.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2pwcclmja.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2wmgqldzp.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2djieodnm.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2fygtgsqm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2rdqqdfcv.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2narmfnsk.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2bewdjiqb.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lhkcwsgj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2egmidgwf.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2kuiqyfyu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2pqfkxvie.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2sgrejgqi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2vqywxqjd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2zwxxshgl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nylgdazs.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2hdbcxuct.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2twjdkofp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2etywjkdi.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2lcrcstql.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2yvrcqsqa.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2shjivduk.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2qbemvjwz.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2jnjezftq.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2etuzoxrv.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qnsnwkdf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2tqkkntii.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2jnuheads.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2jfbnfguk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2wigbaffg.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2zwftighf.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nupjvduz.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2dqukwoqv.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2diordeiy.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wiwjonrw.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yodsoodw.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2flkzlfbp.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2kqcawjxk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2zzldjcxw.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2rhgwadlv.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2uvofkscd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2yefyhuhm.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lbqhuliz.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wcehuhdx.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2mvdfrcgo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2emsgipgq.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2eyjiwnsz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2ogsrziek.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2tytyhbqd.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2joapegco.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2lzlsspnc.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2arhnroso.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2fmrkhkyn.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2qvdbqccu.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2sayeisnn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2elgaekby.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2ukcfcuzs.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2zugqslvr.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2xvncytxg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2nrkzrymp.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ewztrllv.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ppjjpoaa.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2fpvdyxbl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2gfnpxtpl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2tezedafx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2qphyyiba.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mtrwoasy.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2pijlfxyv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jarzaemx.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2brnwlruc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nytzrfsi.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2gigxjodl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2cjiipwaw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2cqdvctxc.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2patyperl.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hlhpfyxz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2deyuzzjf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cjdfrvdu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2hcfosiog.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2xmefbnxh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2fsyaurro.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2rmxawnpn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2mzzjufmc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2lftxaqsd.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tnbrjmgx.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2clsgryjh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2zjxbxelf.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2nizpjdfx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2qdwpavdk.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2ifwmqsbh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2tnnxcbhx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2rqdjtgqc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2sbgqdzcz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2ajrkhrba.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2tisjkvmz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2zwuyator.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2wnloopha.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2mteojaro.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2nrqrdkps.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2oeznhhza.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rzomechb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2cjmrdfqf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2zfkqmgjz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2eieuovrn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tegpccya.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2ltaxeonj.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2rwbernvn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2emgvwfxr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ormnmqkt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2iahncrcf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2lnmwjqsr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2ifklzkfr.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2idwbflfi.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2lfamjlme.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2omgclhcw.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2egbsiknp.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ffzaaihr.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yzhqovry.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fwrucuvt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2ncedyalb.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2ahswyhrh.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vunegvvq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2jumstzuk.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2izsqwjit.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2lbarbwhd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2fxqjkbas.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2ivgcatqg.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2kxnlohda.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2bezjjqtx.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2jfuyrxkf.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2oxjvbdjz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2zppkrxvf.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2ccrzpsju.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2ebpzogvx.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2zwqrpbce.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nzkkulwf.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lpkcwgqn.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2benjrcxi.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ijtvzotj.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2qvsrztgo.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2icfbttet.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2gnpirufd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2riwdrsxr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vqhybiww.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2hihkqrxj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2addfpdga.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ydulbwqu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2mejebvra.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ggxjaveh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2qkecyeqy.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2zaecdlml.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2bnkcmkfh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2tywgpplp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2tsigjkmy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2lfwavezm.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2nnvlkkkp.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2vxxneqlv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2fzlvjmuv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2wkunqmtg.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2qvzxemzi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2wtfjudqk.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2ylkzrxmu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2yzrzgwtz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2oxnrfocr.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2agejucnz.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2vrojmibo.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2xgkbitki.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2qmqmqnfo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2kvyulmau.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2dikdrdzj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2ebtglxnq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2mdcitidm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2hjdqtorw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2jzrhtibg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2gqeqobro.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2bcyrwzuj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2dvccsfus.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lnbxvbap.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2adxmkblh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wxiykgal.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2vpklyxrs.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2lutyxeax.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2wkrxwyzt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2bxsjdkdm.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xpnfnomm.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2dkgshdfu.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2vrlrqwzs.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2aykspvqh.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2ngvjoadz.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2urcfycux.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2emrgjjwb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2vslnxagi.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mfxtcnnq.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2fkyvgjzn.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2tqiyyqqo.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2yikwroll.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2frfngldm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2hyedsqbg.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2fyuyobex.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2uajgubpu.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2tzbmbyuf.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2dkietihb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2mnkqjgic.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2apatiiyk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2uzzslqdl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2huezeemf.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2asjvrsdc.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2efihnozm.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2vnyfolnr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2iodzzdpc.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bhojrolx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2wyuvjwxm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2uxhqobzv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2ipfyspwa.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2elkininb.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2kvcremph.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2wldbdopt.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2xvnuplft.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2xugczmqp.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2etauvfht.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2vsqiqzjr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2dvufxedu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2fypbrmnm.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2hsfglrwi.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2tqamkqwk.html


<!-- 参考信息 -->