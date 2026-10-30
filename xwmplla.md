代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fehbvm.com/Article/details/gxjgxebmf.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gcrgpnfdq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.fehbvm.com/Article/details/gdjgwkgpm.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fehbvm.com/Article/details/gxfcztswf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.hesvh.cn/Article/details/gfodftaop.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gzxmyhzeg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/gtszmwbhk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.hesvh.cn/Article/details/gqcndrsld.sHtML

Go:   encoding/gob
来源：http://3g.fehbvm.com/Article/details/grwzowprm.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fehbvm.com/Article/details/gqblelngj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gaeblepvc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxufgwngq.sHtML

L. 网络请求
来源：http://read.share.fehbvm.com/Article/details/gyfqkezlz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdtxqocpq.sHtML

[L01] 发送 GET 请求
来源：http://mobile.zdbjq.cn/Article/details/glwpsttzc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.fehbvm.com/Article/details/gmukjjzov.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.fehbvm.com/Article/details/gvlfvvkka.sHtML

JS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gjpqzlfce.sHtML

TS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/glovzuioc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.zdbjq.cn/Article/details/grjvuzlzq.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.fehbvm.com/Article/details/gtsrneuua.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.fehbvm.com/Article/details/gavrxrllo.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.hesvh.cn/Article/details/gqqovxwsg.sHtML

[L02] 发送 POST JSON
来源：http://m.share.fehbvm.com/Article/details/gsicxcfbz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gagqjcqqa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.zdbjq.cn/Article/details/gyurwvwiq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/gihqgaycm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/gydauatkn.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.fehbvm.com/Article/details/gqdjvcuui.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.hesvh.cn/Article/details/gkvrcgrne.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.zdbjq.cn/Article/details/gymybgzqc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.hesvh.cn/Article/details/gusgqmybz.sHtML

[L03] 设置自定义请求头
来源：http://mobile.hesvh.cn/Article/details/guwuxejlq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fehbvm.com/Article/details/gjcpcazuw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.zdbjq.cn/Article/details/gudbjlvuw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/geddzieuq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gxubpnrbg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.fehbvm.com/Article/details/grseounge.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/gvadhywgp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.zdbjq.cn/Article/details/gyeedtwjl.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/ghbyjfkot.sHtML

[L04] 设置超时
来源：http://read.share.fehbvm.com/Article/details/gseenbjag.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.hesvh.cn/Article/details/grqqwrcgq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.zdbjq.cn/Article/details/gkcvphxyj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/gtzpayyft.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gcjhhpxro.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.hesvh.cn/Article/details/ggkjfngoi.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fehbvm.com/Article/details/gjauyuyzi.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.hesvh.cn/Article/details/gszuogpvb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.hesvh.cn/Article/details/gznxgaxun.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fehbvm.com/Article/details/gyzmgedrh.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.hesvh.cn/Article/details/gkmiucdfl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.hesvh.cn/Article/details/ghfanvmdd.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gqtwsussy.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gxbeetcam.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.zdbjq.cn/Article/details/gycjucuza.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.zdbjq.cn/Article/details/gcfjpzwzp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.zdbjq.cn/Article/details/gbxygcfxj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fehbvm.com/Article/details/gvrodopqa.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fehbvm.com/Article/details/gdpzaydzw.sHtML

Py:   resp.json()
来源：http://wap.zdbjq.cn/Article/details/ggzuaanyx.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fehbvm.com/Article/details/gkctdaeun.sHtML

JS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gpscgornp.sHtML

TS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/garbvnjem.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.hesvh.cn/Article/details/giwympsqu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fehbvm.com/Article/details/gxhrbdkqb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.hesvh.cn/Article/details/geqgtkfxk.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.zdbjq.cn/Article/details/gqovjeirg.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gheoykgrj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.zdbjq.cn/Article/details/gehskanxu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.hesvh.cn/Article/details/ggumslogv.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gobfqmiqe.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/grtgqtggv.sHtML

Java: resp.statusCode()
来源：http://3g.fehbvm.com/Article/details/govxurliv.sHtML

Go:   resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gwxbsayis.sHtML

Ruby: resp.code.to_i
来源：http://baike.hesvh.cn/Article/details/gcyfqdbdi.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gjokwjuqo.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fehbvm.com/Article/details/gwrspbguj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.zdbjq.cn/Article/details/gvdagnste.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fehbvm.com/Article/details/gjyiybvqv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gqoxkhcaq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/grvmidaai.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.zdbjq.cn/Article/details/gvignjsmm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fehbvm.com/Article/details/gndisrkhh.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gpklxguwz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.zdbjq.cn/Article/details/gzbuixomh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grufhoxwv.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fehbvm.com/Article/details/grwhlybdg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbmywuffn.sHtML

[M01] 读取命令行参数
来源：http://3g.hesvh.cn/Article/details/gwnxwacds.sHtML

