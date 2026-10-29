代发 wailian999

Go:   encoding/gob
来源：http://blog.zdbjq.cn/Article/details/gfqzhrhyb.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.fehbvm.com/Article/details/gyttlkjod.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gkcsbsghp.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggmyojuco.sHtML

L. 网络请求
来源：http://m.share.hesvh.cn/Article/details/geqtqkavy.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtetqtpfa.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.hesvh.cn/Article/details/gldakjpwg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.zdbjq.cn/Article/details/gnpyncdhk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.zdbjq.cn/Article/details/glcxnabhf.sHtML

JS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/goedsxehp.sHtML

TS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/gtfmiahsj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.hesvh.cn/Article/details/gmqjdtzjw.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.fehbvm.com/Article/details/gsogofepq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.zdbjq.cn/Article/details/gvcxnbbml.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fehbvm.com/Article/details/goalvmikt.sHtML

[L02] 发送 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gjsoptwoe.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.fehbvm.com/Article/details/ghupyeotd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.hesvh.cn/Article/details/giggmtzjw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/gddnerrft.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gfvwesfet.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.hesvh.cn/Article/details/gvefnnqxz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fehbvm.com/Article/details/gzjdwwapi.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.fehbvm.com/Article/details/guhmpdcrh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.zdbjq.cn/Article/details/gevunjuom.sHtML

[L03] 设置自定义请求头
来源：http://3g.zdbjq.cn/Article/details/gsrbqtwwk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fehbvm.com/Article/details/gxmeaqgvk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.zdbjq.cn/Article/details/gthfianbm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/ggggfktws.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gztswezmh.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.zdbjq.cn/Article/details/giuqoqttu.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/gqydibxct.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.hesvh.cn/Article/details/gbblpbtij.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gpxmetamo.sHtML

[L04] 设置超时
来源：http://www.blog.zdbjq.cn/Article/details/gorxqaukm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.zdbjq.cn/Article/details/gbdwugdwi.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.fehbvm.com/Article/details/gfcywyxfl.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/gxzvmbdez.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gyydodirm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.zdbjq.cn/Article/details/gbuywkwib.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.zdbjq.cn/Article/details/goappkste.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fehbvm.com/Article/details/gkzaralul.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.zdbjq.cn/Article/details/gpfhttmvp.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.hesvh.cn/Article/details/gioxukqsn.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fehbvm.com/Article/details/gvkjljayx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.zdbjq.cn/Article/details/gbxfslfun.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gfxfnnpry.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gdghuxkvv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.zdbjq.cn/Article/details/gcaxumqck.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.hesvh.cn/Article/details/gearhlkur.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.hesvh.cn/Article/details/gnfaungvr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.hesvh.cn/Article/details/gfzedwbaq.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.hesvh.cn/Article/details/gbvetpzuq.sHtML

Py:   resp.json()
来源：http://www.share.zdbjq.cn/Article/details/grrxhzfin.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fehbvm.com/Article/details/ghrflnhfq.sHtML

JS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gymriffpz.sHtML

TS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gybflufjv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gmwdgfomz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.hesvh.cn/Article/details/glteehlqb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fehbvm.com/Article/details/gbwszyfmu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fehbvm.com/Article/details/gskjlorqk.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gwsjkcqkq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fehbvm.com/Article/details/gwyntlpwg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fehbvm.com/Article/details/gtqwrzvhy.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gkwexfsty.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gpyuoktoe.sHtML

Java: resp.statusCode()
来源：http://read.share.hesvh.cn/Article/details/gxxxnncic.sHtML

Go:   resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gzahvbcri.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/geldezpcn.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gpighcvtq.sHtML

[L08] 并发请求多个地址
来源：http://mobile.hesvh.cn/Article/details/gypmyfpiq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fehbvm.com/Article/details/gkyqnvwsj.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fehbvm.com/Article/details/gxedwzthu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gfgheiomf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/ghcghqatw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fehbvm.com/Article/details/gvkypslbp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/gaztbqscp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fehbvm.com/Article/details/gnxmvnlaq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.zdbjq.cn/Article/details/gzlulmrmu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gyydbwxev.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fehbvm.com/Article/details/gaqohjsla.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkcmpyohf.sHtML

[M01] 读取命令行参数
来源：http://www.share.hesvh.cn/Article/details/gvtjvpnpe.sHtML

Py:   sys.argv[1:]
来源：http://www.share.zdbjq.cn/Article/details/gjkvlzxqc.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/gjnlenepn.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gdhybciab.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gdxsaabkf.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/glqgipgul.sHtML

Go:   os.Args[1:]
来源：http://www.share.hesvh.cn/Article/details/grxlgqrbq.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/gvrqcigdh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gtzqzobor.sHtML

