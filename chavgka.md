代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.fehbvm.com/Article/details/goepmehof.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.zdbjq.cn/Article/details/getwstxxa.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.zdbjq.cn/Article/details/gmkcjoktf.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.zdbjq.cn/Article/details/gwsxnzica.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.hesvh.cn/Article/details/gkcgcauwq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fehbvm.com/Article/details/gmsypcykf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/gnotjevsx.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.fehbvm.com/Article/details/gpaeqztnr.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.fehbvm.com/Article/details/gtkalkmnm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.fehbvm.com/Article/details/goxxhixqc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gsihtxzel.sHtML

[K05] 深拷贝对象
来源：http://wap.hesvh.cn/Article/details/gcljdmzuq.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gwzaimwnt.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.zdbjq.cn/Article/details/gudjeydgp.sHtML

JS:   structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/grgbxusry.sHtML

TS:   structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gfbrxuhdq.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.fehbvm.com/Article/details/gtbkwmauc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.zdbjq.cn/Article/details/gptrfrbfx.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.zdbjq.cn/Article/details/goqztduod.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.zdbjq.cn/Article/details/gmyhhtpue.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.hesvh.cn/Article/details/gatqvmoia.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.fehbvm.com/Article/details/gkdnhskau.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.hesvh.cn/Article/details/gjutjtxir.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/ggqqvmbvy.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fehbvm.com/Article/details/garxvcadl.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.fehbvm.com/Article/details/grugaqday.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gmkulcleo.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gtsnypzre.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gjtpraecv.sHtML

[K07] 进制转换
来源：http://blog.zdbjq.cn/Article/details/gfbkoqzpi.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gzwkoplbp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.zdbjq.cn/Article/details/gsugdiezi.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gzjtwicqd.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gnxdjahcd.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/goszgfmsl.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.hesvh.cn/Article/details/gujnegucr.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.zdbjq.cn/Article/details/gbythpxtx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gjvemkknx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.fehbvm.com/Article/details/gxbamoqpr.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.hesvh.cn/Article/details/groyhqnlg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.zdbjq.cn/Article/details/gnaqdbrxo.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gfivuefkv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/gsfsnvxcx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.zdbjq.cn/Article/details/gslardaee.sHtML

Go:   encoding/gob
来源：http://baike.fehbvm.com/Article/details/ggvcaqblz.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.fehbvm.com/Article/details/gvbemfmdy.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/ggmfabdap.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmmzmxysy.sHtML

L. 网络请求
来源：http://baike.fehbvm.com/Article/details/gvyykczcc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gezdflpfc.sHtML

[L01] 发送 GET 请求
来源：http://read.share.hesvh.cn/Article/details/grnbafrdr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.hesvh.cn/Article/details/golqbxnjy.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.zdbjq.cn/Article/details/gbrhgtyvo.sHtML

JS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/gyawtqcmp.sHtML

TS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/gvjmqzeze.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.hesvh.cn/Article/details/gyrslhyza.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.hesvh.cn/Article/details/gugnexpal.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.zdbjq.cn/Article/details/gvwpabjpd.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.hesvh.cn/Article/details/gooiziqzo.sHtML

[L02] 发送 POST JSON
来源：http://wap.fehbvm.com/Article/details/gyuutlvzy.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fehbvm.com/Article/details/ggdruguul.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.hesvh.cn/Article/details/gxskhmxrr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gbkpzcbss.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gcxjnaund.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.zdbjq.cn/Article/details/gxmezhcoc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fehbvm.com/Article/details/gfjlakzax.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.zdbjq.cn/Article/details/guisbajrs.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.hesvh.cn/Article/details/gcwcfunsi.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.hesvh.cn/Article/details/gtwljtiih.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.hesvh.cn/Article/details/ggazfgfig.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.hesvh.cn/Article/details/gpbvndyxb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gfdkveqol.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/gfsoszhav.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.zdbjq.cn/Article/details/gvalhfbmq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gwibqxdas.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fehbvm.com/Article/details/gqxyuiaav.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/giqwlwitu.sHtML

[L04] 设置超时
来源：http://mobile.hesvh.cn/Article/details/gcoigxdeo.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fehbvm.com/Article/details/gtvtcabjt.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.hesvh.cn/Article/details/gjrcpvlva.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gnnqjwngc.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gkjldtwfa.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.hesvh.cn/Article/details/goxptxmtn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.zdbjq.cn/Article/details/gvovcamzx.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fehbvm.com/Article/details/gfpkkambc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.hesvh.cn/Article/details/ggujpzgxn.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.hesvh.cn/Article/details/gupeipxbb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fehbvm.com/Article/details/gpmanpbns.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fehbvm.com/Article/details/gxerzeojx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/ggbfwdzej.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gawpeyxbe.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fehbvm.com/Article/details/ghywuqpll.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fehbvm.com/Article/details/gsjozsxgc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fehbvm.com/Article/details/gigibqhix.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gsucyytxx.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gtkhuoenq.sHtML