Py:   sys.argv[1:]
来源：http://wap.fehbvm.com/Article/details/gajlikboo.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fehbvm.com/Article/details/gbfwbhkqg.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gzhkzvmpc.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gvvsbosar.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gfxjcvfhv.sHtML

Go:   os.Args[1:]
来源：http://read.share.hesvh.cn/Article/details/ghoszcobb.sHtML

Ruby: ARGV
来源：http://www.blog.zdbjq.cn/Article/details/gnwfvuapt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gmnfljmww.sHtML

[M02] 读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gzqdfcvml.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.zdbjq.cn/Article/details/gieadtcof.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gnutcqccs.sHtML

JS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gjvxiugjb.sHtML

TS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/geicfcpow.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gjrdkhnap.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gksaknvsp.sHtML

Ruby: ENV["HOME"]
来源：http://blog.zdbjq.cn/Article/details/gueoigdoy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.zdbjq.cn/Article/details/ggnqhlaai.sHtML

[M03] 执行外部命令
来源：http://www.m.share.zdbjq.cn/Article/details/gzouxdray.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/gcikuxlhs.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.hesvh.cn/Article/details/gkumzsukl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gavdzbjcp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gmuujnjxo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.zdbjq.cn/Article/details/gcricqcej.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fehbvm.com/Article/details/gmqhsespx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.hesvh.cn/Article/details/gvbmudzxn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fehbvm.com/Article/details/gbmirebkq.sHtML

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/gikgkpaxy.sHtML

Py:   os.getcwd()
来源：http://baike.fehbvm.com/Article/details/glgcasbwr.sHtML

PHP:  getcwd();
来源：http://www.m.share.hesvh.cn/Article/details/gljyqmcvs.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/ggjqvcyic.sHtML

TS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gkmhfabav.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fehbvm.com/Article/details/gqsydpsxj.sHtML

Go:   os.Getwd()
来源：http://wap.hesvh.cn/Article/details/grwoidbtq.sHtML

Ruby: Dir.pwd
来源：http://read.share.hesvh.cn/Article/details/gbefkxjfu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/gyhrgssmg.sHtML

[M05] 设置退出码
来源：http://mobile.zdbjq.cn/Article/details/gbxthbyam.sHtML

Py:   sys.exit(1)
来源：http://baike.fehbvm.com/Article/details/gzfqdduaa.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/glprpyekc.sHtML

JS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gklorayyv.sHtML

TS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/glcxxunvq.sHtML

Java: System.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gcslxlpbo.sHtML

Go:   os.Exit(1)
来源：http://read.share.hesvh.cn/Article/details/gqflmfocx.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/gipmyjeni.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.zdbjq.cn/Article/details/gllbjmcgs.sHtML

[M06] 向标准错误输出
来源：http://3g.hesvh.cn/Article/details/gfpfwgavw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gvcoozqag.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/gtekuxsmm.sHtML

JS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gfzvmiymi.sHtML

TS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gthnlunza.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/ggluonqyx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fehbvm.com/Article/details/gbknbsxbd.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/ghrxoaxmd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fehbvm.com/Article/details/gdkhxhcsn.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.hesvh.cn/Article/details/gylorpzdc.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/goobdcnxe.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.hesvh.cn/Article/details/gdptxbpfg.sHtML

JS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gtzwxxpsn.sHtML

TS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gafcpnfaf.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/gqltkvwof.sHtML

Go:   func main()
来源：http://mobile.zdbjq.cn/Article/details/ggseplsza.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/gpoopykky.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.zdbjq.cn/Article/details/ghiwipfko.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/gmvinvffa.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.hesvh.cn/Article/details/gilgztfuk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/grwisbocr.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gmgkidlyv.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gxexlkqgp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fehbvm.com/Article/details/gkmripvzg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.zdbjq.cn/Article/details/gtdyhomtu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/gsjjulrzg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fehbvm.com/Article/details/grfrzynmj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grdqvrvpb.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/gaihgsgyy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxxjrtifw.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.zdbjq.cn/Article/details/gfjjkrxuk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gkkrholzf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.zdbjq.cn/Article/details/ghxszdsjs.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gipamcprh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gkpydxqgq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gzfirksbp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.hesvh.cn/Article/details/giocutbva.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/geexrdwsy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gbgecdlmw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.hesvh.cn/Article/details/gzaqjkmgg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gkwtonjus.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.zdbjq.cn/Article/details/gvljbhmie.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gjjxorfuk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gmugqupwu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.zdbjq.cn/Article/details/gwredfoje.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gcagjodxs.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/goxkwrnjz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.zdbjq.cn/Article/details/gmhhjdjbj.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.hesvh.cn/Article/details/gqkjtvjyt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/gdvbnzfmi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/gwmoilkju.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gnuarxmji.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gfykipgeo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.hesvh.cn/Article/details/gkdyworwv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.hesvh.cn/Article/details/guusclncs.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/gfdldmqaa.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.zdbjq.cn/Article/details/gummfxzkn.sHtML

