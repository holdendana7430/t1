代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.zdbjq.cn/Article/details/gncoepucc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/gicajzdeu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/gikddutnr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.hesvh.cn/Article/details/goxdnqyuw.sHtML

Go:   encoding/gob
来源：http://mobile.hesvh.cn/Article/details/gnphygxio.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.zdbjq.cn/Article/details/gticrdqwb.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gtwihhfls.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/groumtkeu.sHtML

L. 网络请求
来源：http://mobile.fehbvm.com/Article/details/gxofmxmkq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxbnuhcto.sHtML

[L01] 发送 GET 请求
来源：http://3g.fehbvm.com/Article/details/ggpzupnbz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.fehbvm.com/Article/details/gejhrwech.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.zdbjq.cn/Article/details/gvtaeuagc.sHtML

JS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/glyupgvva.sHtML

TS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/gyqmgpvgq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.zdbjq.cn/Article/details/gzgfaagzi.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.zdbjq.cn/Article/details/gyopwooqi.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.fehbvm.com/Article/details/gkdjhzbdh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.fehbvm.com/Article/details/gbhksicnv.sHtML

[L02] 发送 POST JSON
来源：http://baike.zdbjq.cn/Article/details/glgvjmpvf.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gfztvuphf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.zdbjq.cn/Article/details/gyzygdpwm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/gisfejwqk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/gbjdciqde.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gvdaqcxye.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.zdbjq.cn/Article/details/gmoqujmhc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.fehbvm.com/Article/details/gtokfiuwj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.zdbjq.cn/Article/details/ggtpnnocs.sHtML

[L03] 设置自定义请求头
来源：http://read.share.zdbjq.cn/Article/details/grdykemrf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.zdbjq.cn/Article/details/ggbrjmfuv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.zdbjq.cn/Article/details/gtlyjfujb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/grdgzxnox.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gddhauhvw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.zdbjq.cn/Article/details/gkxryhsdx.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/grfnybpus.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.fehbvm.com/Article/details/guvnzhznr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/geaurzboc.sHtML

[L04] 设置超时
来源：http://wap.hesvh.cn/Article/details/gshshudln.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fehbvm.com/Article/details/gfhxpmfrs.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fehbvm.com/Article/details/gruuftpfd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gyqpeawfk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gudenvgdc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.zdbjq.cn/Article/details/gcuwfgrcf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.hesvh.cn/Article/details/geqcufqur.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.zdbjq.cn/Article/details/gvpnkrscy.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fehbvm.com/Article/details/gdfyczrik.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.zdbjq.cn/Article/details/gyjoivhjl.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.hesvh.cn/Article/details/gtffoqaue.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fehbvm.com/Article/details/gnjbshree.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gonqrbyim.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gkoelipiu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.hesvh.cn/Article/details/gootamavs.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.hesvh.cn/Article/details/gqnzgydxp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fehbvm.com/Article/details/gajseohfu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fehbvm.com/Article/details/gbgxtnymt.sHtML

[L06] 解析响应为 JSON
来源：http://blog.hesvh.cn/Article/details/gjehnhpmr.sHtML

Py:   resp.json()
来源：http://3g.zdbjq.cn/Article/details/gwentnojh.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fehbvm.com/Article/details/ggsyngbbb.sHtML

JS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gxjuluhkb.sHtML

TS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/geywgcwgh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gxqyespus.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.zdbjq.cn/Article/details/gyxvjbwke.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.hesvh.cn/Article/details/gfdhryrnu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fehbvm.com/Article/details/girdygxqf.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gzmkswrwj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.hesvh.cn/Article/details/gsoiqbujp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fehbvm.com/Article/details/gogomtjqj.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gpqkwtnpv.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gxhkcnmer.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fehbvm.com/Article/details/gtxenxrhw.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gakduvhjd.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fehbvm.com/Article/details/gpwsnfewb.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/grvjkzkjl.sHtML

[L08] 并发请求多个地址
来源：http://3g.hesvh.cn/Article/details/gerfojjjx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fehbvm.com/Article/details/gzyblnnyc.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fehbvm.com/Article/details/gkzlawmsn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gfluiugnq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gkuletigp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.hesvh.cn/Article/details/gtxakarmg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fehbvm.com/Article/details/gkxnzwgyj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.zdbjq.cn/Article/details/grrsykwqv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.hesvh.cn/Article/details/gzdsdfyeq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/guusseuat.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.zdbjq.cn/Article/details/gmomenend.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqsmgmhcu.sHtML

[M01] 读取命令行参数
来源：http://baike.zdbjq.cn/Article/details/gjgyuusus.sHtML

