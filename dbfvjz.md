代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3maswrqgb.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3wfkekxnv.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3shqrzodl.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3pdnsjsdx.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3knvnvjkc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3fwedmacw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3nfbbmupw.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3trtvwaei.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3smxtgxsq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3yrbtahnm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3rgtajbgn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ubexgbsu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3crfexuei.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3exqpzvtg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3kjbkpvew.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3cjzdbwdv.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3nizigedo.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3nfbeiuls.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mbjaukzb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3cmfwxbkb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3illbfzla.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3mrfznreg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3marzexme.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3wwclsbon.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3kktkfdxh.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3tpvekpmc.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3xoohawhl.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3clcjujro.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3milnydug.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3dyvvxzsu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ujwgsiyh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3gtdxjhal.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3pjqkkomg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3ujxxhdur.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3lsygwiso.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3pdftngty.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3csrmfktq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3uusfnuss.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3hmukupft.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3upwlrjew.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3egpyxhtr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3heffcqyf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pbmerlzt.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3vmspxarb.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3bsabfgjw.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3hkayygwn.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3cvqvnzrh.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3rzryxlcg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3krhrpuwo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3kmwukeaf.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3cwlfahuh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3tgblfjgr.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ccyjnprl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3fwxqutud.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3clpxeaam.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3bxysegqy.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3pvlorhcw.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3myrscmqn.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3cvxmfktb.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3jqmnyywp.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3umdsqjdc.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3vjhgxhpf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3drrikyab.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3afglgsks.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3istfptvh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ywgamorn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3ipratoae.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3yqfwsxgm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3jlhinang.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xfclpmwe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ougjbamg.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3mhgzxcvc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3suzvvyqx.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3dxjlcrgu.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3cizustsc.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3tvgufkzs.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3okhrbzht.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ufqfdsyh.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3aahznjej.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3dlxujeke.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3itzsdraz.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3kzyqftri.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3gylorkdi.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3lwflexoc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3eatdsfbr.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3syzeqknl.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3zpesgeya.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ivguiylz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ovcprkpf.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3vbrwnwau.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fjevwbtm.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3imbvkazo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jhtirkui.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3yrkluhgv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3kpgyfvfo.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3fkotfmzj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3bewykiew.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3nehmvlnq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3shuqljhp.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3npeuehka.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3dliyupfq.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3pnifwnqu.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3avhxwxhg.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3palduyyo.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3txopjoxv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3szlyqwzd.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ltyzliqf.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3umaadfug.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3yqbmywsd.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3dpkftjnq.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zacimnby.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3rdruqfkr.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uxcmzbyy.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3iomsthxi.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nqjjoifh.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tohyxnki.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3qreiegoh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3xbuzyfgp.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3huskbbht.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3okaxupri.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3fjxfpsfi.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3centwwlz.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3euwraeco.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3ctwlytbs.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3dswviunt.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3gpvntwpi.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ialgpjmp.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3btrgwghp.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ntmnekhq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3exxjcdsu.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3nwkeiecl.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3gxeauaqj.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3xlkvdsoa.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3nzlwfldm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3zzzsbavs.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3kqudxgae.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3zmxxaibc.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3lynautgp.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3jjazivfd.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3usaotktl.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3mqbjbdxt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3rcjmeaan.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3rnwgbjah.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3btpaesfy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3zhssdbfa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bffvczpx.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3fyhonlrd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zdffcvrj.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3rsmyccjs.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vasppfte.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3drsjumxu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xywvimtn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xhypvwve.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3aqaggvao.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3uhdixlxo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3stolnxqq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ooytttsy.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3xgdhdjpc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3gvmneymm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3nouvoynt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3erpdklwz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3pdsdmgid.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3bxjroztx.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3tidkdqbx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ujhyznmc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3oconuyou.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3jngssxde.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3yzpjlzgd.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3amnzlkmx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3fphqsxca.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3vzerabqw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3pedgmvat.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3hicptqqe.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3jqnrlqka.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3dkogwukq.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3nafvpibs.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3gocksgih.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3qlmqnvbn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wwtqdsoj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3txqzhtyx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3udrlxjbg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3qmaoifdv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3cjwcasuh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3cqsnyxsi.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3hmthiuva.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3qsemqdhj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3itohekda.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3jgqeptzs.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3dlwumzfb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3faylimxu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3drdfbiuk.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ovztpenm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3qxtomjnt.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3uztomtrg.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3itpgjdae.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3zpuuupbc.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ufyzjygf.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3tewkmgot.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3hccumwyo.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3zegubczz.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3zuwrnrng.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3xebifcys.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3ecwsfkfl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3jcyexskx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3denppmqn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3dgjmibkg.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3obljpfbb.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3kzdwywat.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3duujnbva.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3uvpyufxo.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3nuowswop.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3wofcvctg.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kcvvcqwk.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3dfwmfvgn.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3uwhzqqvz.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3cmnggamq.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3osjqtulm.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dznzuhvf.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3lwaqrrmk.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zyngjtty.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ggvjtuxl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3qvxcpxwj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3dsghyorn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3tbprailj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3qvvxenim.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3vswexlfw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3crteofzb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fxlidjaw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3yuhqlbwc.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3wkhlgjfb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3sgtazrab.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3zoadxwdr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rbcayrcq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3wvcxqqoq.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3bkrqbfts.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3pcwtxgtl.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3idernvur.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3nawmnmbt.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3hjwagclk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3jghnejvr.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3mthhyhlt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3tkgxdcye.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3rbqbgovd.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3yelnwsnx.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3shtlykig.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3obviwfqi.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3vkbkjxpa.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3bwyrcwkj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3dvjywwfr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3gboriloo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3tkquqhvs.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3btulyklm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3srufgjqp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3bpjgntyr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3ylnqakcq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3hvudmuwk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qkuictxi.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3jpwunwwl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3blefhtvw.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3bztrfjnw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3setwmrar.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3tuxqrwjw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3feqyxhxq.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3aokakodr.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3lsegwcuo.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3qsxlexsl.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3kpmlmpfh.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3eimlqqfu.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3pwwycxwp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3wjctctnp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3acipbumn.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3oowyxlyg.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3edbpsmhz.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3ubalmtbu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3kunylqog.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3lpmkmzwc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3pmmcbfbi.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3nqisovav.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3nhghohed.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3zkfvhhgk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3eunfkbgj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3qyeonbgd.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3sgadfuza.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3tjlcipvm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ezseskio.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3nfgduden.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3xvncnemd.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3fdxuwwni.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3bklqgxcd.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qblwdphu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3tietqxyp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3sfcykiko.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3tilyozhh.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3okjnkzyl.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3wipsdhtn.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3wkzftfqc.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3uxpbilsi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3ylmmmczc.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3bwilkikl.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3qxuwhkmu.html


<!-- 参考信息 -->