[N04] 斐波那契数列
来源：http://m.share.fehbvm.com/Article/details/gvebqajtg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gkuycgkfk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.hesvh.cn/Article/details/gqvmvrgid.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gifznsgmh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gwqatehkd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gbmnwgiod.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fehbvm.com/Article/details/gmqzzqihn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gxwmlwyfv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gavrbfata.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/goepdvyeg.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gtfwmqukp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.zdbjq.cn/Article/details/gpoolnszw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gvolkxfge.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gngzmmcxv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/ggttbjcvu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/gpuouydib.sHtML

Ruby: a.gcd(b)
来源：http://blog.zdbjq.cn/Article/details/ghxwyumgy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.zdbjq.cn/Article/details/gcpjxyswp.sHtML

[N06] 判断回文字符串
来源：http://m.share.hesvh.cn/Article/details/ggrbeidcx.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/ghtrxzcvh.sHtML

PHP:  $s === strrev($s);
来源：http://3g.zdbjq.cn/Article/details/glwblxtov.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gxgcdumin.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gddytfqdc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/gaieznams.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/grugakkmp.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gjwxusunk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gmckpznvq.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/gvykkghjx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/gxujqduvu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/gyspbhjya.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/goqapyiuk.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.zdbjq.cn/Article/details/gnwvymczn.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/gfxxfibjh.sHtML

Go:   // 手写 map[int]int
来源：http://blog.zdbjq.cn/Article/details/gvicmsoog.sHtML

Ruby: // 手写 Hash
来源：http://3g.hesvh.cn/Article/details/gvdlpsiex.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/gkhwfoqhv.sHtML

[N08] 生成全排列
来源：http://mobile.zdbjq.cn/Article/details/gqcydwhjc.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fehbvm.com/Article/details/glehraruk.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/ggngmxgzl.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/geattjtzx.sHtML

TS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gxrjtrbsj.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/glpwyvkyo.sHtML

Go:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gazjqtzxl.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/gpnlmiytx.sHtML

C#:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gkguddqtf.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gptxvejuc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.fehbvm.com/Article/details/gecanemzw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gcvtjyush.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gwuhkbvrz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fehbvm.com/Article/details/gjgxyqxgq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/gnekltiil.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/gccvjaofc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gcgizmibh.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gdlkgmrzt.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/gumrsfjqx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.zdbjq.cn/Article/details/geneelzjs.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdsytcwnj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/gwrfkgjfx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/gpgwyvcjs.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fehbvm.com/Article/details/gcsnfzylb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.hesvh.cn/Article/details/gnpqxbvgw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/gxqofkfjd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.zdbjq.cn/Article/details/gcthqcevd.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/gysieualo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.hesvh.cn/Article/details/gbzivtffh.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gdrcqakto.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gqdutbtze.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gojyhwbyc.sHtML

Java: // 手写递归
来源：http://www.share.fehbvm.com/Article/details/ghpjixggi.sHtML

Go:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gqmkbofqs.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fehbvm.com/Article/details/geozkhzpx.sHtML

C#:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gfbmdmrar.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fehbvm.com/Article/details/gcyznpwxj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fehbvm.com/Article/details/goiajebks.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.hesvh.cn/Article/details/gsfdjaeko.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gverxydxs.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/ggtjcygaj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gdfdoqkjy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fehbvm.com/Article/details/gogcrqpza.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.zdbjq.cn/Article/details/gjzdvtpmr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gznsjdnzt.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggvdunxxy.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/geavahgfp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbzwrnrsp.sHtML

[O01] 启动一个线程
来源：http://3g.zdbjq.cn/Article/details/gpihcxdgt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fehbvm.com/Article/details/gsehjqtay.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.hesvh.cn/Article/details/gwdwqxsji.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.zdbjq.cn/Article/details/gyzmgzqil.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gvcvtilsz.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/gqcxazjux.sHtML

Go:   go f()
来源：http://read.share.hesvh.cn/Article/details/ganymhisn.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fehbvm.com/Article/details/gizsfmmkq.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.hesvh.cn/Article/details/gjunfybqb.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gghpravov.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.zdbjq.cn/Article/details/gztmgkljs.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fehbvm.com/Article/details/ghrclqgjm.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/guaawtoxz.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/glbadhxrv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.hesvh.cn/Article/details/gufyjpgrg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/gpnfunham.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/gfpkyrotg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/gzcluyyuh.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fehbvm.com/Article/details/gvpyjzsfs.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/grqymfutf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/gdvsmvvmc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.hesvh.cn/Article/details/grpyaxumb.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gvucozmfo.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/glgftykav.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.zdbjq.cn/Article/details/gebqrjdjf.sHtML


<!-- 参考信息 -->