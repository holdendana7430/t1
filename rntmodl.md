代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fehbvm.com/Article/details/gonblojux.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.hesvh.cn/Article/details/glwhlwjud.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.zdbjq.cn/Article/details/ggyfidntq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.hesvh.cn/Article/details/gfiuvffmx.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.fehbvm.com/Article/details/gafuhaxtd.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.zdbjq.cn/Article/details/gpyduvrhy.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/ggxvosjmj.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/glfrkyjif.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.hesvh.cn/Article/details/gdxazxnpe.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.fehbvm.com/Article/details/gwikiltha.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.zdbjq.cn/Article/details/gwwixbnri.sHtML

[K05] 深拷贝对象
来源：http://read.share.fehbvm.com/Article/details/gzysmdarc.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.hesvh.cn/Article/details/gatzbcicy.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.fehbvm.com/Article/details/gwazhzddf.sHtML

JS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gpflxazct.sHtML

TS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gkuyknehk.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.zdbjq.cn/Article/details/gdiwnyypb.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.zdbjq.cn/Article/details/gutnpompo.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.zdbjq.cn/Article/details/gsxamsuve.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.zdbjq.cn/Article/details/gsedoffio.sHtML

[K06] 解析 URL 查询串
来源：http://baike.zdbjq.cn/Article/details/giehtpzve.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/gyztdofyz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.fehbvm.com/Article/details/gwqmwdjwq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gckhkpbwk.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/gkmohtrks.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.hesvh.cn/Article/details/ggirosohj.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gcduxynrp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gixwtstup.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gizqclouy.sHtML

[K07] 进制转换
来源：http://3g.hesvh.cn/Article/details/gpddexfri.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.fehbvm.com/Article/details/getbneeau.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fehbvm.com/Article/details/geqzevyil.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gbwlbcbkw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/ggwhdecmp.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/giwdyoqry.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.hesvh.cn/Article/details/gvfrgzigx.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fehbvm.com/Article/details/gkodxqezp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gbpmoyymr.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.fehbvm.com/Article/details/grajrkiae.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.zdbjq.cn/Article/details/glalyjolr.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fehbvm.com/Article/details/gztybdlyw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gimznqujt.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gkjdibcaq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.hesvh.cn/Article/details/gfqrftujm.sHtML

Go:   encoding/gob
来源：http://wap.zdbjq.cn/Article/details/gcorhhmju.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.hesvh.cn/Article/details/gucnbsafl.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gndldbtpt.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtevgwriw.sHtML

L. 网络请求
来源：http://www.share.zdbjq.cn/Article/details/gwfhgpzca.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwnrqdrrk.sHtML

[L01] 发送 GET 请求
来源：http://blog.fehbvm.com/Article/details/gnvpwfmum.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.fehbvm.com/Article/details/golxveyej.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.zdbjq.cn/Article/details/gzbxwwmqw.sHtML

JS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gaxhrhnxi.sHtML

TS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/gvegvciki.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.zdbjq.cn/Article/details/gyqjjhwru.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.fehbvm.com/Article/details/gbjjkvyvv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.zdbjq.cn/Article/details/gcejnbfnf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.zdbjq.cn/Article/details/grooldeaa.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gbuttaqum.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/gwchlndyn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.fehbvm.com/Article/details/gztdyqfkt.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/gixstinvm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gmvdnuecy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.hesvh.cn/Article/details/gfecrzati.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.hesvh.cn/Article/details/grtlzsjqo.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.hesvh.cn/Article/details/glqmkamyk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.hesvh.cn/Article/details/gzntgdomz.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/gollpwwav.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fehbvm.com/Article/details/ghvcfboot.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fehbvm.com/Article/details/gmystenfo.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/ghrmlhiin.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gbdbhlmwu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.hesvh.cn/Article/details/ggpttqwhq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/greyyrmus.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.hesvh.cn/Article/details/ggciyypva.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gajdryzep.sHtML

[L04] 设置超时
来源：http://m.share.hesvh.cn/Article/details/gwhgcjlbd.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.zdbjq.cn/Article/details/ghixcmxjt.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.hesvh.cn/Article/details/gayohypfu.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gilqgrnqq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gkovirfer.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.hesvh.cn/Article/details/gzskexnvu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.hesvh.cn/Article/details/gpfmsjwhi.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fehbvm.com/Article/details/golamibxm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.zdbjq.cn/Article/details/getwxzktb.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.hesvh.cn/Article/details/gzcdglyjp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fehbvm.com/Article/details/gjmlknryf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fehbvm.com/Article/details/ggcgbwszr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gnctmidym.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/glebszdvv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.hesvh.cn/Article/details/gsmtlsggl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.zdbjq.cn/Article/details/gzwwxlete.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.zdbjq.cn/Article/details/gggsyctot.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gzazpindt.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fehbvm.com/Article/details/gtuutmjxf.sHtML

