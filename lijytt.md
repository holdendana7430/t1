代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3pwagloyh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3jysifyel.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ligfcjei.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3qdhvvjht.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3hnwwpmyw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3lmbtslhz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ghtaiqla.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3qnqgfgil.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3wirecocw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3iavgsdug.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3oxbdafdp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3vfpfyccr.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3rtwebtzq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3ulznbszp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3yvkigqxd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3qmzaqhxd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ktejbzuk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3cwlyypgv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3bjnrslgi.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3hzrvlyta.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3adrurjvr.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3noeozngc.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3kigbewea.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3jpaieapi.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3kgmhbccc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3saoeozdy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3mjmqkpbb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3ppfkrrqe.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3hnchizdl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3xlbwamqd.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3yvmfqbln.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3btbmuxby.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3hdibkggn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3nxnflkwq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3lqseciaj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3qnfacneq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3mktzcwql.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3nbqlkkxb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yrulespp.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3ensgatwa.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3crwwalee.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3cgljvunu.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3xpayrefq.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3uzmeifmu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ydvkezwo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3qbesgtfj.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3dpfylfhy.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3dgtzgfkc.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3uvrfarbg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3nqclnlwv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3clrhxoph.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3stlwaeyx.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ujgdcffa.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3vhbwxure.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3wqsuwgjx.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3kjoonrov.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3bwjmjizn.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3kvxbnvzg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3gmtmuayw.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3xpohzjyw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wnahzplv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3udbnmjvf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3ejrmccmq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3cwnkhrlp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3tjmcvnyd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3podimweh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rsuqqrzt.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3oepegxif.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ubcrhrjk.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3mseflobq.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3arxdtzgo.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3xhvocihu.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3zbhvuahf.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3zxxlnghf.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3gpvklacp.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3aziyjzva.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3cwhtykpm.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3kowwndwl.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3pryyxpfv.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3vaakracs.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3etsmxbyh.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3udmtnmkk.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3cflrrvxx.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3aejsljcc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xwgnxsdi.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3rqbfcaxm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3mndkybvw.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3uervmtxl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3kfcelocs.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3morvgsha.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ucbhfiha.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3qtdpetxa.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3utenuoyj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3cvcudtxz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3dfioqtza.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3nsjdbggn.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3koayvona.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3hxtvbync.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3ylosjavn.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3jaaaoemw.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3kivzcras.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3uyduqubf.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3fluwwnnm.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3kcgdmrbe.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3llmoxefx.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3prhfimvj.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dfuasmqg.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3gibejllo.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hhbgegza.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3efnthrbu.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zrepmzdh.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bydbfiii.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3syuufyok.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3wczwtinv.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3ztaxjcns.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3dcftuveo.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3aldnnofp.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3muqaffqh.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zlkhhtyi.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3psztkodd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3pocdijfp.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3iscmymah.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ugjbutgh.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3azlaosut.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3qvbrlktq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3habcaqgi.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3fwoaokbm.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3knmqiznp.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3zuqgrrhr.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3skfyjfia.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3xzwpzdbi.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3xnhzrfxq.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3zfljlpnc.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3dqvbaxab.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3xoqxnvfi.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ckogdodk.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3fgoihlfn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3lkcqtkgu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3fcmiiiwc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3semxzlwl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3hxoibuje.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mmipnmez.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3mwilqcsg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pmnbypyc.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3qeqzjneo.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mkhnhbub.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3avyhcapx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ihmbcrbs.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3xsfyucug.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ychivcsk.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vbiscmwo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3ekktlkjo.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gmazyaki.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3jluagkex.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3tqtjaeis.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3fonozixd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3uuykyokt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3eeqtdlpa.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3tqqbdqye.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3hzcmarqr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3bcxehbks.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3qllaoaqo.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3armpoqdt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3bdtdiijg.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3khcephfj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3bovpxqvd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3twjcplua.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3lqjjodzc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3feyyddef.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3gjfvbwus.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3fsjzkhic.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3knytbgql.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3whnbzdsc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3pfkhiztw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3fesjrsxw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3revulrwy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3anavuuhm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3fhkhvtdb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3hcqqceku.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xgagsaso.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3vnshwfdt.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3vysmxsui.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3bduxojxx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3pahsulsc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3pozpbpvk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3egzjvglh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3ibkouwrg.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lbwliasn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3sblwulim.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3vxyiqzgj.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3fixfucet.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ykoxagis.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ymubmbfx.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xwbkqtti.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3wrtiomji.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3qdqfdvyc.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3gkketmvc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3tlvhcaye.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3fcysgjuz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3xfwcyhbi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3xwaxfwjf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3jwwsnbfm.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3xnrcgcgr.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3ogbmeppz.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3rldvguax.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3areinphk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3iaetkyfw.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3bqfrxgca.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3omxkondg.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3dldfvbll.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jqrobacf.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ynhjunul.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3knqfxxqr.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xrfuqczi.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3aqbjflgl.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bhjalslb.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3jqeretxm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3srgoaies.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3qqnshipf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3thcunddy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3aewmsoxe.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3blqaevei.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3fduaedwb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3gldcvmko.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ylnlzzpt.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3kshsxylb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3loywykax.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3jsbzsadk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3smfyujnd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3utacikgz.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnwcutrr.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3jvfphojn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3kqdwrbwt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3bwqhnjdx.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3lrlcxlnp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3vbkquzji.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3hbohcfig.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3dqzhywep.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3gbhvlswr.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3jtqjgzpx.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3zvfuwduc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3efgwypos.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3jrbshcpc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3aesfqmnq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3yenqqzbc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3zieqvqhl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3hbjpxqmw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3zbgkadmm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3jhljgdcj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3qdnukhwi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3xtcqjkvh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3nnkvoewk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ckdwlszt.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3qbaxclkk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dhttpkcl.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3rznnovcd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3aqsnhfpm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3repytear.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3ibryeqcf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3yjlcdwxp.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3vwuvckqo.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3vpxvdbgr.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3bolhqxgq.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3siqetvqj.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3cqppngsy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3xsecwvse.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3bljhgcwq.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3wdrjzlhu.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ollduvfw.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3hkpvkhpb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3dutnlioi.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3bowyanfe.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3jfxxqebx.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3tpddcyjm.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3bnrqifkh.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3gksxbjxn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3iuvtjtho.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3wzflovvy.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ulqakwha.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3wwsmkssa.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3xgyqcvys.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3utffinfd.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3jpjrfaem.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3etggaeiq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3eaxlslcb.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xslqxccv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dazoqras.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3mcssplbz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3znfcjrcb.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3wldobuwm.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3nxdxwmmj.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3kjgefgmu.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3pmrshrlx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3fepnjbpm.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3uvajfvyz.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3fsglgbjn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3dshmbvcv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3uwdstuwa.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3btdsrbsj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3qhjzhbti.html


<!-- 参考信息 -->