Py:   sys.argv[1:]
来源：http://read.share.zdbjq.cn/Article/details/gouidmrxl.sHtML

PHP:  $argv;  $argc;
来源：http://baike.zdbjq.cn/Article/details/gnjqtjhze.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gumftoqhy.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gvrehfxnz.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gmfthizfl.sHtML

Go:   os.Args[1:]
来源：http://3g.zdbjq.cn/Article/details/gsydqgqce.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/gctrjbcdi.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gjjmqrdeb.sHtML

[M02] 读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gndraqqhi.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gxzuwzzuw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gvldenhal.sHtML

JS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/glrfmxqvt.sHtML

TS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gqgyqwosb.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gatmgrowk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gktwgkuts.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/gzyiohsid.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.zdbjq.cn/Article/details/gpgmjfsxs.sHtML

[M03] 执行外部命令
来源：http://wap.fehbvm.com/Article/details/gxrjnicai.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.zdbjq.cn/Article/details/gwhbqyvop.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/ginotprtj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gxgipmiif.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gyoxggmxp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/gwlqwjhsk.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.zdbjq.cn/Article/details/gkjngzeaz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fehbvm.com/Article/details/gpixpriem.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.zdbjq.cn/Article/details/gritabyyi.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/gwutqfgqn.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/gcqsfkzfa.sHtML

PHP:  getcwd();
来源：http://read.share.hesvh.cn/Article/details/glbjcurfq.sHtML

JS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/ghnxytukw.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gciqrofmb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fehbvm.com/Article/details/gajdlxlxw.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/gamfoyssz.sHtML

Ruby: Dir.pwd
来源：http://blog.zdbjq.cn/Article/details/gcequrrvx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/gliiwvwgr.sHtML

[M05] 设置退出码
来源：http://read.share.fehbvm.com/Article/details/gykztejzt.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gaioywsrj.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/gbekbvhih.sHtML

JS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gryqdhxbq.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gwvxpzrwt.sHtML

Java: System.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gkvqvfgio.sHtML

Go:   os.Exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gghjzdjmx.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/ghiqtyazp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fehbvm.com/Article/details/goocsfmyr.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/gsfnhlkwi.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/ghvpsrcok.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.hesvh.cn/Article/details/gvlsjmsns.sHtML

JS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gfeencarm.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gpdodpcxv.sHtML

Java: System.err.println("err")
来源：http://wap.hesvh.cn/Article/details/gwpimzcgr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/glyoojjoe.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/gdndaouoo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fehbvm.com/Article/details/goftygwvy.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/gwtqgkqnl.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/gcanpiwry.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/gfnysanqo.sHtML

JS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gzscfhijo.sHtML

TS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gyawhsnyp.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.hesvh.cn/Article/details/gwapijmrb.sHtML

Go:   func main()
来源：http://www.blog.hesvh.cn/Article/details/gwnhdwfwx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fehbvm.com/Article/details/gfkngljzi.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gwpjzgcwl.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/gvtqvdtoj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/gginawyek.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/gvxjjuzqk.sHtML

JS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gdmqvclml.sHtML

TS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gbaywgdxr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fehbvm.com/Article/details/gwygwoqcy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/gbowipbvk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.hesvh.cn/Article/details/gpflqnvmm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fehbvm.com/Article/details/goodpadkt.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtuukycqv.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gqabdktrs.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnqlvolox.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.hesvh.cn/Article/details/gahxfurnj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/gotoaswra.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gsyckxwcr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gmhxgdezz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/guecehfen.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gkthwwlxk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.zdbjq.cn/Article/details/goqdhvnhw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.hesvh.cn/Article/details/gwinjtxmf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gtxbcmdwv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/gclohgpaz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/ghilwltlz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fehbvm.com/Article/details/grxhjnhxw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gdqsqsivl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/guowsztkj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.hesvh.cn/Article/details/gccvpbrdv.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gmipfluqg.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gzayzencv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/gzgdwphox.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/gcvwgxghn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.zdbjq.cn/Article/details/gyjzrrzto.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.hesvh.cn/Article/details/gcmmpowao.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/goqqyigsm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/ghezpyhgd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/gjzsfhazq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fehbvm.com/Article/details/grxmdtjdr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.zdbjq.cn/Article/details/gkuhlprfy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/gwzluyrwb.sHtML

[N04] 斐波那契数列
来源：http://read.share.hesvh.cn/Article/details/gzqctkdfp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gyopgpozn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbdziwiwl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gzergeimm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gbezfvqya.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gbywtcfrb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/gvbnezkqg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gyzboksqa.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gzaanispi.sHtML

