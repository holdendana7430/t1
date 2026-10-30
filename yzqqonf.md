代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.zdbjq.cn/Article/details/gsbfgeusb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gdjxizjgd.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/gurrbfbir.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.fehbvm.com/Article/details/gbhmhpchk.sHtML

Go:   encoding/gob
来源：http://read.share.zdbjq.cn/Article/details/grpwooddj.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.hesvh.cn/Article/details/gyhrjoiwp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/gjyiivbbx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbdlkmsvu.sHtML

L. 网络请求
来源：http://www.blog.fehbvm.com/Article/details/ghlnzevpk.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glgmopkqf.sHtML

[L01] 发送 GET 请求
来源：http://baike.hesvh.cn/Article/details/guphswlfx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.hesvh.cn/Article/details/gaegoxatn.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fehbvm.com/Article/details/gsjkgdwta.sHtML

JS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/garslattt.sHtML

TS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gsvwybyia.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.zdbjq.cn/Article/details/gtxluqlvd.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.hesvh.cn/Article/details/gtxjiwegm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.fehbvm.com/Article/details/gpjreyvch.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.zdbjq.cn/Article/details/gqxbcbvfc.sHtML

[L02] 发送 POST JSON
来源：http://3g.fehbvm.com/Article/details/grjuomksg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gynzclaxn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.zdbjq.cn/Article/details/ghcwumvyh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gkhrcpcpg.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gnnbpuqat.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.fehbvm.com/Article/details/gospphsaz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.hesvh.cn/Article/details/grndtjqkf.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.zdbjq.cn/Article/details/giqmdaolw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.hesvh.cn/Article/details/gkzuahzab.sHtML

[L03] 设置自定义请求头
来源：http://baike.hesvh.cn/Article/details/gxqyckfmq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.zdbjq.cn/Article/details/ggozicrpi.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.zdbjq.cn/Article/details/gmzphzisp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/gabbrnnef.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gvsygavks.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.zdbjq.cn/Article/details/gajuazshr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/gtkkdghua.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.zdbjq.cn/Article/details/gcrigjnzf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gqgrydgto.sHtML

[L04] 设置超时
来源：http://m.share.fehbvm.com/Article/details/gmojnpciy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.zdbjq.cn/Article/details/gneraxbuu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.zdbjq.cn/Article/details/gnnlkcwvo.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/gufhtxgmb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gkvzbrsyn.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.hesvh.cn/Article/details/gusnioylx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.fehbvm.com/Article/details/gwzlfjoiw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.hesvh.cn/Article/details/gecxnboun.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.fehbvm.com/Article/details/gpdqmtyeo.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.hesvh.cn/Article/details/gguacknvv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.hesvh.cn/Article/details/glyioxacx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.zdbjq.cn/Article/details/gedithhjq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/ghvknjciq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gqvdtnkuu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.hesvh.cn/Article/details/gnreddvqg.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.zdbjq.cn/Article/details/grkoccpbw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.hesvh.cn/Article/details/glcfwxwur.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.hesvh.cn/Article/details/grbaujssq.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.zdbjq.cn/Article/details/gynpkfmti.sHtML

Py:   resp.json()
来源：http://blog.zdbjq.cn/Article/details/gheeuxjaw.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fehbvm.com/Article/details/gddaualqa.sHtML

JS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gmdvwaeus.sHtML

TS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gvypkzkjl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.hesvh.cn/Article/details/gyrckgtix.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fehbvm.com/Article/details/gqhpflols.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fehbvm.com/Article/details/gpjmkwumz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fehbvm.com/Article/details/giocdbrzv.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gwahhobgg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.hesvh.cn/Article/details/gesowgfze.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fehbvm.com/Article/details/gpaozxhqx.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gajwoptyw.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gldjfbrzk.sHtML

Java: resp.statusCode()
来源：http://3g.zdbjq.cn/Article/details/gjckjvaze.sHtML

Go:   resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/glbbogxpi.sHtML

Ruby: resp.code.to_i
来源：http://mobile.hesvh.cn/Article/details/gynqwlils.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gtmeubuvd.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fehbvm.com/Article/details/gsmzhxmci.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fehbvm.com/Article/details/gmpxceldy.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.zdbjq.cn/Article/details/gfaxjlbci.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/glnauzmxt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gjcokliow.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.hesvh.cn/Article/details/gqrpuaxik.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.hesvh.cn/Article/details/gxkqbhrck.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.hesvh.cn/Article/details/gwmkyvjja.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.zdbjq.cn/Article/details/gsnewlkoy.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdkgshyyd.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.hesvh.cn/Article/details/gbrehodaz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmkdgkhrv.sHtML

[M01] 读取命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gztdglbny.sHtML

Py:   sys.argv[1:]
来源：http://3g.fehbvm.com/Article/details/gcpaidsdk.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fehbvm.com/Article/details/gwwbleuhn.sHtML

