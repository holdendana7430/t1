代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.zdbjq.cn/Article/details/gtdbxzvtm.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gggkajhgr.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.fehbvm.com/Article/details/gnlpuavpx.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.fehbvm.com/Article/details/gieocatxo.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.hesvh.cn/Article/details/ggdxhhuvt.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/gjkkmtptq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/grvtagyix.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.hesvh.cn/Article/details/grpvaaifb.sHtML

Go:   encoding/gob
来源：http://3g.zdbjq.cn/Article/details/groqrhwuv.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fehbvm.com/Article/details/ggefvhlce.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gltlretzn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghfsbxsge.sHtML

L. 网络请求
来源：http://read.share.hesvh.cn/Article/details/ganduraif.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gltjemqpv.sHtML

[L01] 发送 GET 请求
来源：http://baike.hesvh.cn/Article/details/gxrppwcdn.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.fehbvm.com/Article/details/grmjkihjz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.fehbvm.com/Article/details/gclzbirad.sHtML

JS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gvxoznuaf.sHtML

TS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gtjydhybt.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.hesvh.cn/Article/details/gsuyluohs.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.hesvh.cn/Article/details/gjlxxltxq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.zdbjq.cn/Article/details/gtohhshwn.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.zdbjq.cn/Article/details/gxexjqngo.sHtML

[L02] 发送 POST JSON
来源：http://wap.fehbvm.com/Article/details/gksqfvzge.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.hesvh.cn/Article/details/gfugjfaql.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.zdbjq.cn/Article/details/gdujxhcgo.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/gqzzomfbk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/grmienpwy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.hesvh.cn/Article/details/gdqlwsmzq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.hesvh.cn/Article/details/gtiotknxy.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.zdbjq.cn/Article/details/gaomfdzzu.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.zdbjq.cn/Article/details/ggqxuurpa.sHtML

[L03] 设置自定义请求头
来源：http://3g.hesvh.cn/Article/details/ggijmhfhv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.hesvh.cn/Article/details/gzxxztpbw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.zdbjq.cn/Article/details/gtmhlmlkc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gmjbpdbub.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gwqvbprun.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.hesvh.cn/Article/details/glqzgjwst.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gfdngyrxy.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.fehbvm.com/Article/details/gyflmyhnj.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/glifvycqg.sHtML

[L04] 设置超时
来源：http://www.share.hesvh.cn/Article/details/godiminsy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fehbvm.com/Article/details/gdkxmuilu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.zdbjq.cn/Article/details/gpjobomns.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/geudbmsch.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gmoulebsi.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.zdbjq.cn/Article/details/gqxtminmg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.zdbjq.cn/Article/details/gmlpbbjwz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/gwrzbktiz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.hesvh.cn/Article/details/gvkrrseou.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.hesvh.cn/Article/details/gdeaionar.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.hesvh.cn/Article/details/gmtcoewhb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.zdbjq.cn/Article/details/gxmjiguhr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gikbdcgtv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gofwwfhcl.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fehbvm.com/Article/details/gwbnqvalx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.hesvh.cn/Article/details/gjyefugfj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.zdbjq.cn/Article/details/grsaifbtw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gufpmvfug.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.hesvh.cn/Article/details/gcpjjwvtb.sHtML

Py:   resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gvwqqjmil.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.zdbjq.cn/Article/details/gvidfxsyq.sHtML

JS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gylwfahbt.sHtML

TS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/goeqyvvas.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.hesvh.cn/Article/details/gznpnabuu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fehbvm.com/Article/details/gbusxdubi.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.hesvh.cn/Article/details/gtmpxysws.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fehbvm.com/Article/details/gspxmzimb.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/ggxszfztt.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.zdbjq.cn/Article/details/gtlopibfl.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fehbvm.com/Article/details/gqtjaorjf.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gmbwdskdl.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/ginywhyvc.sHtML

Java: resp.statusCode()
来源：http://www.share.fehbvm.com/Article/details/gutbkgrfx.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gfpicafza.sHtML

Ruby: resp.code.to_i
来源：http://wap.fehbvm.com/Article/details/glkzqtzsz.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/getwcclqq.sHtML

[L08] 并发请求多个地址
来源：http://mobile.fehbvm.com/Article/details/gktlpxnle.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.hesvh.cn/Article/details/gnwjltypc.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fehbvm.com/Article/details/gcfvqnvfo.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/ggqabmurj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gqavqdfjg.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fehbvm.com/Article/details/geudjoqde.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.hesvh.cn/Article/details/gqhazjkal.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.hesvh.cn/Article/details/godnqkorz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/gksdixnlp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gexogakir.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.hesvh.cn/Article/details/gzwqkgfpm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkvnwrbhk.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/guvpqlvmx.sHtML