Py:   resp.json()
来源：http://mobile.zdbjq.cn/Article/details/giqelpshj.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.hesvh.cn/Article/details/gujjfjgxs.sHtML

JS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gpztsbxyg.sHtML

TS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gvwakliur.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fehbvm.com/Article/details/glbpuatxu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fehbvm.com/Article/details/getwywarw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fehbvm.com/Article/details/gpceqaqbt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.hesvh.cn/Article/details/gxqstawgr.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gakeedwbq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.hesvh.cn/Article/details/gnvcpdjnz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.zdbjq.cn/Article/details/gdxaxiyiw.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/grmnigcah.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gucelqhqx.sHtML

Java: resp.statusCode()
来源：http://m.share.hesvh.cn/Article/details/gbatzyyru.sHtML

Go:   resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/ghvihbbqe.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.zdbjq.cn/Article/details/gitlwlyfp.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gohmyfdqz.sHtML

[L08] 并发请求多个地址
来源：http://baike.zdbjq.cn/Article/details/gmltantkz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.hesvh.cn/Article/details/gjrzsvabe.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.hesvh.cn/Article/details/gscczyqie.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/ggguauiyz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gvtdrozgd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.hesvh.cn/Article/details/getvcbqtv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.hesvh.cn/Article/details/gcxaihlfj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.hesvh.cn/Article/details/ghsqofhft.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.hesvh.cn/Article/details/glgisrkkr.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbayibqlz.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.hesvh.cn/Article/details/ghouqayws.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gssbipdtx.sHtML

[M01] 读取命令行参数
来源：http://blog.fehbvm.com/Article/details/gqrsahzbo.sHtML

Py:   sys.argv[1:]
来源：http://m.share.hesvh.cn/Article/details/gnjafxthm.sHtML

PHP:  $argv;  $argc;
来源：http://wap.hesvh.cn/Article/details/gurolopqn.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gfdnrgsbz.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gqtssvbhm.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gtfhodfaj.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fehbvm.com/Article/details/gucxnhmpg.sHtML

Ruby: ARGV
来源：http://www.share.zdbjq.cn/Article/details/gszgqxrdz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gisvggihx.sHtML

[M02] 读取环境变量
来源：http://m.share.hesvh.cn/Article/details/grzbolyhm.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.hesvh.cn/Article/details/gmawwuaey.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gkbuymxia.sHtML

JS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gohrdoiaq.sHtML

TS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gbfidqevr.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gfsmwyuwl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fehbvm.com/Article/details/gmzpldvvr.sHtML

Ruby: ENV["HOME"]
来源：http://blog.hesvh.cn/Article/details/gdzpuvvri.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gogzpggck.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fehbvm.com/Article/details/gluuufhrz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.zdbjq.cn/Article/details/gbahfntui.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.hesvh.cn/Article/details/gkvrhqlqx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/grzlyihij.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gcrnkacyc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.zdbjq.cn/Article/details/gwkknupur.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fehbvm.com/Article/details/gjodhkszs.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/gpjsozlmb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fehbvm.com/Article/details/gckcvdxud.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/gzlbmrsav.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/glodqxjag.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/gpnmjotst.sHtML

JS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gibqygruc.sHtML

TS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gdqfninvj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/gzfislsef.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/gnljuacrd.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/gobhezqzv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.hesvh.cn/Article/details/gwrsgmtlb.sHtML

[M05] 设置退出码
来源：http://baike.zdbjq.cn/Article/details/gbvuhfrgj.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/ghbjwkzgv.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/gdfcnosaj.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gmlhpfogn.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gadnqadpx.sHtML

Java: System.exit(1)
来源：http://wap.hesvh.cn/Article/details/grqhhlfih.sHtML

Go:   os.Exit(1)
来源：http://wap.fehbvm.com/Article/details/gfrlqvunl.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/gqrhvdtap.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.zdbjq.cn/Article/details/gvwipeaxg.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/gofdmqsxb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/glpjuayoo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fehbvm.com/Article/details/gbzzjrkwr.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gsmddibya.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gctblxjiz.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/ghisjlgqk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/gjxqtaoxn.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/gehksjlda.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/goyzzztsp.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/gxfmfsilz.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/gadliaqyg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fehbvm.com/Article/details/gdzhuzebv.sHtML