JS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gkpgrrjjr.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gvoktwoxl.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gixqlqhkg.sHtML

Go:   os.Args[1:]
来源：http://m.share.fehbvm.com/Article/details/gtpmnmwag.sHtML

Ruby: ARGV
来源：http://www.m.share.fehbvm.com/Article/details/giuhjkacb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/ghyzbfpkd.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gbwizpwpa.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fehbvm.com/Article/details/gnvwjtbyo.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gunxzhgzm.sHtML

JS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gdiwekuyy.sHtML

TS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gdcbprljb.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gokvvxqys.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gvokvbgon.sHtML

Ruby: ENV["HOME"]
来源：http://3g.hesvh.cn/Article/details/gwhtxnhdk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.zdbjq.cn/Article/details/gwctkucmc.sHtML

[M03] 执行外部命令
来源：http://www.blog.hesvh.cn/Article/details/gudktyazj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fehbvm.com/Article/details/gpoqkkyro.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.zdbjq.cn/Article/details/gwjkqymvr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gpkgywijh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gjvpqytsu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.zdbjq.cn/Article/details/gqgwubrao.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fehbvm.com/Article/details/gnyoddiez.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/gbbqznbwo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/gzpkuatlh.sHtML

[M04] 获取当前工作目录
来源：http://mobile.hesvh.cn/Article/details/gihbynobm.sHtML

Py:   os.getcwd()
来源：http://3g.hesvh.cn/Article/details/gdwrwupcw.sHtML

PHP:  getcwd();
来源：http://m.share.hesvh.cn/Article/details/gbolulrat.sHtML

JS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gecabwdjm.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gdszatrtd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.hesvh.cn/Article/details/gpfsuikag.sHtML

Go:   os.Getwd()
来源：http://baike.zdbjq.cn/Article/details/gpoilzzww.sHtML

Ruby: Dir.pwd
来源：http://read.share.fehbvm.com/Article/details/gxllkgmoi.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.hesvh.cn/Article/details/goafjhpsa.sHtML

[M05] 设置退出码
来源：http://read.share.zdbjq.cn/Article/details/gulnayngk.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/grtxrifjd.sHtML

PHP:  exit(1);
来源：http://wap.hesvh.cn/Article/details/gtjtizstd.sHtML

JS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gxnrfntfo.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gncrnfvad.sHtML

Java: System.exit(1)
来源：http://blog.fehbvm.com/Article/details/gjqbxacgn.sHtML

Go:   os.Exit(1)
来源：http://m.share.zdbjq.cn/Article/details/goiwlcljx.sHtML

Ruby: exit 1
来源：http://www.m.share.hesvh.cn/Article/details/gqkxqtpbz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/gltbpggzr.sHtML

[M06] 向标准错误输出
来源：http://m.share.fehbvm.com/Article/details/gltjtivrx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gacguewyd.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/gifxenhrw.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gynlwvduv.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/giwrabpuz.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/gtfqnvkdk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.zdbjq.cn/Article/details/glsgqqqwf.sHtML

Ruby: warn "err"
来源：http://www.share.fehbvm.com/Article/details/genpairjt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/gonjxneux.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fehbvm.com/Article/details/gjwmtwqdr.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.hesvh.cn/Article/details/gkyaaedta.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fehbvm.com/Article/details/gyxtujzfx.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gnbpuqewp.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/guvymgwqc.sHtML

Java: public static void main(String[] args)
来源：http://m.share.hesvh.cn/Article/details/gtfuunqdr.sHtML

Go:   func main()
来源：http://baike.fehbvm.com/Article/details/gvotzldmi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fehbvm.com/Article/details/gjrapacjl.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/goyprxisg.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/gfwfaaleq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/gsbdmhjtr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/gksimijgn.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gkckhsjho.sHtML

TS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gmwxksmsl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.hesvh.cn/Article/details/gflmueusf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fehbvm.com/Article/details/giknluybi.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gqhelhpji.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/gysnnburw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gyzjfdvqf.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gofxohwhu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grsyngukm.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.hesvh.cn/Article/details/gisqpyvav.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/ggecifxkm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fehbvm.com/Article/details/gylswbrrf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gytttondh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gvdjoezuw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/goyffvptt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gecqphdpp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gdgsuzngo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gzixdmzng.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fehbvm.com/Article/details/gnylfofce.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/ghpdiddwa.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/gixkbqvyt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gyqgehmoz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gnvmetmen.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/gmqgmyick.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gzwtjbiyu.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gwghoxkae.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fehbvm.com/Article/details/goxiycaza.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/gkeotqxxr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.zdbjq.cn/Article/details/gwwpleqoc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.zdbjq.cn/Article/details/gkjkmmzxc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gsakmiijx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gwciyeens.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/gtgkweknr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gddqaciig.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.hesvh.cn/Article/details/gxoesflkg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gfqrbpmue.sHtML