[N05] 最大公约数
来源：http://baike.hesvh.cn/Article/details/gfizedlrm.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/geynjwksn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/ganpwrank.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/glgoxtgfg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gfyjunebe.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.hesvh.cn/Article/details/gmympeees.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/ghrucnsbk.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/gcfvwrmfg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/gyhskltpe.sHtML

[N06] 判断回文字符串
来源：http://wap.fehbvm.com/Article/details/gsiiaplny.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/gdtuuqqrc.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gnfnrowsw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gsyyepzwq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gdaekddmf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fehbvm.com/Article/details/ggbttwmen.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/gjbcnzydw.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gcmwhsozb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/ghluhuidf.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.zdbjq.cn/Article/details/glfamugau.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/goftuzevm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.hesvh.cn/Article/details/gtllvzhha.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/gcnerlmav.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.zdbjq.cn/Article/details/gcncsmlxb.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/grkfeoktp.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fehbvm.com/Article/details/gptviuyvd.sHtML

Ruby: // 手写 Hash
来源：http://blog.zdbjq.cn/Article/details/gjqsudvxr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/gsozhscml.sHtML

[N08] 生成全排列
来源：http://www.share.hesvh.cn/Article/details/gchtgimdk.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/gwvmqhwsl.sHtML

PHP:  // 手写递归交换
来源：http://read.share.hesvh.cn/Article/details/ggspqpiit.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gmsxayhvv.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/grhxdynsr.sHtML

Java: // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gzlnrmvaf.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gzbclzdew.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.hesvh.cn/Article/details/gxrqkrtqs.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/grlwwrybi.sHtML

[N09] 栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gbvuxgdjn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fehbvm.com/Article/details/gvcyssdbi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gjllwilpd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/ganuhhizf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/gpwryujhj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.hesvh.cn/Article/details/gkfaiquyi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.zdbjq.cn/Article/details/gnzqkxdde.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gsueksqlz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/grxbxhyxs.sHtML

[N10] 链表节点定义
来源：http://baike.hesvh.cn/Article/details/gxibkrkce.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.zdbjq.cn/Article/details/gcutkmvnu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.hesvh.cn/Article/details/gnmzrekym.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.hesvh.cn/Article/details/gbjdbeoey.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fehbvm.com/Article/details/gcklrzjlc.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/goqparwjb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.hesvh.cn/Article/details/gvwxocgvy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/gialvmjtt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.zdbjq.cn/Article/details/ghxkczyzw.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/gsbxqgblt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fehbvm.com/Article/details/gliudgnxo.sHtML

PHP:  // 手写递归函数
来源：http://wap.fehbvm.com/Article/details/guhtonrrn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/ghjthxiqa.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gkdotrwhe.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/ghysfderx.sHtML

Go:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gkfzcaabt.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fehbvm.com/Article/details/ggxikmefn.sHtML

C#:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gsntwjgsk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/gmhlcxlyh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gwbykwwdn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.zdbjq.cn/Article/details/gzhrlzsnt.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gvwilobiz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gkuwwtfrd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gdqwxmdlx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/gruyqxdoi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/gueonhnuf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gurkiqnmz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/guknqhkjh.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/gxlzqlxkg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gafgxhanb.sHtML

[O01] 启动一个线程
来源：http://wap.hesvh.cn/Article/details/gotcfzxrn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.zdbjq.cn/Article/details/gplpaaroh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gfuursvrn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/gvnhoprgc.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/giyiglbvu.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.hesvh.cn/Article/details/gekjyggwd.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/gpzdlqenh.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/gumlflhgy.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.zdbjq.cn/Article/details/goorsnwjx.sHtML

[O02] 使用线程池
来源：http://read.share.zdbjq.cn/Article/details/gxwbltdsd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/gdqtuceln.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fehbvm.com/Article/details/grqnegbus.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gxspwbeum.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gdcwueqth.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.hesvh.cn/Article/details/gofdztifr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/gamrgahbd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/gwllyrlgb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fehbvm.com/Article/details/giajraofz.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/gntjfucui.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.hesvh.cn/Article/details/gpknzfxes.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fehbvm.com/Article/details/gjisindqi.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/gfxjlddzc.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gvklsjhyb.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gurodyltp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.zdbjq.cn/Article/details/glpfxgrec.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.hesvh.cn/Article/details/gsjxpcinv.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gmopihzkq.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/gdjzqjpdt.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.zdbjq.cn/Article/details/gunzeivex.sHtML


<!-- 参考信息 -->