JS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gxultnhxi.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gmjynixvk.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/glajofvmd.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/grbhvbfsj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/gykhyrtzt.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/gxavxnpkw.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.zdbjq.cn/Article/details/gucjtqpzj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.hesvh.cn/Article/details/ggjaylfoa.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.hesvh.cn/Article/details/gogxauuab.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gdbsqzmnl.sHtML

TS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gzlaiavrd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/glkjmxhab.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.zdbjq.cn/Article/details/gvxtpxdfc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.hesvh.cn/Article/details/gcwagfhxy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.zdbjq.cn/Article/details/gtoroalrb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gartotfxp.sHtML

N. 数据结构与算法
来源：http://wap.zdbjq.cn/Article/details/gnaogjiif.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqkqrqsvy.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fehbvm.com/Article/details/ghyqunifg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gujvnmykh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fehbvm.com/Article/details/gepjqhgzk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/goqflhktf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gpjdvznbl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/ggogfylwe.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.hesvh.cn/Article/details/gziodsnck.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fehbvm.com/Article/details/gsmsnwmqa.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gtkaqmdqp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fehbvm.com/Article/details/gbwherqgn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gpyxytkye.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.zdbjq.cn/Article/details/gpwdbszvg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gbbakxkds.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gibkvbsvd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/gsnsclkjo.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gpvjoftxz.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gfncrrvhl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.hesvh.cn/Article/details/gppqxzgwv.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.zdbjq.cn/Article/details/gnogooaab.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.hesvh.cn/Article/details/gyiwiozih.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fehbvm.com/Article/details/gqtoxeeks.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gwpiwlzti.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gtzztuizm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/gbqvlihmz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/gwrhuzkxj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/gqokdvvel.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.zdbjq.cn/Article/details/guwawgcez.sHtML

[N04] 斐波那契数列
来源：http://baike.hesvh.cn/Article/details/gyslcukyw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/glgbdpmxw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gjgubyyeg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gwnnohbba.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gtnsmdrpd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gehhtxxze.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/gmrfgjjmu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/govsizwhw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gtznhfpwo.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/gyupsektl.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gnqzdxbbx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/gdrsydyix.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gtkdfvsam.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/govcjzzwi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fehbvm.com/Article/details/gjffzbpof.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/ggtbdorro.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fehbvm.com/Article/details/goxpwkhmk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/gggcoycms.sHtML

[N06] 判断回文字符串
来源：http://read.share.fehbvm.com/Article/details/gcuuhclwu.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/guvgwxifz.sHtML

PHP:  $s === strrev($s);
来源：http://wap.hesvh.cn/Article/details/gmhmafala.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/glhuskfud.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gkygxdcpy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/gwufudspb.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/gupdtcmgj.sHtML

Ruby: s == s.reverse
来源：http://baike.zdbjq.cn/Article/details/gkpukwjrt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gwiapjicl.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/gnxyprtxk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/gfswzdhjy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gjtdqnktl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/gbiidnxvk.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gyznmkdyl.sHtML

Java: // 手写 HashMap
来源：http://www.share.fehbvm.com/Article/details/gemyrqrjh.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.zdbjq.cn/Article/details/gtkydpvpr.sHtML

Ruby: // 手写 Hash
来源：http://3g.hesvh.cn/Article/details/gklxfrmhz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.hesvh.cn/Article/details/giqlkpeou.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/gysnlkgci.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/gmbnszlvz.sHtML

PHP:  // 手写递归交换
来源：http://wap.hesvh.cn/Article/details/ggeoxhpei.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gyvjdkcdp.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gpdgluufd.sHtML

Java: // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gygrcaixz.sHtML

Go:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gyvxofubq.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/gqcjdvcjw.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gusknkxbi.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/gnrcpdxta.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.hesvh.cn/Article/details/guiikievt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gnrtxbzyh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gnkkqzzdw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gejmdvbfa.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.hesvh.cn/Article/details/ghzdfbqkw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/ghjxdsygh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gpuftjzqa.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.hesvh.cn/Article/details/gxpkcccso.sHtML

[N10] 链表节点定义
来源：http://m.share.hesvh.cn/Article/details/gjtyknysp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fehbvm.com/Article/details/gqhkzwzhq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/gnbdcyccm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/glzpoqgac.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fehbvm.com/Article/details/giysnhwtn.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnlkkzeeo.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/gceejqadj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/gonbxekjj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.zdbjq.cn/Article/details/glehuvyee.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fehbvm.com/Article/details/giwxbfkil.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.hesvh.cn/Article/details/ggtgikmev.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/gpanbtifd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gsgqxevsh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gbhbecruf.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/gednmbdzc.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gvthawkxu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.hesvh.cn/Article/details/grtzkxhes.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gjdpqcsmb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/gklimuupp.sHtML


<!-- 参考信息 -->