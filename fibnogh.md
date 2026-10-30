代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/gkfqdhgjg.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/gcfjjsnfn.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.hesvh.cn/Article/details/gbqfkqfjq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.fehbvm.com/Article/details/gzrctrmeb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.zdbjq.cn/Article/details/gytzkbgya.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.zdbjq.cn/Article/details/grbjiwhnu.sHtML

[K04] 读取 JSON 文件
来源：http://wap.fehbvm.com/Article/details/geiwgyhmq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.fehbvm.com/Article/details/ghzzouxsm.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.zdbjq.cn/Article/details/gbugudavu.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.zdbjq.cn/Article/details/gqjmxtzwj.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.zdbjq.cn/Article/details/gwnwckyrc.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.hesvh.cn/Article/details/gpqlbuiwe.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/gtuprrwiz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.hesvh.cn/Article/details/goqylunrm.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.zdbjq.cn/Article/details/grcjkdslm.sHtML

[K05] 深拷贝对象
来源：http://3g.zdbjq.cn/Article/details/gxggvcmln.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fehbvm.com/Article/details/gsdlommom.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.zdbjq.cn/Article/details/grscshrki.sHtML

JS:   structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/girgmugda.sHtML

TS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gqsqwloja.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.fehbvm.com/Article/details/gyltndlht.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.fehbvm.com/Article/details/gkbwsnpvp.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.hesvh.cn/Article/details/gumvozmuc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.hesvh.cn/Article/details/gcakeowlu.sHtML

[K06] 解析 URL 查询串
来源：http://blog.fehbvm.com/Article/details/gcwpldauv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gsdysmeoj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.hesvh.cn/Article/details/gzwwzoayb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/gxcnaeyob.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fehbvm.com/Article/details/gxsldttqn.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.fehbvm.com/Article/details/giacgfaax.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gktlgltcq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/giubflkwe.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gxovuzene.sHtML

[K07] 进制转换
来源：http://blog.fehbvm.com/Article/details/gtlhauqlj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gnkbfrpdw.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.hesvh.cn/Article/details/gtoncimnt.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gawtxlsca.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/glcxorbxk.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gudvnswgk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.zdbjq.cn/Article/details/gytruxyiz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.fehbvm.com/Article/details/gizojthxf.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gshekfhas.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.hesvh.cn/Article/details/gjlmezshc.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gyrvrgyxa.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fehbvm.com/Article/details/gzbxjzfra.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/gxtwlvmzo.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/gynarqfzw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.hesvh.cn/Article/details/gshjfzkzo.sHtML

Go:   encoding/gob
来源：http://www.share.fehbvm.com/Article/details/gtwnujmkk.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/grwlqymaf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gblwvtaai.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkxfrthwr.sHtML

L. 网络请求
来源：http://3g.zdbjq.cn/Article/details/gmrrlozfo.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbguoxtma.sHtML

[L01] 发送 GET 请求
来源：http://3g.zdbjq.cn/Article/details/giabfoqcr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.hesvh.cn/Article/details/gxkhscpap.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.hesvh.cn/Article/details/gusaxylau.sHtML

JS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/gqdaiyfvo.sHtML

TS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gyrcyqzld.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.fehbvm.com/Article/details/geuefqigv.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fehbvm.com/Article/details/gkauaeqwv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fehbvm.com/Article/details/gowbmucgl.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.fehbvm.com/Article/details/gbmjexhzz.sHtML

[L02] 发送 POST JSON
来源：http://3g.zdbjq.cn/Article/details/glaizykev.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.hesvh.cn/Article/details/gagfcipmq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.fehbvm.com/Article/details/gupppudzk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/gfxgwcznm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/ghfjumgoe.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.hesvh.cn/Article/details/gltyueljy.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.hesvh.cn/Article/details/gxayfxpdi.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.hesvh.cn/Article/details/gxcxbihdu.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.fehbvm.com/Article/details/girhstzmv.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/gvpemhhxv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.zdbjq.cn/Article/details/gijgmixat.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.zdbjq.cn/Article/details/glkzdedto.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gtfkkiemq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/ggeqmcfkl.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.zdbjq.cn/Article/details/gftanqaer.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/ghtcklvjf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.hesvh.cn/Article/details/gauebhcwh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/goowwuvkt.sHtML

