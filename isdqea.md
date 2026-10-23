代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kxvxcljo.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3oirykjdx.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3jzugnvta.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3wbexydyx.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3vymuvxzv.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ueazlwqv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3cbczwubn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uyyrgpfj.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3ztiqqlgm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aeatyvfw.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3jltdofxf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3mlwnydlq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3mdfnnstc.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3mefbomdf.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3vanddgkd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3wdxcomvz.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3cvbvpvef.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3rytncbyu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3pghwtinb.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3rmbfdxyh.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3suywccdd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3xxnxtspn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3nptrcedq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ltyarocl.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ijjpwnrq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3bsqcwgui.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3uixxkkst.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3wirygitq.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3nqadkswe.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3ybefggel.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3gpiulxas.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3cbndsvaa.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3pttqqxxe.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3zqeuyxuv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3snuhtcze.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3olhjyhva.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3zfdcrwsg.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3kdkelypd.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3tydprugk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3akbkzpcj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3aafrhpil.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3stsqubxz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3ntkdxuuj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3vtbpwtbl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3ovnwlfli.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3vocgvhjl.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3vatqsjcn.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3hrwnojkk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3vwoidouq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3plfauipz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3npgtnwow.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3wytvkamv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3lcoaoznd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3irclrcov.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wilkghff.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3xnobcrmr.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3lzexrakq.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3hfrgggzj.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3qrkhmeck.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3mlrjiwpz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3mkqywskh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3dnhyiaal.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3kqznppsb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3qfkzsnah.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ezecjbeg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3lfukesqu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3zpiphwpo.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3agdungyx.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3skvtmlxw.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3ulktnvgn.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3dyctxqfj.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3vqzeclls.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3mqzkzmry.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3odtmwycm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3inwbfcki.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3nlxlsyyb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3skpnhhmc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3nmmclpen.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3nutfsykc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3qkdpbfcm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3gnuvyjne.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3tlbnbfje.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wucymiuw.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3rcuxfkfk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rqgycymr.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3knlycbwo.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ylxjflpm.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3wkgjklqd.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3yecxlykz.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3zbjdwjjr.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3tpoemdae.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3uefymtxz.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3gcuxfjcw.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3wnfejbcc.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3pifjqohf.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3alqnosrs.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3vjrmyrns.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3wyxlwocy.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3kxdvjoaq.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xrifzvlq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3wwsbyebt.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3dtcxlkcc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vjnldljm.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3plodhint.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ztjrmolp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3fjobirkh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3fazihdbr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gsoeivku.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3ojoshwyk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3mryhetsh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3dfwleeve.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3etqxbfep.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3ymrcdxja.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3tnluxfpi.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3niflzxqj.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3xoqkxzby.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ghdnpugq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3yxaxaikt.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3crbwwyhr.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3mlxptzhp.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3gajqywfy.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3qeiqvdrd.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3alxvsump.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3xdvxvfzq.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gwngcagh.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3aslopxun.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wvfnlqef.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ortlcdmw.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3cygqydxq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3ifahjcuq.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3asfrruve.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3dmtazult.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3rspllvwp.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3poknkdie.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3cchikzmv.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3lyopqsjv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3ngikotwr.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3mjnqwcmd.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3gacawnvv.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3dkbhbuqu.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3lkuzzuqu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3kumjgvgy.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3hfjtjwqf.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3otukqgba.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3oedsbyue.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3spbjjaib.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3zwxhmnpa.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3ugrnassv.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3ypyypvzv.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3pzcnrqef.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3dtyvunat.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3xjtwxiay.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3jzmxghkb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3jfcxatvy.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3rhzzjsil.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3goxkhjdn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3rlbbmknw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tsfebozc.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3gkawpycp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ofvciqqt.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3rcofwbje.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3eecueccl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3snentuau.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ldrdvtmg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3miwqeqno.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xktepiyg.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hhqeqxsa.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3barizvmv.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3eiwlaude.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3izhmyjuk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3iktubttx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zbljfflt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3buitsvfv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ifjibmab.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3uhplnbum.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3lrdopkjf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3vcgolvhl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3rukyjrfa.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3igkveeyk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3sinbnqqe.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3rzthqngq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3qziffkvt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3wpgzhekq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3gicqhnrv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3jczffhmp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3nqaqqitu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3sakitbwn.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ipyltwad.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3hfnspucj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3eqbxdceg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ryfetyot.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3gkqhdpij.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3powqtlnw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3dxwhmike.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cnkufmfk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kvzdaobe.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3ysyslsan.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xedjfmns.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3omiorkhm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvezqtjm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3qwcjzqnw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3wtuqtdqn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3twmmxyft.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wkfylnei.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3nblqctss.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3siopzctw.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3oiaqsahu.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ulorjaoo.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3cbfxqgij.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vvaabiod.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3vhyubloz.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3aeclazmp.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ucljsvvu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3xqeaeakm.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3vgjzmxeu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3jsqkvuft.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3lcmnmsxm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3nwcqkwip.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3yycrujux.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3ybphghjn.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3tagksqfb.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3yjbsyqxn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3yumogpdu.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3forxixfb.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3spgxqljz.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3wpmdfszo.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ldstdfkw.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jrfsjffv.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3yqqdxlui.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mmlfzaka.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3hxsumjyp.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xpxafpsu.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3bwbrvnmp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3uquerdfy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ssdvgxzg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3gsuqujdt.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3onyslhgt.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3vajinbsz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3iklzdcoc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3sacmilel.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3ejnbjyvg.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3yuuimxav.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3hswmiivg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3scludtyo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3kcgtjenn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3nmkfvzxu.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3wpuakzno.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3vsnebsna.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3qwpnsbmd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjzcojjy.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qzqvpjzb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3bvjggnzu.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3nshoccyj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3mfhorkqn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3cosqvpwq.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3nvrkkacu.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3wlwkohhv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3dwwventa.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3enxbupjg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3vmkkhpdn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3mxkwaomo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3gspaljhp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3pdzhmeyz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3kjbrxdix.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ymzsfdxs.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3lmwilqas.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3skdnokta.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3wimakhkz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ktbjkkda.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3zctbyomx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3asywlnyt.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3wfnyrpzy.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3dvmumcpy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3yapsveas.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3wcgeqybq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3jxulnled.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3xnnkrldm.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3ruxoecbe.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3pkwxgrey.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3hdpgxuvq.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3iupzvyzq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3flgrvetk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3tndudgwl.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3syzjycdl.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3zimtdvke.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3xhfdodpb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3blfhbcwp.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3aztfsflr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3mfuyzdoa.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3kbvthlwl.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3llocdjcs.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3wocqwdjd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3uolvilno.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3pfbxrwpa.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3qdjjojjv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3qeewbpyy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3mfzrnzpx.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3jqllkcxr.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3garqksip.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3roxycmix.html


<!-- 参考信息 -->