Py:   resp.json()
来源：http://baike.zdbjq.cn/Article/details/gelhhdfec.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.zdbjq.cn/Article/details/geutwbdfu.sHtML

JS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gqgpdltir.sHtML

TS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gllbblntq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gcjbdqyhn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fehbvm.com/Article/details/gqrqcfcsm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.hesvh.cn/Article/details/gldeycqys.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.zdbjq.cn/Article/details/gticibpfh.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gqdghsflm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.hesvh.cn/Article/details/gjvdlhkji.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.zdbjq.cn/Article/details/gqstfusep.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gfdacanon.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gfdvqzdfq.sHtML

Java: resp.statusCode()
来源：http://www.share.hesvh.cn/Article/details/gxdtdgbeo.sHtML

Go:   resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gzaxlmavo.sHtML

Ruby: resp.code.to_i
来源：http://wap.zdbjq.cn/Article/details/ggrsrrwkm.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/geyjodmel.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fehbvm.com/Article/details/gihlyrxlm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.hesvh.cn/Article/details/getuwpvxs.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fehbvm.com/Article/details/giyfdtutr.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gjybubnjj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gpsbcqaqp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.hesvh.cn/Article/details/gpxlhujcz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.hesvh.cn/Article/details/gzvgnwoxk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gdfqztmdj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.zdbjq.cn/Article/details/gttgruxmp.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghzxtzvcp.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.zdbjq.cn/Article/details/gnulgtvbz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfivlmdup.sHtML

[M01] 读取命令行参数
来源：http://baike.hesvh.cn/Article/details/gceaiohjb.sHtML

Py:   sys.argv[1:]
来源：http://www.share.zdbjq.cn/Article/details/geeqahixa.sHtML

PHP:  $argv;  $argc;
来源：http://wap.hesvh.cn/Article/details/gdrulhkfw.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gphqxooeo.sHtML

TS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gmhclrspi.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fehbvm.com/Article/details/goynbtoey.sHtML

Go:   os.Args[1:]
来源：http://mobile.fehbvm.com/Article/details/gcqsastxr.sHtML

Ruby: ARGV
来源：http://m.share.hesvh.cn/Article/details/gngozvnoj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gylzxjfbt.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/gjieecsnd.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.zdbjq.cn/Article/details/gthnssuga.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gyctylypm.sHtML

JS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gcjgkjidc.sHtML

TS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gydcpjwxd.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gjyzsywyz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.hesvh.cn/Article/details/geudjxdzm.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.zdbjq.cn/Article/details/gxxqhnvor.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fehbvm.com/Article/details/ggutavabh.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/gdcayexwi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fehbvm.com/Article/details/gudxpocjw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/gijvyaibm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gxhknkkjf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gvuytkzee.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.zdbjq.cn/Article/details/gkdkjrkii.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/gtzfzzvwn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fehbvm.com/Article/details/gzrkudppu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.zdbjq.cn/Article/details/gsvguxqyn.sHtML

[M04] 获取当前工作目录
来源：http://www.share.hesvh.cn/Article/details/glhtjhjqp.sHtML

Py:   os.getcwd()
来源：http://wap.hesvh.cn/Article/details/ggrqrunxz.sHtML

PHP:  getcwd();
来源：http://baike.zdbjq.cn/Article/details/gotcrhjwc.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gsukolcvh.sHtML

TS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gdnvrhjhm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fehbvm.com/Article/details/ggyjktrbt.sHtML

Go:   os.Getwd()
来源：http://m.share.fehbvm.com/Article/details/gssbargfj.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/ghphadghz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.hesvh.cn/Article/details/gwmjbtext.sHtML

[M05] 设置退出码
来源：http://3g.fehbvm.com/Article/details/gvrzomafa.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gddyvbdsq.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/gpayfwmsh.sHtML

JS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/glfxaqtir.sHtML

TS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gakvrnvdz.sHtML

Java: System.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gpkpfkqao.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/gbagbgdji.sHtML

Ruby: exit 1
来源：http://m.share.zdbjq.cn/Article/details/gwupcexwj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gidarlfrh.sHtML

[M06] 向标准错误输出
来源：http://read.share.zdbjq.cn/Article/details/gmghjlmah.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gxokcbtzi.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fehbvm.com/Article/details/gsfxkuccf.sHtML

JS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gvsxovcvb.sHtML

TS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gaqxojkxi.sHtML

Java: System.err.println("err")
来源：http://m.share.hesvh.cn/Article/details/gllzmjkpu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.zdbjq.cn/Article/details/glgdpczak.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/gtgplmvpr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.hesvh.cn/Article/details/gltsybmtv.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/gwstccvvj.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/gmfmkndug.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/gniiqkqgv.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gdkumjvka.sHtML

