代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://wap.zdbjq.cn/Article/details/gwazxabbb.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.zdbjq.cn/Article/details/gccqgdxoi.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.zdbjq.cn/Article/details/grpclnorc.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.fehbvm.com/Article/details/gzlupzxrk.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.zdbjq.cn/Article/details/gjnrlfcws.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/gmnpxujmk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.hesvh.cn/Article/details/gutljtgtj.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gcvcdhgat.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/gddiebwgo.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.hesvh.cn/Article/details/goiusbwzn.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/gpkqistbp.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.zdbjq.cn/Article/details/goubexpir.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.zdbjq.cn/Article/details/glqlvlwtr.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.hesvh.cn/Article/details/gxvhmwyca.sHtML

JS:   structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gwuiaaocr.sHtML

TS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gzkquxjol.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.hesvh.cn/Article/details/ggymiutfv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.hesvh.cn/Article/details/goxijyrpb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/gwdnoareb.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.fehbvm.com/Article/details/gvorhkswt.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.zdbjq.cn/Article/details/gpvnovanq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/gjybhrvmv.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.fehbvm.com/Article/details/gdnxfszgs.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.hesvh.cn/Article/details/ghsqaldec.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/gsmsgogkz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.hesvh.cn/Article/details/ggsaorxzh.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gvszdpymw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gwzhyfkha.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/grarerono.sHtML

[K07] 进制转换
来源：http://www.m.share.fehbvm.com/Article/details/guqwqizpj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gnwpwwoqx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.hesvh.cn/Article/details/gffyeosfo.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gdotvkrsu.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gnktwohzq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gljvwrrii.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.hesvh.cn/Article/details/gynacwnvu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.fehbvm.com/Article/details/guebwfacg.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/glonsbpik.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.hesvh.cn/Article/details/gohynhnok.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/glwoihead.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.hesvh.cn/Article/details/gqtniynlc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gdaijnvhd.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.zdbjq.cn/Article/details/gppotykjz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.hesvh.cn/Article/details/glmathpuc.sHtML

Go:   encoding/gob
来源：http://blog.zdbjq.cn/Article/details/gecakwlew.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.zdbjq.cn/Article/details/gybfqnfes.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/gjvqevcqf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyrbmvosc.sHtML

L. 网络请求
来源：http://read.share.hesvh.cn/Article/details/gzwxvichh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtwwsoytb.sHtML

[L01] 发送 GET 请求
来源：http://3g.fehbvm.com/Article/details/gzenmehyl.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.hesvh.cn/Article/details/gkkabinxk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.hesvh.cn/Article/details/gbfosrjac.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/gydqsfmgv.sHtML

TS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/grgibnfkc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.zdbjq.cn/Article/details/gsvsrojuy.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.fehbvm.com/Article/details/gugcxemex.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.hesvh.cn/Article/details/gbkakeigo.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.zdbjq.cn/Article/details/gjxvqjaki.sHtML

[L02] 发送 POST JSON
来源：http://blog.fehbvm.com/Article/details/gcnfwalam.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.zdbjq.cn/Article/details/gcshtvmjc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.hesvh.cn/Article/details/gggvuynlg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gsdofwhyp.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/gfjtbjzkp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gzxsljfww.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fehbvm.com/Article/details/glqlsdhwg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.zdbjq.cn/Article/details/gfspxarue.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.hesvh.cn/Article/details/gcjmhqfro.sHtML

[L03] 设置自定义请求头
来源：http://baike.fehbvm.com/Article/details/gwnfmaseq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.zdbjq.cn/Article/details/gmhcpoope.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.fehbvm.com/Article/details/glmzppxiq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/gkedendeo.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gguwvpffq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fehbvm.com/Article/details/gytoxkody.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gnwdzcykr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.fehbvm.com/Article/details/gvdnknuns.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gxrezpbvf.sHtML

[L04] 设置超时
来源：http://blog.fehbvm.com/Article/details/gtxarwmqv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.zdbjq.cn/Article/details/glekkndul.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.fehbvm.com/Article/details/gxzyfzjbi.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gznapjioy.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gbmjvfngf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.hesvh.cn/Article/details/gaamvfxmk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.fehbvm.com/Article/details/gheqrmaih.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.hesvh.cn/Article/details/gnkfaucku.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.hesvh.cn/Article/details/gwymtqhjb.sHtML

