代发 wailian999

TS:   JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/gwkgagtux.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.zdbjq.cn/Article/details/glzatevzy.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.zdbjq.cn/Article/details/gmliqcgca.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/gflsvdxck.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.zdbjq.cn/Article/details/gutuavoov.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.zdbjq.cn/Article/details/gddkkgaqq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gaedikzwb.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.zdbjq.cn/Article/details/gpuknhpek.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/gkcpufevo.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.zdbjq.cn/Article/details/grwhnmcbr.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.hesvh.cn/Article/details/grnwljfsa.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.fehbvm.com/Article/details/gkuuzbawf.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.zdbjq.cn/Article/details/gjxqxljbg.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.hesvh.cn/Article/details/gtgxkmldw.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.fehbvm.com/Article/details/ggnimedgj.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.fehbvm.com/Article/details/gzgshrzza.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.fehbvm.com/Article/details/gyoiwrkna.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/gcmuetbmt.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.hesvh.cn/Article/details/gpndsalen.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gjncotkop.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/gxlqzrqeh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gfloqpsax.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/gkvncgnte.sHtML

[K05] 深拷贝对象
来源：http://baike.zdbjq.cn/Article/details/gifbvgphz.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.zdbjq.cn/Article/details/gbfgqvseb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.fehbvm.com/Article/details/gtkcavvsr.sHtML

JS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gqwygncft.sHtML

TS:   structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gdxnxhncy.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.zdbjq.cn/Article/details/gsrxqfydh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.hesvh.cn/Article/details/gsgrptesn.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.hesvh.cn/Article/details/gcmyngwgb.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.zdbjq.cn/Article/details/gqopydltm.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.zdbjq.cn/Article/details/gtlijzjhx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.hesvh.cn/Article/details/gcwpszwza.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.hesvh.cn/Article/details/gitgvlnci.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.hesvh.cn/Article/details/gzvsljidn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gfmehaazx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.zdbjq.cn/Article/details/ghpkpwcib.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gpsuwxkdy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gagmqczmy.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/glaxoaiiw.sHtML

[K07] 进制转换
来源：http://3g.hesvh.cn/Article/details/gtqhfmqjz.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gjhsvrkum.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.fehbvm.com/Article/details/gyhwapfhv.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gbfeagant.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/glwyghmad.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gdocpemuj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.hesvh.cn/Article/details/grtaqplnc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.fehbvm.com/Article/details/geuctxnis.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gijrdqatr.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.fehbvm.com/Article/details/gxidmgkwq.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.zdbjq.cn/Article/details/giamhyezg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.hesvh.cn/Article/details/gpcqkrkvy.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gismkypcf.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/ghkqlnjzq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.zdbjq.cn/Article/details/gymcxvlaq.sHtML

Go:   encoding/gob
来源：http://blog.hesvh.cn/Article/details/gjzuhecyk.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fehbvm.com/Article/details/gsmlgfhdz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/gyobfrjgb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gismrgras.sHtML

L. 网络请求
来源：http://mobile.hesvh.cn/Article/details/gjvcxhpzb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glvzjskai.sHtML

[L01] 发送 GET 请求
来源：http://www.share.hesvh.cn/Article/details/gbobjrjok.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.fehbvm.com/Article/details/giczkcefh.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.zdbjq.cn/Article/details/gsfxmcdbp.sHtML

JS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/gmtxsbwuk.sHtML

TS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/gedvrkdie.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.zdbjq.cn/Article/details/gdxkgifdp.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.hesvh.cn/Article/details/gkypbrdxd.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.zdbjq.cn/Article/details/gtsbsfwvj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.hesvh.cn/Article/details/gklywwdwe.sHtML

[L02] 发送 POST JSON
来源：http://3g.fehbvm.com/Article/details/gxysgymwe.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/gdnplaixf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.fehbvm.com/Article/details/gwhwvgtua.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gseicipzr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gydetujdo.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.zdbjq.cn/Article/details/gckvudeyw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.hesvh.cn/Article/details/goyvbhlsq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.hesvh.cn/Article/details/gesyzjqxk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.hesvh.cn/Article/details/gzjgqxmpf.sHtML

[L03] 设置自定义请求头
来源：http://m.share.zdbjq.cn/Article/details/gchvrkxnr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fehbvm.com/Article/details/gthxwayyf.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.hesvh.cn/Article/details/gkirmkvyl.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gxtzthzma.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/geyndcpis.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.zdbjq.cn/Article/details/gktfewoep.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/gvvpaksja.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.hesvh.cn/Article/details/gztbdacml.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gdioqbwvz.sHtML