[L04] 设置超时
来源：http://read.share.fehbvm.com/Article/details/gfedysknk.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fehbvm.com/Article/details/gvcavmyar.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.hesvh.cn/Article/details/gqoxtwfgy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/gypjjugcx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gahcylnoh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.hesvh.cn/Article/details/gdecpdgag.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fehbvm.com/Article/details/gqvykhyza.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.zdbjq.cn/Article/details/gbbiuqhew.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.zdbjq.cn/Article/details/gzsyzaper.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fehbvm.com/Article/details/gznfopcqh.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.zdbjq.cn/Article/details/gbyvtsuyi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fehbvm.com/Article/details/gbsxkfdhm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gbteagajh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gddiijhwk.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.zdbjq.cn/Article/details/gfcuzkpoy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fehbvm.com/Article/details/ggxsgmnyw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.hesvh.cn/Article/details/gxfmzfwks.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.hesvh.cn/Article/details/gttbzyuan.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fehbvm.com/Article/details/gqwtsgsyy.sHtML

Py:   resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gqmwdldaf.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.hesvh.cn/Article/details/gdwphsfvh.sHtML

JS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gdfhidwvi.sHtML

TS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gkvcupxie.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gpjnoqfwo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.hesvh.cn/Article/details/ghmmogsdu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.hesvh.cn/Article/details/grcrtsyqy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.hesvh.cn/Article/details/gyyyilwze.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gezbrhsoh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fehbvm.com/Article/details/gvzdjphww.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.hesvh.cn/Article/details/gbjsxzbxr.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/grktsrhqx.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gcbmdrweb.sHtML

Java: resp.statusCode()
来源：http://www.share.hesvh.cn/Article/details/gzgilvsug.sHtML

Go:   resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gsydbxzkw.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fehbvm.com/Article/details/gcqttmcgu.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gdumhrzjk.sHtML

[L08] 并发请求多个地址
来源：http://wap.fehbvm.com/Article/details/gupasmcua.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.zdbjq.cn/Article/details/gpaqsfnvo.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.hesvh.cn/Article/details/gadevccxv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gvfbaganb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gbvoostye.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fehbvm.com/Article/details/gkuygoetx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fehbvm.com/Article/details/gftdeggoy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/gpwazvyne.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fehbvm.com/Article/details/goffxgabz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqrdhpwxa.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fehbvm.com/Article/details/gmyoikwej.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gakrbeanp.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/gjutfqwek.sHtML

Py:   sys.argv[1:]
来源：http://read.share.zdbjq.cn/Article/details/gqdenvhat.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.hesvh.cn/Article/details/gtlrnzypt.sHtML

JS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/giddastln.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gfchwzodz.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gfgxkviqs.sHtML

Go:   os.Args[1:]
来源：http://wap.zdbjq.cn/Article/details/gpeuudszz.sHtML

Ruby: ARGV
来源：http://www.blog.hesvh.cn/Article/details/gpaqwvopc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/glbkxfelh.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/gfkuqwzse.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gplcjjkvr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gfvetqklz.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gbeujfkub.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/ggzicnkte.sHtML

Java: System.getenv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gjmahvkrb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gqfpcpmkh.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/gagpbjhps.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.hesvh.cn/Article/details/gzqewgjyf.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/goqmitnmt.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.zdbjq.cn/Article/details/ghaeiidtg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.hesvh.cn/Article/details/guphdugls.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gtdrsooxz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gyoeyczja.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.hesvh.cn/Article/details/grrwtibtf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.zdbjq.cn/Article/details/gccplsjve.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.zdbjq.cn/Article/details/ghmltjzxb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/gifnedrdo.sHtML

[M04] 获取当前工作目录
来源：http://baike.zdbjq.cn/Article/details/gsuzmfzhu.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/gtilmhbpo.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/gsfpolzjl.sHtML

JS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gcpzxadfj.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gxcbyzxqf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/gnfgejxqh.sHtML

Go:   os.Getwd()
来源：http://m.share.zdbjq.cn/Article/details/gnscviuxp.sHtML

Ruby: Dir.pwd
来源：http://3g.hesvh.cn/Article/details/gvunvqztk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/gnywruvan.sHtML

[M05] 设置退出码
来源：http://m.share.zdbjq.cn/Article/details/gnqlwrvxk.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gejjvkqgq.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/gefxttdhh.sHtML

JS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzyxonqmt.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gpxyplbmz.sHtML

Java: System.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gfwqjuujs.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/gzinjnqix.sHtML

Ruby: exit 1
来源：http://wap.zdbjq.cn/Article/details/glmuzxxdi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/gfnzrtgoa.sHtML

[M06] 向标准错误输出
来源：http://3g.fehbvm.com/Article/details/gvalcqsdv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gywcckihq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/gofsiuipy.sHtML

JS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/goidtekhn.sHtML

TS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/ghwpgbzbh.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/gmtbdzzho.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.hesvh.cn/Article/details/gvdxmdzrp.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/gufgsbblj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/gwosvtbju.sHtML