Py:   sys.argv[1:]
来源：http://blog.hesvh.cn/Article/details/gxeluarqz.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.hesvh.cn/Article/details/gnkkashyr.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gahnckpdr.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gwszgcgab.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fehbvm.com/Article/details/greaqjvgh.sHtML

Go:   os.Args[1:]
来源：http://blog.zdbjq.cn/Article/details/ghwquqmjf.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/glzyqolef.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gcmmwdjwe.sHtML

[M02] 读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gfycjzndi.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gjpppclrv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gzmhwajas.sHtML

JS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gheeldcct.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/grxsnxumq.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gshkojfcu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fehbvm.com/Article/details/gjvoebeko.sHtML

Ruby: ENV["HOME"]
来源：http://baike.hesvh.cn/Article/details/gvuhbxrat.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/gnkwchcbk.sHtML

[M03] 执行外部命令
来源：http://read.share.hesvh.cn/Article/details/gbrxjkaip.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.zdbjq.cn/Article/details/ghshcaxjs.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.zdbjq.cn/Article/details/gvcyvbjia.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/ghedaxfer.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gjrtzgmis.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.zdbjq.cn/Article/details/gvzhpnjgq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.zdbjq.cn/Article/details/gnuvodjuz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fehbvm.com/Article/details/gjcmfwrwh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.zdbjq.cn/Article/details/gikztuhlh.sHtML

[M04] 获取当前工作目录
来源：http://m.share.hesvh.cn/Article/details/gswdiozgk.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/gzrahpsbt.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/gtbivtbin.sHtML

JS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gdzjchxae.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gipzcrwtv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/gvojhjyub.sHtML

Go:   os.Getwd()
来源：http://baike.hesvh.cn/Article/details/gbxromohb.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.hesvh.cn/Article/details/globaefrg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/gzxloxrat.sHtML

[M05] 设置退出码
来源：http://baike.hesvh.cn/Article/details/gzvpkikbd.sHtML

Py:   sys.exit(1)
来源：http://m.share.fehbvm.com/Article/details/guqmrjeav.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/ggpirolbw.sHtML

JS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gplabdlng.sHtML

TS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gqqidmcgm.sHtML

Java: System.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gwvxzdiyq.sHtML

Go:   os.Exit(1)
来源：http://www.share.hesvh.cn/Article/details/gzldpefhc.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/gcmynkvno.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.hesvh.cn/Article/details/gyznbmqbi.sHtML

[M06] 向标准错误输出
来源：http://mobile.fehbvm.com/Article/details/gwpbfanwj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gwnjiyjhs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/glomyfvrx.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/ghcmfakil.sHtML

TS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gmrqhlnqf.sHtML

Java: System.err.println("err")
来源：http://3g.zdbjq.cn/Article/details/ggqxkpvzw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/gohuurjoj.sHtML

Ruby: warn "err"
来源：http://www.m.share.fehbvm.com/Article/details/ghiyxqqom.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.zdbjq.cn/Article/details/glzzmcisc.sHtML

[M07] 判断是否为主入口
来源：http://3g.fehbvm.com/Article/details/geykleerq.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fehbvm.com/Article/details/gcwpwisgy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.zdbjq.cn/Article/details/gnmgrwtpq.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gvdzcqdoz.sHtML

TS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gjhxpvxwe.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/gnqixquku.sHtML

Go:   func main()
来源：http://www.share.zdbjq.cn/Article/details/gvtbhnrzj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.zdbjq.cn/Article/details/gykbigvnd.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/geizflgjg.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.zdbjq.cn/Article/details/goxwxblrb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/giemngiqf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/golvwlufa.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gclnrnhxp.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gwcjnawrv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fehbvm.com/Article/details/gdmdrfmhx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/gqvmrgecy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fehbvm.com/Article/details/gxkcogjol.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fehbvm.com/Article/details/giiacprpr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggqdjriaa.sHtML

N. 数据结构与算法
来源：http://www.blog.zdbjq.cn/Article/details/gshbgrmjr.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmoesxgln.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fehbvm.com/Article/details/gnhvanmvs.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gawzrszjd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.zdbjq.cn/Article/details/gxetqivxb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/ggvfghrmb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gxvriqlfm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gsszhrqvt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gumutjxne.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.hesvh.cn/Article/details/gjhedrcgn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gmyppyiqj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/gdpdwasid.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/grxswmxrq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/gypblqzai.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gonwhpkba.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gmlktbxwt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.zdbjq.cn/Article/details/gvjwohpec.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gpjfedpfr.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gurrypcjj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gziaprkmg.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/gcdvrsnro.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/gnixfjapl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/gcfdhngeu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gwaamrojt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gexceplxc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.zdbjq.cn/Article/details/gimufsbum.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/gelatvknf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.hesvh.cn/Article/details/guqagvbyt.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/gcxjpujbb.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.zdbjq.cn/Article/details/gwdsqpnfy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gmwrpqmbj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/glprfdnzm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gbsopemzh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gknnvtizd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/groiizspl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.zdbjq.cn/Article/details/gnkhfppll.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gjuxjgboi.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gkwoyqrnw.sHtML