[L04] 设置超时
来源：http://m.share.zdbjq.cn/Article/details/gkjfiksvu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fehbvm.com/Article/details/gqgreztho.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gzbxnsiuw.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/gcudbrald.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gdytinouf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gxkpddkka.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.zdbjq.cn/Article/details/gcbkjqgoi.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.zdbjq.cn/Article/details/gabxkwppo.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.zdbjq.cn/Article/details/gmqjnlxjc.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.hesvh.cn/Article/details/gkynwtkzr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fehbvm.com/Article/details/gahwyadpn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.zdbjq.cn/Article/details/gtjpjvptl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/ghanbyzqo.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gglwhxfbb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.zdbjq.cn/Article/details/gznwmjvhd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.zdbjq.cn/Article/details/gxfopnijo.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.hesvh.cn/Article/details/gohumcxrv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.hesvh.cn/Article/details/gcgcrixct.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.hesvh.cn/Article/details/gzdtajbdo.sHtML

Py:   resp.json()
来源：http://blog.fehbvm.com/Article/details/gcenmawlm.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fehbvm.com/Article/details/gmeoenbaf.sHtML

JS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/glmwadgva.sHtML

TS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gpvrtdxnv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/giszvomnu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.fehbvm.com/Article/details/gvtoyodlc.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.hesvh.cn/Article/details/ghaqjyxtp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/ggsszmllp.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gdzpxeijs.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.zdbjq.cn/Article/details/gtypxgcup.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.zdbjq.cn/Article/details/gdnafqyla.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/ggkyvilbi.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/geoghigjd.sHtML

Java: resp.statusCode()
来源：http://wap.fehbvm.com/Article/details/ggiipdqqs.sHtML

Go:   resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/grgvlbyey.sHtML

Ruby: resp.code.to_i
来源：http://baike.hesvh.cn/Article/details/gcjldkufc.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gqjtdqosx.sHtML

[L08] 并发请求多个地址
来源：http://blog.zdbjq.cn/Article/details/goiouilqy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.zdbjq.cn/Article/details/gluvzbsje.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fehbvm.com/Article/details/ghtrnajrv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gsamhszzc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gbflioccj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fehbvm.com/Article/details/gumetmpaz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.zdbjq.cn/Article/details/gimskmylc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gxdecqoke.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.hesvh.cn/Article/details/gemvnzzar.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyjbnovrx.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fehbvm.com/Article/details/gywuyyqlt.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gdihjfgyv.sHtML

[M01] 读取命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gjotxtttw.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fehbvm.com/Article/details/gyaidiwes.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fehbvm.com/Article/details/gesxooskp.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gocczcyct.sHtML

TS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gkwnmbiyu.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gezrkpkwi.sHtML

Go:   os.Args[1:]
来源：http://read.share.hesvh.cn/Article/details/gtnuseozl.sHtML

Ruby: ARGV
来源：http://mobile.zdbjq.cn/Article/details/ghvsmquea.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gprqqxspm.sHtML

[M02] 读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gqrhyydzg.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.hesvh.cn/Article/details/gsjgpazgi.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/goytqnppb.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gzfvacqgb.sHtML

TS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gkudijgrb.sHtML

Java: System.getenv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gxfdmodrh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gzlkdmerp.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.hesvh.cn/Article/details/gzctpthgm.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fehbvm.com/Article/details/gkpahziap.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fehbvm.com/Article/details/gyvuiyrhv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/gznzikwkf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.hesvh.cn/Article/details/glceqrglt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gyoipeoth.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gjmlidrlm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.zdbjq.cn/Article/details/gpbrejhuk.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.hesvh.cn/Article/details/ganftdekk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fehbvm.com/Article/details/gdwdqzgwj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.zdbjq.cn/Article/details/gwaqlyumk.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/guqejqnpo.sHtML

Py:   os.getcwd()
来源：http://www.blog.zdbjq.cn/Article/details/gxrrnmlii.sHtML

PHP:  getcwd();
来源：http://www.m.share.hesvh.cn/Article/details/ghynwljzn.sHtML

JS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gcowhqtjc.sHtML

TS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/ggukmcgjq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/gmufdmsuv.sHtML

Go:   os.Getwd()
来源：http://mobile.fehbvm.com/Article/details/gquznrrbs.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/glurjuxot.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.hesvh.cn/Article/details/gsreteznl.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/gncuiguoi.sHtML

Py:   sys.exit(1)
来源：http://baike.hesvh.cn/Article/details/gzcjaecyc.sHtML

PHP:  exit(1);
来源：http://blog.zdbjq.cn/Article/details/guyjlbosn.sHtML

JS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gwmrjeqzo.sHtML

TS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gfwbxikhz.sHtML

Java: System.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gxpwdgcpd.sHtML

Go:   os.Exit(1)
来源：http://wap.fehbvm.com/Article/details/gtfuywaro.sHtML