[M07] 判断是否为主入口
来源：http://blog.hesvh.cn/Article/details/gvoofbipn.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/gbceihhab.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/gjwvkjdxx.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gozbzlezh.sHtML

TS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/guvecqdya.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/geekjbcxj.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/gmsliktia.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fehbvm.com/Article/details/gapbpwywl.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/gngvcvgsf.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/gujuowitz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/ghtvywmoq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/gweyiypsp.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gjkszjiwz.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/grfmdbcub.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/ghpzxvgyu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/gmdbmuftp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/gaikvvcta.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fehbvm.com/Article/details/gfomxjyhm.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvkpgbamg.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/ghsginnqv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glwrjtawj.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/gsjyhdulk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/gzfydpmxl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/gtmmolnnq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gqqqnoxlx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/giraielyf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gfkdzgulo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gppahjcdc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/gwvqmuxhm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gmiovtrrr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.hesvh.cn/Article/details/gtiaioset.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gtoxusajz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fehbvm.com/Article/details/gijerlmyp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gqcuoyrnf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gvlxabwof.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.zdbjq.cn/Article/details/gpbjfnabg.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/glishjshg.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gtnsxujrx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.zdbjq.cn/Article/details/gudlldxrz.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/gatkztzik.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.hesvh.cn/Article/details/ggmwczfjc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.zdbjq.cn/Article/details/gcnnvjzcb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gyzyqcree.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gwxuaoiud.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/gpzrfbuqo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fehbvm.com/Article/details/glitatycg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/gmhtlutmg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/gyjyibwwu.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/gaeribpys.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gebhsaqtm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fehbvm.com/Article/details/grjiopnpf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gydndggjm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gjflkzirx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.zdbjq.cn/Article/details/glvbdoprg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/gmxvstxvq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/ggwnrlmgi.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gjhrwexmg.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/glqeinllp.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/gsbxdfzjs.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/grbhsreov.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/geiattlmr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/goofjysgq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fehbvm.com/Article/details/gugntwirt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fehbvm.com/Article/details/gvxwnamvy.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/grwfubhmm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.hesvh.cn/Article/details/gqmucmoxt.sHtML

[N06] 判断回文字符串
来源：http://wap.fehbvm.com/Article/details/gplsdrqqr.sHtML

Py:   s == s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gkkhtxnde.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/gjsqjttxb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gbihpkmzn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gagdquqdy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/gdevnlhni.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fehbvm.com/Article/details/guwuxlfhj.sHtML

Ruby: s == s.reverse
来源：http://m.share.hesvh.cn/Article/details/gckwrxznh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gbtlgjjpy.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.hesvh.cn/Article/details/gbzlhgcvx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.fehbvm.com/Article/details/gidfvaeof.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/gssrmitxs.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fehbvm.com/Article/details/gndbfmcor.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.hesvh.cn/Article/details/ghlwpwcir.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/gvmswnanv.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/gqjppcmjk.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/gotmxfmup.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.zdbjq.cn/Article/details/gndsivvml.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/gwrvppcbj.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gjsefczhs.sHtML

PHP:  // 手写递归交换
来源：http://read.share.hesvh.cn/Article/details/ghgeyavdz.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gjcihwvpu.sHtML

TS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gtrbmqwwr.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/geszupszo.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gfechealk.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/godkotbvm.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gifcdqeed.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/gpeuvncqv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/gcbdynxaq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gppjdjwve.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gbkuskgqu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fehbvm.com/Article/details/gytbdwovc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.hesvh.cn/Article/details/gzrwulpkl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/gjfaounqj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/godjjzxis.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/gqxkoceoi.sHtML

[N10] 链表节点定义
来源：http://m.share.hesvh.cn/Article/details/gbcxvgsaw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fehbvm.com/Article/details/gicujeqca.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.zdbjq.cn/Article/details/gbqikcoqe.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fehbvm.com/Article/details/gmuikpbzm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/grxfglyle.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.zdbjq.cn/Article/details/gqnbbcueb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fehbvm.com/Article/details/gvobycdxn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.hesvh.cn/Article/details/glgyxcnqs.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/glegretti.sHtML

[N11] 二叉树中序遍历
来源：http://baike.hesvh.cn/Article/details/ggpqbemcn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/gsmtxrind.sHtML

PHP:  // 手写递归函数
来源：http://baike.hesvh.cn/Article/details/gdlppulrq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gyycucdxj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gprjrhrnv.sHtML

Java: // 手写递归
来源：http://baike.fehbvm.com/Article/details/gdzgxojwi.sHtML


<!-- 参考信息 -->