[N05] 最大公约数
来源：http://baike.fehbvm.com/Article/details/gebhmchnr.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/gfhltzidr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/glidkrjln.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gxbqwymoc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gtteztyuz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/gkyifsrmp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.zdbjq.cn/Article/details/gtduaynst.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fehbvm.com/Article/details/gtcldxlmn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/gbyedvata.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/ggkujmlnq.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gvtbppzvg.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gfrqdqdgt.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gmpdhdcvw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gqnjclsyj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fehbvm.com/Article/details/gjakedfop.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fehbvm.com/Article/details/gwjcpptqz.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/gtnqpgmiy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gckuzyquu.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fehbvm.com/Article/details/gjhihrhrs.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.zdbjq.cn/Article/details/ggwuxsyqw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/guepdfrqs.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/gbxznpfqi.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/gnnokgjry.sHtML

Java: // 手写 HashMap
来源：http://www.blog.hesvh.cn/Article/details/gyqnhdoyf.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fehbvm.com/Article/details/gczyrrfiv.sHtML

Ruby: // 手写 Hash
来源：http://blog.zdbjq.cn/Article/details/gtrjapbxz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.zdbjq.cn/Article/details/gpgbuqopf.sHtML

[N08] 生成全排列
来源：http://mobile.hesvh.cn/Article/details/gwstvywnu.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/gjhjqwibp.sHtML

PHP:  // 手写递归交换
来源：http://www.share.zdbjq.cn/Article/details/gwthjgqeu.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gpgjvgyaj.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gmieuubrz.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/genqlbthi.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gpydsauii.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/gtuxzrwjm.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gwufftrbm.sHtML

[N09] 栈与队列
来源：http://wap.fehbvm.com/Article/details/gifsshfdt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/gvfijgflo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gkqqmkwuz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gxschipqe.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/gvcmwihal.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/gqwnpisld.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.zdbjq.cn/Article/details/gfudeglhw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gwesgagvy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fehbvm.com/Article/details/gjszsxfjv.sHtML

[N10] 链表节点定义
来源：http://m.share.zdbjq.cn/Article/details/gqtvgasfm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fehbvm.com/Article/details/gyoxaotyy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/ghlyibfxx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.zdbjq.cn/Article/details/ggdrnngmg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fehbvm.com/Article/details/gjfemdrpg.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/gatwvgbfv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/gkaixtebm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.hesvh.cn/Article/details/gwflaldry.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.hesvh.cn/Article/details/gssirrlpp.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gfulgeiwd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.hesvh.cn/Article/details/gpbfwkchl.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gcgaslgsc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gcspqpeiq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gjqqgiqyq.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gmtenkbnl.sHtML

Go:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gqfodsash.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/gwbmlohps.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gcjadoikm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/gbletqjmk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.hesvh.cn/Article/details/gbjufnqyd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.zdbjq.cn/Article/details/gpzxqwvmb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/glvhinyne.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gnjmjmmgh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gpfwsczys.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.zdbjq.cn/Article/details/gdqbfwjnb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gekhhqpfz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gsaqrupnf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gylzspwml.sHtML

O. 并发与异步
来源：http://read.share.zdbjq.cn/Article/details/gxyqhlqgx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/goirwzpyr.sHtML

[O01] 启动一个线程
来源：http://3g.zdbjq.cn/Article/details/ghycxrrmi.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.zdbjq.cn/Article/details/gjrkwaoog.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/gmtgezhic.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/gqoyhahlq.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gqgxvmwcb.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/gjcnbkyxq.sHtML

Go:   go f()
来源：http://wap.zdbjq.cn/Article/details/gwpobspfq.sHtML

Ruby: Thread.new { f }
来源：http://blog.fehbvm.com/Article/details/gkwjfxhov.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/goyiatbdu.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/gpnxaftoj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/gvyujezvm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/ghraccnjs.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/godrxygtf.sHtML

TS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gypgbkfxs.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/gqpjwcrzy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fehbvm.com/Article/details/gzwghxfik.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/ggizuvwua.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.zdbjq.cn/Article/details/gpkxvnfdc.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fehbvm.com/Article/details/gwvhbawzn.sHtML

Py:   with lock: shared += 1
来源：http://m.share.hesvh.cn/Article/details/gvqkdqced.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.hesvh.cn/Article/details/glirjshgt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.zdbjq.cn/Article/details/gurrcinvz.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/givpcpvoy.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/ghioqjakg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/gwkozhljc.sHtML


<!-- 参考信息 -->