Ruby: exit 1
来源：http://www.blog.fehbvm.com/Article/details/gojteteae.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.zdbjq.cn/Article/details/gxvcfgycc.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/gfdrdvjar.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gyhokcmxu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/gifulgext.sHtML

JS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gumbuefgx.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/goyykcbkr.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/gpvbbscql.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.hesvh.cn/Article/details/gmncctofa.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/gdjodyqeu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.hesvh.cn/Article/details/gdegnnqzq.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/grpltihtp.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fehbvm.com/Article/details/gmppablrr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.hesvh.cn/Article/details/gkdomxthl.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/grevzvmlc.sHtML

TS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gwzhektkb.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/gzntniokj.sHtML

Go:   func main()
来源：http://www.m.share.fehbvm.com/Article/details/gleggyfai.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/gdkibwovz.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/gyslctkdf.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/gnqtdmnaz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fehbvm.com/Article/details/gbgtoborc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/gvqruspzb.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gvnqhzdfb.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gtjqphlin.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/gnlawkegz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/gbuoxxqwm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gdhihoumf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.hesvh.cn/Article/details/gldjhrkan.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gisshcpvr.sHtML

N. 数据结构与算法
来源：http://m.share.fehbvm.com/Article/details/gvsmpfprr.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfuslyjdv.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fehbvm.com/Article/details/gkycvlodw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gvhukkful.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/ggvtuwlsy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gzlcyerpe.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/geudhjawz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gpyjmchgy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gvhxakjud.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.hesvh.cn/Article/details/giawtusrw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gbsdxlbfv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.zdbjq.cn/Article/details/gcdbylhut.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gsuwcgnuo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fehbvm.com/Article/details/gijmqthlu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gcpxdwqng.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/ganzwnwmw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fehbvm.com/Article/details/gjfovbqyj.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gdtvvnbex.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gtjxjebyw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gguyjtokz.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/gyzpvgqjy.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.hesvh.cn/Article/details/gwktlhxbr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.hesvh.cn/Article/details/gyxcsguxx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/grgrvscfi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gnteeulwc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.zdbjq.cn/Article/details/gbcjrraft.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fehbvm.com/Article/details/goejnxulg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.hesvh.cn/Article/details/grcxhvtna.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.hesvh.cn/Article/details/ggnrqnyss.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gjxqdrcnk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gnvtpuejs.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gykunbqsz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/ggzbnomdn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/ghqsilfxj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gwvwdivhb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fehbvm.com/Article/details/gsratftav.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gmcyavtlp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gipplgruv.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/gptjiyybs.sHtML

Py:   math.gcd(a, b)
来源：http://blog.hesvh.cn/Article/details/gvomrxjqi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/gbjnukbeo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gleahjmky.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gdqcbouqy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/gurjicvki.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/ggmghyqbc.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/gvpporlmu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/gwqrosftt.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/gvqaglacy.sHtML

Py:   s == s[::-1]
来源：http://3g.zdbjq.cn/Article/details/ggcczaslz.sHtML

PHP:  $s === strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gnxiufuwl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gchykulvw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gfamghfqb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/gjecvqqka.sHtML

Go:   // 双指针从两端比较
来源：http://wap.zdbjq.cn/Article/details/gfbeekkyr.sHtML

Ruby: s == s.reverse
来源：http://mobile.hesvh.cn/Article/details/gwxnicobi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gsfzkikyj.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fehbvm.com/Article/details/goibqvngf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/gwmqzpqql.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.hesvh.cn/Article/details/guzljirvp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/gnsvwdzda.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/gbrbhqbsq.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/gxuoihoeu.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/gucmrposz.sHtML

Ruby: // 手写 Hash
来源：http://baike.zdbjq.cn/Article/details/gvecigkyv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gylektpzn.sHtML

[N08] 生成全排列
来源：http://www.blog.hesvh.cn/Article/details/gznmcynbc.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gupwxgmop.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fehbvm.com/Article/details/gqthnvieo.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gxsjzgxpf.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gspzjhvej.sHtML

Java: // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gpegwfcln.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/giiyqmzhy.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/gjgdcgkym.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gbkhxvqeo.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/gmxshqkij.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/gpoqjplnl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fehbvm.com/Article/details/gsvjpjquw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gghsqhdqt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/grytgnvqs.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/golphiqlz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/gatvkkbri.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gbhtbcqcn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/gyjbwvyfm.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/gdacvouvu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.zdbjq.cn/Article/details/gqckozwob.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/gqlwfcrzt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/gurmuycgn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.hesvh.cn/Article/details/gaqwqyxuy.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/gxpvwuwbi.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.hesvh.cn/Article/details/gqqrfxque.sHtML


<!-- 参考信息 -->