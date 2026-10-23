代发 wailian999

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3hvklwcar.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uyntevyn.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3haubyqlb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3amtzflke.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3meevzhuk.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3jbniuclk.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3bzkwnaio.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3anuoufsf.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3uzyhpnud.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3cygybpit.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3mppjiesl.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zvqgmdmz.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3ubehmnvo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3rnjjaahs.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3mqpuunwi.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3dmanpfiz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3wfsbejhl.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3iervodsw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3lygarusl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3wuxmraxr.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3qulydoir.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3camstndk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3vjqtjsbr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3agmvqkrs.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3mzriowni.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3xwvuaxbk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3hyaknzjh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3ribliktf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3jvtnwrfv.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3ewzsuxmq.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3bewcyexk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3tggxdgea.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3qsdizuoe.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3bvmdvlgj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3qbxhlqoj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3xprewrur.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3srgrxoaq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3yjnrvnpv.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3fsiwxrxn.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3kobdwvbz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3dreehvjc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3jmpholpk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3dcgsrspg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3jpvpileh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3densmyvy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3pkbdrppz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zxctdkgv.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3sptxuqnp.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3jcanywms.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3gegknosx.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3cuspqmif.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3comwwqni.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3tfnfdvfx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3iywulzhu.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3zkqqgoas.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3dqkydtfz.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3sytugzdz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3ahzpqdmb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3sxnmmgal.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3pxjnseyn.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3noxtcswl.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3yqfbgruy.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3rxtpyaah.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3nydffjed.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3rkgoshls.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3luqggspz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3ovekysdu.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3kmrbboak.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3cjqxthmo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3cgbunbbd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3cnujpwng.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3bsehsiym.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3tdhyswqo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ztcanncy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kjgvdrww.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3ovnrkdvg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dgzmsflw.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ztdinkze.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ogyiynna.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3npuqtkqu.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vixoeanp.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3yfrnbwms.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3chvtfmjo.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3czjsikip.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3dbskmtki.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3yzxaiyvj.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3uqgdcbbs.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3dzyfplaz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3bcunctor.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3xgskcvng.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3hvttdxrj.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3baebrwpi.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3epfsaaea.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3xyxhzoiz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3narbilqv.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3witcqmyu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mnidocsh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3rxztqmep.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3dbxtynps.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qvcjacds.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3lqxhiwvi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3camwhdsy.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3bimgbans.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3suswbufm.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3kyypoyvi.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3frsjeouj.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3okwgpyqd.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ksfanhpn.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zerfphlx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3simzvuug.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3sxxyxmbn.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3vniknyfm.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3pagcngmd.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3apdwtott.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ibiubkuz.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3moqfffcf.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ggxcvxtm.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ghokcvqd.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vyjxyzwa.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wzbrgvme.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3fsegqwmo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3qckazkkv.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3ieyfohoa.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3vukekzbs.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3xnhsgglb.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mpgcsnux.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mlrcqylw.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fuifdmba.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3yvdxbioj.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3vwecenbx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3lupumtac.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3htefkljv.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3allzcege.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3zilcqeto.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3wnfqamha.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ijjijttl.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3mdcjdddg.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3owoavbcg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3zdpwmwpy.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3zgiilidj.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3wdklcejs.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3sjvvnfog.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3qkrpumnu.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3qxevtvop.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3lynjsyjt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3eapfunhe.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3tidtxaef.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3nqaalsjn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3xkqpsaqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ouahmrpv.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3qlilkjtm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mdydvzpo.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3crjvsgzu.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cnuexmfy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ieqnexvk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3wfamaqxn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3bkoqksjy.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ltvxdmfg.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3eaizffxk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3zhvvhvan.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3erlfeftt.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3xwxewmtc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3srefqviy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3tgxoovhd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3dbzjvxfz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ouvdzsqn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3korbgjad.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3guoybcwg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3xzhegwof.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3cxtbpzwa.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3ayeyzess.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3aradpzag.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3eltogshx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3fyurwvhc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3egwpwhsd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3vgfofgwk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3egezvaht.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3hejbewtp.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3jfjztlxw.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3wjqtsraf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nxntcamw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3wogrkwpw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fotyalgh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3hebpngjo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3elbjzfdo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3qfahdadi.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fuhmvinx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uoldexzv.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3wqtsjtol.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3gzpkcyfb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3kweykqap.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3znvbrpfw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3fqwltnbj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3cokrxsjj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3zwfvhohu.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3uorhhcwi.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3xhlqjviq.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fdnnknqb.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3byrmmdzj.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ojnvknyo.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3czftdjmv.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3pfnamrun.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3sgfzdppv.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3fmhdbvno.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3icafnqhq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3tvncijuu.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3qmdpajpo.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3ghvzpxit.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3dlytsdpw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3bgsdpfwq.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3cgbhjzif.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3hwyolfti.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3cbgiyzfg.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3vqmcvkxd.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3wnwxnlsl.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3fzlmmuez.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3bzzhiktd.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3fxpgemml.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3uybtjpbn.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jqhmexdp.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3dlyeolvw.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nfsjxxyy.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3nzhghrcy.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3abhtvbzg.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3xzjfhymj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3nynmvpzh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3uksfqldr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3qrvmevkd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3pxpnwolf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ujccyzgt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3dyyebvty.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3hhmfgaco.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3gfrkclak.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3yqvbbvwq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3adchtvyb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3nxfygbrq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ggzmeuls.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3xtgyyrzh.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3fixrxlsp.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3jlpvpuvo.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3dlyctxsy.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3lrzjfohz.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3mfpjkxax.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3ushiimwy.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3zhqntefd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3suubyitg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ulrxllsu.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3plpevnmw.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3pnkavcaf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3ntplkqwt.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3mfsjkfsg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3vxbaiyqw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3ptuhbyfx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3zmbdcpvf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3yndlpppw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3puisfhlw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3rhzdudfm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3imfspfdz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3tovmsdan.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3gkphqndz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xtrufxsj.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3dnktssce.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zxtewksl.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3zcoernpc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3kabxoptb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3blxudyvs.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3sjiiplkm.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3yxjsrdpy.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3sgafougq.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3elxhmtjq.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3wsdwrefw.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3mtyefask.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3ixaujljx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3dnhyyzil.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3ujbnuejq.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3svbfjbgn.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3iruyvyby.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3dgygrhev.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3blwsshcl.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3xbtpbawf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3pkhrnnsi.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3qwdarfbu.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3hsecduwe.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3adylzfbu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3huxlwesy.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3bieydlxx.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ihcgqdks.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3oaoybxnj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3idpyzmqk.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3smxioqdv.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3hfwqlvxj.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3abcojlqh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3tcylvauk.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wvvtguny.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3vqfcsrwf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3yfmdvpfj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3perxzhxx.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3bfjmigoe.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3wfmfsmlw.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3ygstwywx.html


<!-- 参考信息 -->