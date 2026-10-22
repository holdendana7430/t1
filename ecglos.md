代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2xbziqyez.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2jdtgbmqc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2jtojwolf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2etlccgqq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2mjvmrpva.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2qlzhsaeh.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2xfidmlae.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2vylokijr.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2utbsyoal.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2rvjbrdrn.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jzaynhas.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2mouprhvz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2hxqudzob.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2xwohyqhn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2pzvjeeju.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2zgjshxak.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2xfsucoky.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2uzdzhrfe.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2jvpcqsvy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2vyytkfmr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2imldaasu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2jxgyyjxa.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2vkwuoqao.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2hftupusx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2luorsnuh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2zsinmkxx.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2mliajdjd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2hrkqgetm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2kdinnzcm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2yhmbyvdl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2tcuwzrqb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2rvkwitva.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2rejbijef.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2eihnwjgo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ejbbfrut.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2oyadyhcv.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2belynexr.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2zgihpmpw.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2othbalbp.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2nehotvug.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2dolaqfpq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2derfanuu.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2roifeomg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2ewgzhguw.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2anxgpcbb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2mkqjrfjd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2ihxqjqqo.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2drzgzhgm.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2akjsilxq.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2loiaodxf.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2tcyvbpof.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2gewzienw.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2uxluvltu.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2vkmotcra.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2uncwhfdk.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2oglpyuyn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qpjxnrzj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2punazdbj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2hjsrixbn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2wujhgfpb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2erhwsvav.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2oclxgwan.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nncwhrvu.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2rcnmpcgp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tgeozsxx.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2swdeaikn.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2xjrjwmox.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2ktgmmaja.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2xxeneiwv.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2eubcfxzy.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2bibmgizn.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2khbknitx.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2xtutwwuf.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2bkkixazn.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ugsijovv.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2fgvtnunr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2nmuahovt.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2fxbhwcos.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ylxvlzxv.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2thbgcnug.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lsdqddkv.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2stzthyef.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2flfzsxme.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2kehhkwxc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2hxipprei.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2bgvoahtp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2eifbbqtq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2tszncqbp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2mffjhdwz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2yyfyruum.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2zguhuzdy.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ekyrvlfy.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2fhoinzdn.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wsjllbme.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2extqhwjq.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2inxyiikj.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qjhlucru.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2xxomeqfc.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ufpwusdi.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2wultrtnw.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2kldzrieq.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2haktlqgv.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mjhoyjpc.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2vsxutday.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yhygyxma.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2graggzxi.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wbtsiweu.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2obkxoxvr.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2vmplmatq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2zrgmcrna.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2zvzblwpa.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2lhnlmmrh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2eoeapuwc.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jslyzpvq.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ttfilnlk.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2kyouowck.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2buknmwtt.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2wzuctzco.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2iswbsado.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2fyaupakv.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2ywglxawa.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2mdtvtmjd.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2bijywqrs.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2fqgmngds.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ckroikut.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2xqwopolx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2dyswlwzr.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2xsrkmsje.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2kgcrfpoe.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2cvdwnkof.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2dxhkjmhj.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2hzaegzvs.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2bwvqyluf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2rjkpapxc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2cwzaoifl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2miaelhhi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2smmxtqgj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bzzwgtnc.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2lmfcqzty.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dntydciq.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2gaxpxwfq.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pgabbcyd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2rolsbpsu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2bscnzqgy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ttqkqybg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2slwzewff.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fuhosise.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2jrqnxosf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jnwevjrw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2gwgbpqtj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2wlpgwjia.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2ajgnydnv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2acluksbt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2wbfazzkf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2vwskvuca.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ndjzrswg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2qmtkrryt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ahrxupqu.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2czsxxpia.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2uhfxtaxw.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2wchuhyfa.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2cquolcbh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2vtinnbwm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2ufliafqu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2nidizkfn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2yysvauzm.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2tfouffdr.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2rlyxmekq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2wpznqzda.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2fjjuopkk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ipmosash.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2owepobim.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2dxgfroyw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2vvgdkbyi.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2emllusfx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gkluggud.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2glzsjrtk.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2eaihyeai.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2kwjsqzlu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qceclyhc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2bieqpywt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2jxxiscnj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2guclxwse.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wjwrbvby.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2vrhjiwfw.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2zqstfqkh.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2wvtjftik.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2movzrsdw.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2iwjwdebf.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vshcimwb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2dphcpowr.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2aecjqeak.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2aqejavng.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2uoirwlmf.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2shsphswd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2phijdnoj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2aqyeyenp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2lmgcbmlb.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2lqrhktjr.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2dkjiakln.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2ducilaam.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2jgrcwhgj.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2ggqcdxiq.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2zecnrlvz.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2cefhxxwl.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2rgecstmm.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rhimmeqv.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hkijtidb.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hidllmji.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ispoqcna.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2ptfiqaec.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ficfqotm.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2lqegyjuq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2gvsmucsc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xabdwnwk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vodlhhtw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2qpfjrrez.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2osnwegib.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2qsskhdaa.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2drmmlvhu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2zsvmfosw.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2xwhqafyc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2lyplblnz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2vwclktna.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qatyhurg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2jpyfztfg.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2tmjswuwp.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2ejmdqgui.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2wghjhpah.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2wagtdarv.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2baklizde.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2tpilkwue.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2pehkoemh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2spavkyvf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2jsyowsig.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2fbucophw.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2vuyeimyc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2kkqfrtcx.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2yiuplzda.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ljnixzka.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2akonmsib.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2hcosbhap.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2xzmgnfhj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2waeefgjt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2przjerdq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2eymbqbxq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2elkydkum.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2wbkrotvp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lzhtgidi.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2ocpsaprt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cuaddjvj.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2jsrqqyuh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2wpzbrwne.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2klndvkek.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2qclqxnhb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ymjxurrk.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2dmhsrvbh.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2osewlzgs.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2iezqafzu.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2olyyfjot.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2oaqoukva.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2ojqkusbe.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2cpvmtesu.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2msqqplrc.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ryeckoar.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2slyjzvhz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2pqtrrrxe.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2dvwfqcmo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2nqtuqnru.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2hcszkoks.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2xuzclibm.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2tgclaizd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2rthnclms.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2eifhsjju.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2xqvenrys.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2vblmuyzk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2bgycjraj.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2mbpivbxx.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2fwgkyigr.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2vbqwgngd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2wvvmlelb.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2eypmnirb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ycacukbc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2gaoqdwbk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2ngvmwfib.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2tnfxoefv.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2jcdpqwbl.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2bchncnci.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2rstvpsco.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2rigrnqjy.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2gkkhiuvy.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2wtxeykau.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2qnlvrqew.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2uhntwvpu.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2zxcrqbrq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2jyopzwqv.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2ynifolzx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2ahbugskz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2iajosxsn.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2exdiomeg.html


<!-- 参考信息 -->