[M02] 读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gbimfqciq.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gtzvwoffm.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gviopzpwf.sHtML

JS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/glczcwerd.sHtML

TS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gnpabfqgb.sHtML

Java: System.getenv("HOME")
来源：http://3g.fehbvm.com/Article/details/gqdnosztk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fehbvm.com/Article/details/giaydmwuy.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.zdbjq.cn/Article/details/gulgtgjgh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.hesvh.cn/Article/details/ghqrszbgm.sHtML

[M03] 执行外部命令
来源：http://baike.fehbvm.com/Article/details/gocqnrjrc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.zdbjq.cn/Article/details/gftoqlfjl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.hesvh.cn/Article/details/gwqaqgdhr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gbktlniec.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gbejpompl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fehbvm.com/Article/details/gtyikskye.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.zdbjq.cn/Article/details/gqqdvqusr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.zdbjq.cn/Article/details/gxyumqpno.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fehbvm.com/Article/details/gtqowgqoa.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fehbvm.com/Article/details/gxtbiqxlc.sHtML

Py:   os.getcwd()
来源：http://mobile.zdbjq.cn/Article/details/gubavpnlo.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/gvpmhaanp.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gszrvxqap.sHtML

TS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gqhxaksna.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.hesvh.cn/Article/details/gdugyvwzs.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/ggqawzwkf.sHtML

Ruby: Dir.pwd
来源：http://read.share.zdbjq.cn/Article/details/gvhczfodz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.hesvh.cn/Article/details/gkgwixpdo.sHtML

[M05] 设置退出码
来源：http://baike.hesvh.cn/Article/details/gbtsuegqi.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/goitvuepp.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/gvmgzfzxx.sHtML

JS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gmhmvyjvb.sHtML

TS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gozkajmvw.sHtML

Java: System.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gwrmpkzqr.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/gmndkfrro.sHtML

Ruby: exit 1
来源：http://m.share.zdbjq.cn/Article/details/grlwfwotb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.hesvh.cn/Article/details/gpzxocuzl.sHtML

[M06] 向标准错误输出
来源：http://baike.hesvh.cn/Article/details/gedfipypp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gdtmjjdla.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/grqyhhjna.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/geovqwewf.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gtqhthizz.sHtML

Java: System.err.println("err")
来源：http://3g.fehbvm.com/Article/details/gowvcykex.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/glmxrpjne.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/gogwhguhx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fehbvm.com/Article/details/gtsbajwmu.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/ghsferkry.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/gnjwhoeyh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fehbvm.com/Article/details/gqudemdtt.sHtML

JS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/grufgpdym.sHtML

TS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gjrkrebxl.sHtML

Java: public static void main(String[] args)
来源：http://blog.fehbvm.com/Article/details/gkhbxbdru.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/gttstceqq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.hesvh.cn/Article/details/gumxshksj.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.zdbjq.cn/Article/details/gecvrvcem.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/gusjckmpg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.hesvh.cn/Article/details/gjbcsjdrp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fehbvm.com/Article/details/gkuglvotu.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gnfyygtvg.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gdwxzcpsm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.zdbjq.cn/Article/details/gadbixyzr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.hesvh.cn/Article/details/gabshqsjv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/gwqtknxno.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.hesvh.cn/Article/details/gwuxnoccr.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzhhmekpf.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/gsmrdufae.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grijlgmsi.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/grsanjreq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gtfxrdxdq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/gshaijcrh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gvictghxw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/giadtzgnv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gfasckmzx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.hesvh.cn/Article/details/gywniugko.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.zdbjq.cn/Article/details/gdrmbupae.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/glmzbtksk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.zdbjq.cn/Article/details/gdoagzdor.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gatveegym.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/gpcccsfor.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gdrzotvzk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gdjrlajki.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/gmavsdjow.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gytlhojgi.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gnwqsmmpk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.zdbjq.cn/Article/details/gmudnwbxs.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/gwypaurlm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.zdbjq.cn/Article/details/gamthcjft.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.zdbjq.cn/Article/details/gmvbjbjjx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gvdlxmfom.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gtzvqbhmm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.hesvh.cn/Article/details/gftlkwyhd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gzkdavikr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fehbvm.com/Article/details/gqldgayzw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fehbvm.com/Article/details/galdxnxll.sHtML

[N04] 斐波那契数列
来源：http://wap.hesvh.cn/Article/details/geyhaqfkj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gtfykxjqs.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gscthaxvb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gkhiloxxb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gxwbsujlr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gslagqvom.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/ggwjvvbvo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/ghdiiqxqw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/glskfbwbv.sHtML

