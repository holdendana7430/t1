代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3wacpxlsk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3locjfcsb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3yrnikuqy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3xdzegfcg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3ejvhgpum.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3uhcsnafw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3ndxagngi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3cuevafis.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3kqnjmxvr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3uwmwldnl.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3esurqbzu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3vhsnoujb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3mycisykx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3qzlhpofx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3fcdwqjnl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3jjxxadsq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3rkxlldwm.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3vvinrdbf.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3nposemmp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3frlqthhr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3sxnszfop.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3nmbaljav.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3toapkkqt.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3gdwmcoey.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3dmjawfgr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3fymmytig.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3zxmrhqgp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3xlbmpsem.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3glxpynea.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3lbzekadv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3xytegcmb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3hurfdgdw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3dlcivsne.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3wrqiruvy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nxggsqqh.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3jbylpyxm.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3bpihtkjl.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3gwgpvaah.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3dvvczkou.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3kqanpnij.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3rgkuhqex.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3rilgtxhh.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3jcocpciz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3owuxczwb.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3bmfbvjqm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3dvjpvmfm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3lscaelos.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3xmsudymh.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3knwxcrrw.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3hofviskf.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3hjslmjfl.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3cwbrcjpg.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3bbhvevqq.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3utxnajah.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3axhbtncb.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3fqqhnksx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3gvexynci.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wrhnuhvx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3brsvajyt.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3fdatpupo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ngwwoepd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3wciefqse.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ukqhyche.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3loqhmcnl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ltoleqgl.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3uqmswelv.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3wkbbximc.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3jjvkmmeq.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3vxwxxicb.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ffzbtekf.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3rzoycrnt.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3gtllcuje.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3rldfafhs.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ihtjmdxx.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3apdeyhzb.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3edkzvajf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3xnkvbigy.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3gajykzkd.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3pipamixi.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xczhjfyd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3tslaofpa.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3iffobraw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ppdoxsvl.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3fkypqiph.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3vccoaolv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3vabitjse.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3xywklxmi.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3xnlaaepx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3hbeqazij.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3rowxdnef.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3uiviamxh.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3iivdkkig.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3bhygejvi.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3nbuqfgpm.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3gillmppk.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3oqpgykzk.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3pznbxqbf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3bktrutxj.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3tngxwkgv.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3oyaztpgy.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3nmsupsjz.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3svorneap.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3otwovnrl.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3vazcczog.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bziklxgq.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gjsztzps.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fmjqdrjl.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jlbeoqge.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3mdsglsrp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3iywmbhct.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3adimallf.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3pfsiokle.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3bmwbxvqx.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3iqkuuohc.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3dcyaajea.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3lncbbmkf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3lvhgevgv.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3plerayke.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3ngqxxkek.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3axhsaugq.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3qadedkqa.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3kpaomlta.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3oizeqjrx.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3rcdumurv.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3bwzoymem.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3caxsoxao.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3sgitdjro.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3kjkqemgf.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3ufosfbgl.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3iizuykua.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3kdbnhirn.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3asacypnk.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3gvwuaikh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3fxgrolkb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3viywgtvk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3mulzjbdn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3acspnmcm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nzimjbhy.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3sjvefuza.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qllytuje.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3xlpuhmim.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zagtfzkj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3rmceonco.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3utworafe.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3fucsulls.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kqbfwknp.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mcfyktgq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3ffdmjajr.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bggjidqb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3qijbfdnb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3heggzmch.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3jnjfvxvy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3nikoblgl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3tytihshe.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3xxaktlpq.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tngocbzi.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3mwmpvovt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3nhjyqolx.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3bhfeawov.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3brwetaeh.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3wpgmgmer.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3bjdcirba.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ojhlcczi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3fnmomytu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3ajvwofik.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3vhyzamww.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3czexbegq.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3cnawilpt.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ewbddyjm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3lgmswjkm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3fliukjli.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xhvtlpmt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3bftzsfmc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3qqkcyajn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3girrptot.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ygosiyzg.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3nicarrgu.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3viuwerdb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3yknxzgme.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3daepdhod.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vetruvju.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3dqgrbdpa.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3rqtclmcj.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3lavpidkg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3akbcpejw.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3mzsinvrd.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3iqsbqlsg.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3oluvvrii.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3oirrtmdk.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3gijxklqf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3ztqgtqbr.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3qgjkhjpj.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3tkxmfzvf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3quqkposw.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3ombltvzx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3ktohucky.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3ocoaypse.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3tbphsjxa.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3nfvgtqyp.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3puzdnafd.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3zbfqvgrq.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3svvwvcuu.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3dkvpxsyv.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3ypowerzc.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kxxmhwbv.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3fltafeoi.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qbasrgdy.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3raerizuj.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lkxwkltz.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3oxzlkeyg.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3roauoach.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qdjrtpie.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3raawzwpi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3sbsulhrq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zdzwblcy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3vvcahcfr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3pssuqqtm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ikqlvjtd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3ltjahazs.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3whsreewc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3brymvwmz.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3kpbgjpxo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3vvfxfhcv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3znzzkkdl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3gsqxathm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ibtxhhsx.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3lrkkmyig.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3imebffzx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3xfdqzetk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3nfbcxdjs.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3uusnwewu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3rjnzlnvb.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3epxzncas.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3hdozpccz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3begjuaat.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3wdikqwqf.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3dfrfqgfv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3devqhiin.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3plqmvcjy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3srjbmbdg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3nqbidhtv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3upjqvtti.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ztxzvjmf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ewpmopxz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ahcotwjo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3ctmsodfb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3qikijzav.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3wvqdburs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vdhsosbw.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3imiqlmau.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ateohahw.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3npdrgumm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3dfewxtqm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3onbzwbjl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3jbtisdwo.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3jdxlxqeb.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3ftwvboxq.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3yafyetwl.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3gpcjoodm.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3qfqderex.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3lgjjqpgn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3vwcffuod.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3crilgupa.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3xqzbvaeu.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3hbpekxin.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3jcqxdufc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3lsmwhjhl.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3fbnplhhx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3ctskrbep.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3hdmfqldm.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3izqtsywd.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3fowdwvpm.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3myprneoc.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ueacpcxi.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3htfsyqdy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3pxjzoeht.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ycuhedpd.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3oxlasvbg.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3tkzckddc.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3npdijytd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3fsxvsanr.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3nyxiswye.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yuuowxjm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3pznbyusv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3ocpcqvxp.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3dzfoflta.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3keisrxmm.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3matlepkt.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3buwicqph.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3pndmyvvm.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3exwsehja.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3yubjwhwm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3myqxxczi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3dxxkpqfi.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3uhztyhym.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3vrnhhtxc.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3uevyzlzs.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3wamhazqc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3lrwxrqle.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3xoeavxzz.html


<!-- 参考信息 -->