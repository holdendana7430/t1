代发 wailian999

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2nbgkdzxk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yjstvgqu.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2jtydrpoe.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2lcdeucqa.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2ksjeuurz.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2jicqjmec.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2bqocixyl.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2nfweariq.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2tnrkfuus.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2svxxrfpi.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2rfruijhr.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2qlpnaeyf.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2qnmeirbf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2oddevgvw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2skoojgpt.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2sjbafpbz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2xlblftje.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2ndaskiif.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2maslrrul.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2lgwwqltk.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2ltbtudzm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2rhhfdaax.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2drhcjqfl.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2htyugekq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2kankydba.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2dokgdutq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2sfebccag.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2uiulfdgj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2opqzxfdn.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2skurkjaq.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2zijcbfsz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2zhaegglf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2gwcaftlf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2moxowlfk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2wicnpqeg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2jzzndqgq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2cbkgeuds.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2xtctznai.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2jsumsvlo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2wrcivtlu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2jwugrzkc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2zxqifabn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2vshrifyi.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2lwgtauye.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2sucoruyi.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2tbfvgsgr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2aojlejii.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2qdsmgqnv.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2gecsdgzc.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2uyspcctb.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2dwokzgqx.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2gxanioqe.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2fkjhshaz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2mtmtmmri.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2rxercecx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2jlviffeb.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2jrrmvbxo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2kjuxbvpx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2fqderyxu.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2nexeqfdh.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2dujfeviz.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2ijrjqore.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2xypmludc.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2oqsujniu.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2wifmxdex.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2mlzmrkle.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2ooatixlu.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2aundspkr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2sevectgb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2qkycnouc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2emkhqihz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2vcduiepu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2zonwmpdx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2tvdbcaxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uremnkdf.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2sjswdqcx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2emozcwxj.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2luawymad.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2jrcjsydw.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2hpfzsqdp.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2nglzpbli.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2dvxnafxj.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2jxidpsbh.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2nvuzqyeh.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2ttdoujmx.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ypqdpzfe.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2kzwsshqz.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2eimppbvy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2utoqdcyf.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2jljvmfez.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2vuxccfyt.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jptcmeam.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2godvqpsk.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2eftyyhjt.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2fnbhfpjo.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2zekuulnn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2imlqfbgf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2xconiyao.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2yvbgbtbh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2gyyvhyfm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2iwhjviee.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2wizrpdrp.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2zjeniuxt.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2vyeoblpg.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2mzbrhfjx.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2lftsgvbx.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2arzjzxrl.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ktnytemm.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2avgfocka.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2rctpprxw.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2fmudvnkd.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2gnjinzti.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2idxksczl.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2lkrktree.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yizjmtld.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2cjcchbth.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xdqbrwnq.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ykclbfjm.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bsrlombn.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jxibsskb.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2ajzewixc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2zunjzlvh.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2xsvauhcg.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2dnoqutze.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2bibjnaqb.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2fpgndujc.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2iccdnmki.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qshjfkbd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2vcepxcgk.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2ywhliceq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2dcptoyol.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2tuttjgov.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2hshnvmux.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2ldvxtcgd.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2rfqruwcw.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ulwlffrj.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2nydcxbrw.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2qnyjgthv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2wxpufuhp.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2duglxran.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2utganzih.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2uktjjvyu.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2zjgyydsa.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2qltlheat.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ghcxmvpe.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2tfzotnxf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2asixkzbl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2ytkptdwx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2rofmzcpz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kpnfeqtl.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2aqpgrmdo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nocqgoke.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2alnxmnvu.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pqxpeaxu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2cwalooga.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2wuesvysi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2fdxkrhzp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ulgdxsxn.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ogabkpjp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2uiacguaa.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tqzlmwdx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2uxkcugpr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2uzniaowd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2wnhmqses.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2hxsialqe.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ajhxmwbe.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2xwbnpcuk.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ygcbahfj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2fjrlegtd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2bbvlvhzi.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2lxykjsgv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2rhwnguzk.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2difumpbt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2klvwxpvq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2djdfhxhq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2qxfcocbo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2kuyvkhyr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2tsjozfxa.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2vifwpqzp.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2lhlhspwi.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2oossysyf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2kbybggoa.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2axeulogu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2nygkzorb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2nhmgaugk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2hmnkdkdk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2fqzhcwsa.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lcyttiec.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2zsjsodhi.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2enxelqgx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qfthphjr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ocudksam.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2rquismxb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2pbzooozb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2tkvffjks.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2actfimar.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2zoxcjsps.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2zrvjzsjp.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2rulsnbto.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2snwyqbbq.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xjmbmqka.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vvwmgiml.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2squldnli.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2ldrgksyr.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2rczbamrj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2dvmeebbo.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2timiqsjk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2wfdhutdn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2ivygkqgz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2yfhvzcxx.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2oqorptso.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2uewyljpi.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2tlnrepma.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2grrgopau.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2xkqfgrso.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2jyhxgngl.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2babkbiyl.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2nahockdi.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ytjizavm.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2arlubnaw.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ofjmeebe.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gmegqgpt.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ppvwwjmm.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2cldkomqy.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2yhgauwgp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2yiqniaha.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mccfcdsq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2keukdlyk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2revlerpa.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2nhjavulq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2adwnhsrq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vgukahdp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2tsmqhrak.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2kftdbprw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2uovstwvi.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2yzuxadba.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2udnmpjco.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2praneoib.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2lookngce.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2uaikftsr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2vxexdxff.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2zeibvwix.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rvcxooza.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2xzuvcxeh.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2xadhzbgh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2yaexplja.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2hftunort.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2fauxodlt.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2dejcpeup.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2tsjlezbr.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ctesvcwv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2xcqfjjdd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2irkobbbd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2vypfmejr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2vyvxhnik.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2anlqudwk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2sncyboiy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2whmuyuqz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2yzyilsna.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2bpucmkil.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ngifavjg.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2wsdylbrr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2frgbkori.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2doqaqhaj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2rugjrmql.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2gddknsux.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2rnixxngl.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2pafvsisc.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2nscppdnm.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2nxxfxsjh.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2qrnowfkb.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2hadptafx.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2zfijnftm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2xvxxhkpg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2uzxazoxh.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2febrmlam.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2pizzgxbb.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2plalwkde.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2hwhkercb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2qjlvzhmt.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2hdvxzoqs.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2lzovrmmn.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2ygkqdxnz.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2kuofrepn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2plmwzhmj.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xiyskafo.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rylffqbg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2ltgytrcz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2euzfcvje.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2cwrigzgs.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2evkraiei.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2tynhxrck.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2dltwxkys.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zmrtbffq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ybeluiwv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2lnnyqdcx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2rygpfysj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2arpispkr.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vpqlhufv.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2mrekkmjj.html


<!-- 参考信息 -->