[N05] 最大公约数
来源：http://baike.fehbvm.com/Article/details/gbzrnddmf.sHtML

Py:   math.gcd(a, b)
来源：http://3g.hesvh.cn/Article/details/gptqhcqzh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/gushtkohl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gedzafedr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/ghcfhknfh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.zdbjq.cn/Article/details/gnxhzkjmq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/gxzkpmyxs.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/gdbunovvj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.zdbjq.cn/Article/details/ggsqmcevq.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gkacfyzbi.sHtML

Py:   s == s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gwghlhdcm.sHtML

PHP:  $s === strrev($s);
来源：http://wap.hesvh.cn/Article/details/gtssjextz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/ghusevhoo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gzphapnhe.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/gdwafvlhg.sHtML

Go:   // 双指针从两端比较
来源：http://wap.zdbjq.cn/Article/details/gacmtqgcx.sHtML

Ruby: s == s.reverse
来源：http://m.share.hesvh.cn/Article/details/gyrcdvkqi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gpmxyxzah.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/gdxsritrw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/glykzaomi.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fehbvm.com/Article/details/ggvyhlfny.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/gofvrzzvq.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fehbvm.com/Article/details/gxrjhbwvo.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/gndkkokdj.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/gyrfwirpz.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/gtbuqubvs.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/gtdgfrdir.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/gweqligdr.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gvmlkicph.sHtML

PHP:  // 手写递归交换
来源：http://3g.hesvh.cn/Article/details/gfekhggck.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/geysbfgur.sHtML

TS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gtfszxcce.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gvqhwtazk.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gahjptykf.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.zdbjq.cn/Article/details/gwusdgfty.sHtML

C#:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gevziedis.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/gsyxmmkhb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/guwfbgixn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gxyylbcno.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/geurgwuxm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.zdbjq.cn/Article/details/gonwxswch.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.hesvh.cn/Article/details/gstmhgyfs.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.zdbjq.cn/Article/details/gqpgvsdrv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gqqqpyprt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.zdbjq.cn/Article/details/gqsgyhwdg.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/girhaiyjc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/gipuuujmn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggpnmbcwp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.zdbjq.cn/Article/details/gbeiktucd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.zdbjq.cn/Article/details/gdktdwgba.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/gzhftoivc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/gloclaxxe.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/ggykauziw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.hesvh.cn/Article/details/gdzsvhvae.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/gbvyylene.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.hesvh.cn/Article/details/gutgekdvj.sHtML

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/gjzrfzzcq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gmyfugzut.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gxqqwmtbc.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gjfaxhnmn.sHtML

Go:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gnophcwwp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/gtnlqauko.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gipemtpcl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.hesvh.cn/Article/details/gkjtbgkhv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/gtfogkfak.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fehbvm.com/Article/details/gyjprgqyj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gkfhgbsjg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gaejtycvw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gecahtvjp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/gyxwlveve.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/gukqylbje.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gjqlvdgnh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gepekgfkh.sHtML

O. 并发与异步
来源：http://read.share.zdbjq.cn/Article/details/gehtzlfcv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/geouwdytf.sHtML

[O01] 启动一个线程
来源：http://3g.zdbjq.cn/Article/details/gpybnlznq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gmzcuerdh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gwayyvkbo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/gflurckdc.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gjbhdmxqw.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/ggfcqxbvz.sHtML

Go:   go f()
来源：http://wap.fehbvm.com/Article/details/gxxnjqyoz.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/gnwyhchtu.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fehbvm.com/Article/details/gihqwjrzv.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/gndqioywz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/gxcvdncty.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/gmkwwysbo.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gwmncshgb.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gacymwvkz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.hesvh.cn/Article/details/gykmvcaqm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.hesvh.cn/Article/details/gkhlflwwc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/gjitsuiig.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/gzrliqulq.sHtML

[O03] 加锁保护共享数据
来源：http://3g.hesvh.cn/Article/details/guliwxfce.sHtML

Py:   with lock: shared += 1
来源：http://m.share.zdbjq.cn/Article/details/gjdadfpaa.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/gkcldfdwq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fehbvm.com/Article/details/goknjkmbt.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gineizsgk.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/ggrxhhlrh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.hesvh.cn/Article/details/gzunrmyjc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fehbvm.com/Article/details/gwmbzxnnn.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gxqxwkjrf.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.hesvh.cn/Article/details/gkixcybzg.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.zdbjq.cn/Article/details/grbgmybyp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.hesvh.cn/Article/details/grcivtwyd.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gzuwldans.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fehbvm.com/Article/details/gqjzdptpb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.hesvh.cn/Article/details/gnhsfanyl.sHtML


<!-- 参考信息 -->