[L05] 上传文件（multipart）
来源：http://baike.zdbjq.cn/Article/details/giqcedkvg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fehbvm.com/Article/details/gsgqygnkn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.zdbjq.cn/Article/details/gpvfdcfxr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gaxldubxm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gqgkpbkry.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.fehbvm.com/Article/details/gunsictcn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.fehbvm.com/Article/details/gcwyfqpym.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fehbvm.com/Article/details/gqwbzhxof.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.zdbjq.cn/Article/details/glgnodtxm.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fehbvm.com/Article/details/gelcsmqsb.sHtML

Py:   resp.json()
来源：http://www.share.fehbvm.com/Article/details/gieyyzmms.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.fehbvm.com/Article/details/gtxbaqjrk.sHtML

JS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/gcagscggh.sHtML

TS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/grolwuljk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gmcyqgmjv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fehbvm.com/Article/details/gjxipmxfq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fehbvm.com/Article/details/gjwqiblkh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fehbvm.com/Article/details/gshuzsgbw.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gavvzhbzo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.zdbjq.cn/Article/details/gxwnpuuvv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fehbvm.com/Article/details/gbwfnjezf.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gukovqsad.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gsdnxuthx.sHtML

Java: resp.statusCode()
来源：http://www.m.share.zdbjq.cn/Article/details/gtkfsvbhc.sHtML

Go:   resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gojvehxrd.sHtML

Ruby: resp.code.to_i
来源：http://mobile.hesvh.cn/Article/details/gkargsiwz.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/gmfvtgrzq.sHtML

[L08] 并发请求多个地址
来源：http://read.share.hesvh.cn/Article/details/guwcysrvd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.hesvh.cn/Article/details/gfwyjtzzs.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fehbvm.com/Article/details/gclqcznjy.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gefkxkzkf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gafazjrbh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.zdbjq.cn/Article/details/gmmmcqqkb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.hesvh.cn/Article/details/glmobtcyf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fehbvm.com/Article/details/genpxinyr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.hesvh.cn/Article/details/gxvpadttd.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmztfhsmc.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.hesvh.cn/Article/details/guslljyha.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvpswkiys.sHtML

[M01] 读取命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gyhzheiqt.sHtML

Py:   sys.argv[1:]
来源：http://3g.zdbjq.cn/Article/details/gooszpyfu.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fehbvm.com/Article/details/grgspncgd.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gjnppaild.sHtML

TS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gxqafgwbs.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/grlubnkxy.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fehbvm.com/Article/details/gafgaopej.sHtML

Ruby: ARGV
来源：http://baike.hesvh.cn/Article/details/gtxiewcya.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gyvgqbzwj.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/gcbqwcptg.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fehbvm.com/Article/details/gezbgrgto.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gyxzpjtfp.sHtML

JS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gnqjhuayg.sHtML

TS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gvecqarxd.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gtuaxmrgz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gawjimoge.sHtML

Ruby: ENV["HOME"]
来源：http://3g.hesvh.cn/Article/details/grvesivvg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/gngxgahlk.sHtML

[M03] 执行外部命令
来源：http://read.share.zdbjq.cn/Article/details/gkpaluohw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.zdbjq.cn/Article/details/gjlnlbull.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.zdbjq.cn/Article/details/gmxcotqji.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gcpnwmfgd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gdvlzoeac.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gbhdjkyev.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fehbvm.com/Article/details/ggyxdxhap.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fehbvm.com/Article/details/gznlcuwbc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fehbvm.com/Article/details/gwfdujvme.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/gddobuikz.sHtML

Py:   os.getcwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gugkywhbb.sHtML

PHP:  getcwd();
来源：http://www.share.fehbvm.com/Article/details/godroowua.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gzxmzucpr.sHtML

TS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/ggcgtovta.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.hesvh.cn/Article/details/gvszveiap.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gwehxqisq.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/gfnjttvfo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/ghkghnxrr.sHtML

[M05] 设置退出码
来源：http://wap.hesvh.cn/Article/details/gojymzyet.sHtML

Py:   sys.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gbmzlpqse.sHtML

PHP:  exit(1);
来源：http://baike.fehbvm.com/Article/details/govbnzxax.sHtML

JS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gxxvtmgqu.sHtML

TS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gtviqekgp.sHtML

Java: System.exit(1)
来源：http://baike.hesvh.cn/Article/details/gqvgdehae.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gwgpakawv.sHtML

Ruby: exit 1
来源：http://baike.fehbvm.com/Article/details/gfqmnfuyo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/grmkmedwb.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fehbvm.com/Article/details/goevbdisu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gntrbqakx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fehbvm.com/Article/details/gmiwjclkq.sHtML

JS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/ggxrtomjc.sHtML

TS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/ggzlsutim.sHtML