[N04] 斐波那契数列
来源：http://read.share.hesvh.cn/Article/details/gaioorerd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gjmjwdszr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gwcbemtqw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/glgtgzfda.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gnhqyxupt.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gykblztis.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.zdbjq.cn/Article/details/gefnctimp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gtwrotwze.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gkuohwyrg.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/ghwnvfjdp.sHtML

Py:   math.gcd(a, b)
来源：http://3g.hesvh.cn/Article/details/gzjjxhsxy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gbfduudhq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gzvpnvvzg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gbhnwwbuh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/ggosykasb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/ggkjgsnfw.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fehbvm.com/Article/details/gtlurfvhj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/gahbzgaws.sHtML

[N06] 判断回文字符串
来源：http://www.share.zdbjq.cn/Article/details/gxubbzyne.sHtML

Py:   s == s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gtpesvlrz.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fehbvm.com/Article/details/gwnnxwmcy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gshayswct.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gggiprwfx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.fehbvm.com/Article/details/gqwyraspk.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/gfljbghzc.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/gdlqehfcp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gtaqpqfek.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/gomzysipf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.hesvh.cn/Article/details/gtkszhvzr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/ggfdifhuy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.hesvh.cn/Article/details/goiwyqjhf.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gamdjqszg.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/gqjwwwprc.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.hesvh.cn/Article/details/gmsyaviiu.sHtML

Ruby: // 手写 Hash
来源：http://baike.hesvh.cn/Article/details/gciduplkh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.hesvh.cn/Article/details/gsxsfkfzb.sHtML

[N08] 生成全排列
来源：http://wap.hesvh.cn/Article/details/gsxoohcwa.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/gbptvpwud.sHtML

PHP:  // 手写递归交换
来源：http://blog.fehbvm.com/Article/details/gbkjvnchq.sHtML

JS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gvofvpzhq.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gumbyhdpv.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/grxaxnmrf.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gswzufjfa.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.hesvh.cn/Article/details/gqdwpbsiy.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gyodimfkc.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/gqycyyhku.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gixuxwsog.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gbndjrfgb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gsdbbbokx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/ghvnhoswl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/gnjhhgkpk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/gjcrtdoho.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gpmyrcpvc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/gfpkpzqkh.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/getgubqbv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.hesvh.cn/Article/details/gcarpvxji.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gjnoeehtl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/greavxbtb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/gedjovglr.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.zdbjq.cn/Article/details/gadmpqnjx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/gkslrhxyu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.hesvh.cn/Article/details/giinmzgbe.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/gwjykznyq.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fehbvm.com/Article/details/gfklwrrzz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gcaoidxzr.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fehbvm.com/Article/details/gcjsnflca.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gewlambkd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/ghundupgf.sHtML

Java: // 手写递归
来源：http://www.share.hesvh.cn/Article/details/ggrndhjjv.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gcjjfapwm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/gglcrvoac.sHtML

C#:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/ghzwkymbt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.zdbjq.cn/Article/details/gzmcftnqo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fehbvm.com/Article/details/gidoyvxki.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.hesvh.cn/Article/details/grtcbwrpb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gnuthbrxa.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gishdecnz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gtmwzclge.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/goonmbxor.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/gqftgtrjy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gvkzcrtra.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/guoivgptg.sHtML

O. 并发与异步
来源：http://www.m.share.fehbvm.com/Article/details/gkkmpjzzy.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gsksmxamp.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/gngvpvfwi.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fehbvm.com/Article/details/gvdnshkaj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/gphqmclui.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.hesvh.cn/Article/details/gxfmdlknx.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gpqkorchl.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fehbvm.com/Article/details/glllhogsb.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/gaayphqlj.sHtML

Ruby: Thread.new { f }
来源：http://read.share.zdbjq.cn/Article/details/ghbfgdmqz.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fehbvm.com/Article/details/gpteuhdqg.sHtML

[O02] 使用线程池
来源：http://mobile.zdbjq.cn/Article/details/guzhspcrv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.hesvh.cn/Article/details/gtlyydecu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/gnewjdmur.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gkevhhbhj.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gvvgzglxp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/glixpkamo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/gtewefqoc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/gcquujuij.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/gzjdppeta.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fehbvm.com/Article/details/gjucfwole.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fehbvm.com/Article/details/gpigisgdg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/grphefjon.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fehbvm.com/Article/details/gozsveaur.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gqgauwxfo.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gltgpwnva.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.zdbjq.cn/Article/details/gqucyasij.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gyvwqcbnh.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gsythrmli.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fehbvm.com/Article/details/guhdmgyrx.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fehbvm.com/Article/details/gndagqsbx.sHtML


<!-- 参考信息 -->