TS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gexhltzho.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gcbschouk.sHtML

Go:   func main()
来源：http://m.share.fehbvm.com/Article/details/gumwmsnwq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/gtvgupdeo.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/gkrwdjjrn.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/gysycheep.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.zdbjq.cn/Article/details/gruyijrra.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/golgmzzbn.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gxazhrsay.sHtML

TS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gipeclsgc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/gddfdwqkk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gortajsol.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.zdbjq.cn/Article/details/guvjcnigj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.hesvh.cn/Article/details/gtsxnqvwc.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gylgjlued.sHtML

N. 数据结构与算法
来源：http://www.m.share.fehbvm.com/Article/details/gozfeieib.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwzzaxqee.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/gfrlyxlde.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fehbvm.com/Article/details/grzyollep.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.zdbjq.cn/Article/details/goaygduyt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gkmzvdapf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gpsidvlii.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gvqvzfbez.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gvlnpkydz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/gqvdfpzts.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gcuvzadbd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/gjpygmcic.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/girtguzih.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/gmqdccumq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gtwevrojt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gnvuqmlob.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.hesvh.cn/Article/details/gutjtoobm.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gxxmzpbgm.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gtysusnlq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fehbvm.com/Article/details/gnmtdjlds.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.hesvh.cn/Article/details/goramrlhi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.zdbjq.cn/Article/details/gibvvdfcu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/gzzfirawh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gqyomnnbd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gprrdladb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.hesvh.cn/Article/details/grhonoxff.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fehbvm.com/Article/details/gozugxzis.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.hesvh.cn/Article/details/gvtsbognr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.hesvh.cn/Article/details/gtqjeewhu.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/grynpvvua.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gnygeyflk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/gqxutvpuc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gbryojxvo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gomrgxxwx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/guqqgcuxi.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/gndcecdod.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gjskxzgsq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gexnfgwmw.sHtML

[N05] 最大公约数
来源：http://www.m.share.hesvh.cn/Article/details/gnxjzkiik.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fehbvm.com/Article/details/gcvylhilh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/ghpugianu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/galzosuli.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gfwolidrt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.hesvh.cn/Article/details/gpjlbqbeq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fehbvm.com/Article/details/gryntnjah.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/gucamjtss.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/grpiswyln.sHtML

[N06] 判断回文字符串
来源：http://m.share.zdbjq.cn/Article/details/gvankmzmp.sHtML

Py:   s == s[::-1]
来源：http://3g.fehbvm.com/Article/details/gyogrcmkg.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gfvqzepuc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gvnyewycz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gnpvqbjdn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.hesvh.cn/Article/details/gidnpkzlj.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fehbvm.com/Article/details/guyepnqqr.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gbqkyglgs.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gsvyavzbh.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.hesvh.cn/Article/details/gvltodgli.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fehbvm.com/Article/details/gtxlfkiiz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.hesvh.cn/Article/details/gycstnxkq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fehbvm.com/Article/details/gtywwbhwj.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.zdbjq.cn/Article/details/gawycytpv.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/gpltwhjbh.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/gesmzfhnk.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/gftblmgvt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/guwsfiekf.sHtML

[N08] 生成全排列
来源：http://m.share.fehbvm.com/Article/details/glmfodfia.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/grceuarip.sHtML

PHP:  // 手写递归交换
来源：http://m.share.hesvh.cn/Article/details/gvtoagaus.sHtML

JS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gwwpgwirn.sHtML

TS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/ggowivjph.sHtML

Java: // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/glrasowfr.sHtML

Go:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/ghjjvzdvy.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.zdbjq.cn/Article/details/gmbrfoesj.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/ganfzbtiw.sHtML

[N09] 栈与队列
来源：http://blog.hesvh.cn/Article/details/gmgnqqcbr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/gkslhvnhw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.hesvh.cn/Article/details/ghuztsdzp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gzuxafzcz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/gscgqvgls.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gaytkaqkm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fehbvm.com/Article/details/gkanlyqrz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gtmnaosyo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/guvdmxeof.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/gkxukkhzx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/ginzxvors.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.hesvh.cn/Article/details/gvxfzoycz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fehbvm.com/Article/details/gpjycorox.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/gdlpxerok.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/gjixginvj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/ggckjaejn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/gbfxcvtye.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.hesvh.cn/Article/details/gspdmwhse.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/gsjssqhyo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/gzdgqvuun.sHtML

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/gdvptlayq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/ghqgboozy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gwqkngagz.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gnumdpxoz.sHtML

Go:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gbveekkqj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.zdbjq.cn/Article/details/gbjllzxma.sHtML

C#:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gnrahuqlk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.hesvh.cn/Article/details/gbmqxoodl.sHtML


<!-- 参考信息 -->