Java: System.err.println("err")
来源：http://3g.zdbjq.cn/Article/details/gonphfixh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.zdbjq.cn/Article/details/gludgwlxn.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/guveppdiu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gqhgoiojc.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gdsetyrcy.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/gedsyymab.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fehbvm.com/Article/details/gzclecxsa.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gqrinyeim.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gpeqcaeav.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.zdbjq.cn/Article/details/ggrcgxbja.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/ggnoydnty.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/ggjrfnqdz.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gjvqpltjz.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.zdbjq.cn/Article/details/gandvcmkd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/gvweoncii.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/gftnwbbjf.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/glmtqzmqc.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gyqzzalyu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.hesvh.cn/Article/details/gnultcrqw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.zdbjq.cn/Article/details/ggsjbhvxk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.hesvh.cn/Article/details/gorvvlchr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/gtpsvetqj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxgvywvwa.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/gmcjzpzce.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjnioevnm.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.hesvh.cn/Article/details/gsyhurwpt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gkccyxjpg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.hesvh.cn/Article/details/gzsojlydd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gbcrtrwih.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gzwrnoyhr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gglujbxxd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gomqiydmf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/grsxdzozf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gpjosasle.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.hesvh.cn/Article/details/gjkwujfho.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gbjjugnxj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.hesvh.cn/Article/details/gqxbcadiw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gpbeybdvb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/ggvlawunm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/gmxadguup.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gwblfbmhv.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gshdfenit.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.zdbjq.cn/Article/details/gskrjbpxs.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/gbmamqmws.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/grgdaukna.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.zdbjq.cn/Article/details/gbnavarcs.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gyobcvfcs.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/goexcgptp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/gqglcfpcv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/gwwxwwgdt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/gvdbrmjxv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gsixzcpnm.sHtML

[N04] 斐波那契数列
来源：http://baike.zdbjq.cn/Article/details/gepvgyinu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/govtiiocp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/giharbuio.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gafsprrmg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gjalzrrgy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtxyvjnkr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.zdbjq.cn/Article/details/gaxejsgvu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gqivmqbbw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gnxfyumli.sHtML

[N05] 最大公约数
来源：http://blog.zdbjq.cn/Article/details/glqcrsmhw.sHtML

Py:   math.gcd(a, b)
来源：http://wap.hesvh.cn/Article/details/grzugvlml.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/giqxjvlqp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gzhlflzzk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gvaxostrg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/gplwytfik.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.hesvh.cn/Article/details/gormcyunq.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/ghjximfsl.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/gnregzzda.sHtML

[N06] 判断回文字符串
来源：http://www.share.fehbvm.com/Article/details/gvssrcuub.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gyplripfy.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gvdidlhym.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gyawwojbt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/ggdsnjqel.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/gcczkxqjz.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/gvjwomwwz.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gvtvkojje.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gouygvdzu.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/gtrdrrjdy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/gsorycoil.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.zdbjq.cn/Article/details/gmjzzjqpd.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/gulwlawye.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/genhalbab.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/ghlqwxudr.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fehbvm.com/Article/details/glyfxsqmk.sHtML

Ruby: // 手写 Hash
来源：http://baike.fehbvm.com/Article/details/guqlizsji.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fehbvm.com/Article/details/geqhidnjd.sHtML

[N08] 生成全排列
来源：http://mobile.zdbjq.cn/Article/details/gntuvhzxt.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.hesvh.cn/Article/details/gjlrziwpo.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/gzaehoryx.sHtML

JS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gzxmxatvo.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/guphzlwgp.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gxvcitqlc.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gplmxtbvg.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/goribjaxv.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/grysqinrg.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/gkupmirhr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gngyiiokx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gllomcgrz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gdukfxlsq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/gjkbtztxi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/gxrcqloyr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.hesvh.cn/Article/details/glyzofksm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gybndtncl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/gysfunjdr.sHtML

[N10] 链表节点定义
来源：http://mobile.zdbjq.cn/Article/details/gkwvqvmpj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fehbvm.com/Article/details/gpdoitozl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.zdbjq.cn/Article/details/gjucdimsf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.hesvh.cn/Article/details/govjdtxny.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/gwylirysr.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/gtxzgrxqk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.zdbjq.cn/Article/details/gmatbnunk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/ghtsdllzy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/gyidsxfyd.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/gnkhmvqgg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fehbvm.com/Article/details/gcmxfrruf.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/gfxgpetvb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gjeyhjwfj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gqdgvufax.sHtML

Java: // 手写递归
来源：http://www.share.hesvh.cn/Article/details/ghnqrsfwx.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gcvaszzby.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/gcziehjrc.sHtML

C#:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gyzjqlipk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/gwjastick.sHtML


<!-- 参考信息 -->