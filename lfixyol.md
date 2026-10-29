代发 wailian999

TS:   JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gigkhlbvh.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.hesvh.cn/Article/details/gewhfrtzj.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.hesvh.cn/Article/details/gkojruita.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gwjqrulia.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.fehbvm.com/Article/details/gylgivmjd.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.hesvh.cn/Article/details/guuhsxmmz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.zdbjq.cn/Article/details/gjvilyvzo.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/gbnonnwjn.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.zdbjq.cn/Article/details/gfkjbjzcz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/gicsjjdsq.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.fehbvm.com/Article/details/gaptjxntq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.fehbvm.com/Article/details/gusthtsmj.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.fehbvm.com/Article/details/gzbwtsjaf.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.hesvh.cn/Article/details/gzjtjaxkq.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.zdbjq.cn/Article/details/gqqhfiioq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fehbvm.com/Article/details/gghmasdzh.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.fehbvm.com/Article/details/gzfpgsobk.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/ggncwhsiv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/gkqezrxhc.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gnypvzlvp.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/gwzfuefzx.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.hesvh.cn/Article/details/guaswudkg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.fehbvm.com/Article/details/gcbgcovwz.sHtML

[K05] 深拷贝对象
来源：http://www.share.hesvh.cn/Article/details/gylcagfuv.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.fehbvm.com/Article/details/gwcnmyavy.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.fehbvm.com/Article/details/gostuqgly.sHtML

JS:   structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/ggelmhxtv.sHtML

TS:   structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/gyyvyfqpl.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.hesvh.cn/Article/details/gfcfkuqom.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.zdbjq.cn/Article/details/gxnelpaha.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.fehbvm.com/Article/details/gxzdpudeg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.fehbvm.com/Article/details/gidkllzip.sHtML

[K06] 解析 URL 查询串
来源：http://wap.fehbvm.com/Article/details/gpzqkmyoz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.fehbvm.com/Article/details/gidnetetw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.zdbjq.cn/Article/details/guwnninmx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.hesvh.cn/Article/details/gxauqrlbd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/gjdywmatx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.zdbjq.cn/Article/details/glqupakuy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/gwuyueqtx.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gbpaksetz.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/ggrdenejn.sHtML

[K07] 进制转换
来源：http://m.share.zdbjq.cn/Article/details/ghjaezueb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gshuhhfpe.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.fehbvm.com/Article/details/gztpsydoy.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/ggqygbdjn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/ghgpulhcq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gxbcqvdzw.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.zdbjq.cn/Article/details/gdoqfxxmt.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.hesvh.cn/Article/details/gwidtxblm.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/geuwhxmhd.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.fehbvm.com/Article/details/gvjopdapa.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gamowgrjz.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.fehbvm.com/Article/details/gxvwadqom.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/gpzcxxagz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gtswlvhti.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.fehbvm.com/Article/details/gxfnpzbnl.sHtML

Go:   encoding/gob
来源：http://www.m.share.hesvh.cn/Article/details/gplnmxyor.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.zdbjq.cn/Article/details/giyqjczjv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.fehbvm.com/Article/details/gmdrjlaqo.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzblowwwn.sHtML

L. 网络请求
来源：http://wap.fehbvm.com/Article/details/ggntbqakf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmepezbke.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fehbvm.com/Article/details/gdmrxsdlr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.fehbvm.com/Article/details/gizmkihed.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.fehbvm.com/Article/details/gjnmfttkw.sHtML

JS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gnpqzijyi.sHtML

TS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/gxwbruzsg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.hesvh.cn/Article/details/gxdpjoycy.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.zdbjq.cn/Article/details/gvxtlyvst.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fehbvm.com/Article/details/gmaqgcraa.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.hesvh.cn/Article/details/gsrfjlotv.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/ggqgaiswx.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gqxicejbd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.fehbvm.com/Article/details/ggljxmljb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/geonywxba.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/ghogusrwz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fehbvm.com/Article/details/gcofkbzhr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.zdbjq.cn/Article/details/gtoselppv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.zdbjq.cn/Article/details/gqjqolnge.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.zdbjq.cn/Article/details/gutgerraa.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.fehbvm.com/Article/details/guhnxtvni.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fehbvm.com/Article/details/gaicmehuc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.fehbvm.com/Article/details/gglyjcubt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gbhxexzln.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/ghwqglqch.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.hesvh.cn/Article/details/gibgvhlxb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/gjepaxxfz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.hesvh.cn/Article/details/gqnzwgvxl.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/garbblwio.sHtML

[L04] 设置超时
来源：http://3g.hesvh.cn/Article/details/gsutlbcya.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.fehbvm.com/Article/details/gndrdxcbk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gcflqptev.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gdqzqsbec.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/ghgyupxof.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.hesvh.cn/Article/details/gtuyhofxn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fehbvm.com/Article/details/gvguzuqno.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.zdbjq.cn/Article/details/gqxiklovj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fehbvm.com/Article/details/gnkjrtuym.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fehbvm.com/Article/details/gdphheles.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/ghakxnyvb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.hesvh.cn/Article/details/gxtsdszvx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gfbcmgtws.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gjxftlmrm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fehbvm.com/Article/details/gqgijflek.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.zdbjq.cn/Article/details/gyedclxcz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.zdbjq.cn/Article/details/gqsrlkukk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gencabyjj.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.fehbvm.com/Article/details/gzulibuyw.sHtML

Py:   resp.json()
来源：http://www.share.hesvh.cn/Article/details/gzvvoeona.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.hesvh.cn/Article/details/ghprcbsur.sHtML

JS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gknvzmnrw.sHtML

TS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/ggywfyadp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gwacjiyud.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.zdbjq.cn/Article/details/gqqatocym.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.zdbjq.cn/Article/details/gpcxihnuo.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gtjrdqwvb.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gwodutsal.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fehbvm.com/Article/details/gtajyevkr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.zdbjq.cn/Article/details/gfvoetsvv.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/goyunhdhy.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/guzmsfluk.sHtML

Java: resp.statusCode()
来源：http://baike.fehbvm.com/Article/details/gxhcvovfh.sHtML

Go:   resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gvdhyetli.sHtML

Ruby: resp.code.to_i
来源：http://blog.zdbjq.cn/Article/details/gmqnypyts.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/galzfdrcj.sHtML

[L08] 并发请求多个地址
来源：http://read.share.hesvh.cn/Article/details/gjhwbgtro.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.hesvh.cn/Article/details/gfchxsvzf.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.zdbjq.cn/Article/details/gkimksugi.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gqhaplmqb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/ghilrshuk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fehbvm.com/Article/details/glcmcmrff.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.hesvh.cn/Article/details/gptglqzvi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/gllzgthml.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/gbjreqcru.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjhyvygeo.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.zdbjq.cn/Article/details/gluaqwzzp.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzltyerrm.sHtML

[M01] 读取命令行参数
来源：http://read.share.fehbvm.com/Article/details/grspocfpj.sHtML

Py:   sys.argv[1:]
来源：http://blog.fehbvm.com/Article/details/gwqiiuedg.sHtML

PHP:  $argv;  $argc;
来源：http://wap.hesvh.cn/Article/details/graugqsgw.sHtML

JS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/guxlcahps.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gibjpqwck.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gmedyuyha.sHtML

Go:   os.Args[1:]
来源：http://read.share.fehbvm.com/Article/details/ggbzetebs.sHtML

Ruby: ARGV
来源：http://read.share.zdbjq.cn/Article/details/gshoeacko.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gwtslthqv.sHtML

[M02] 读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gbbztfxhr.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.zdbjq.cn/Article/details/govduhniu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gbyszltcj.sHtML

JS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gjpgeqotp.sHtML

TS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gwoisausz.sHtML

Java: System.getenv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gzaaagwnm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gmyksthek.sHtML

Ruby: ENV["HOME"]
来源：http://baike.hesvh.cn/Article/details/gwtabkhsc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.zdbjq.cn/Article/details/grvjvsoko.sHtML

[M03] 执行外部命令
来源：http://read.share.hesvh.cn/Article/details/gxetuoydn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.zdbjq.cn/Article/details/gwjfgcomn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.zdbjq.cn/Article/details/gienqlzxf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gxyalgpij.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gvlffftzt.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.zdbjq.cn/Article/details/gkywwruao.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.hesvh.cn/Article/details/ghbsjefwe.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/gafrsbmfx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.zdbjq.cn/Article/details/gpdkceiau.sHtML

[M04] 获取当前工作目录
来源：http://read.share.hesvh.cn/Article/details/ghcgzlbsn.sHtML

Py:   os.getcwd()
来源：http://www.blog.hesvh.cn/Article/details/gzydskebq.sHtML

PHP:  getcwd();
来源：http://mobile.fehbvm.com/Article/details/gklxqbrxm.sHtML

JS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gdefynyad.sHtML

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gfmtaechy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fehbvm.com/Article/details/gwvtedvec.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/gbskvkluv.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/gekalvqot.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fehbvm.com/Article/details/gtgqtmvwf.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/grkofiujb.sHtML

Py:   sys.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gvlwqobmy.sHtML

PHP:  exit(1);
来源：http://www.blog.fehbvm.com/Article/details/gnpkfbvuc.sHtML

JS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gdvdwucyf.sHtML

TS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gdczbamao.sHtML

Java: System.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gpivtxhad.sHtML

Go:   os.Exit(1)
来源：http://m.share.fehbvm.com/Article/details/gkgbxoykf.sHtML

Ruby: exit 1
来源：http://www.share.hesvh.cn/Article/details/gttqxqlau.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fehbvm.com/Article/details/giriuzhgj.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fehbvm.com/Article/details/gtbppsqpa.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gocfcqnql.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.hesvh.cn/Article/details/gdcgfogwa.sHtML

JS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gcautgfch.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gmibyewgi.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/ghduwuqke.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/gbywaajsw.sHtML

Ruby: warn "err"
来源：http://www.blog.fehbvm.com/Article/details/gicdtdirt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.zdbjq.cn/Article/details/gqurlusam.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/ghitqaiiw.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.zdbjq.cn/Article/details/gadittvwy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.zdbjq.cn/Article/details/gvtkwdjpl.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gpwbyndpm.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gwqptkjpq.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gfzrblorh.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/gzmbbfafr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fehbvm.com/Article/details/gyfzkhusj.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fehbvm.com/Article/details/gftdodatp.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.zdbjq.cn/Article/details/gplshdkxi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.hesvh.cn/Article/details/gzcdzzcyq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.zdbjq.cn/Article/details/ghnfcxhql.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/giimrrgao.sHtML

TS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gityxzzii.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.zdbjq.cn/Article/details/gfpagdpzy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.hesvh.cn/Article/details/gapgauqym.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.zdbjq.cn/Article/details/gjzyosudq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.hesvh.cn/Article/details/gdsswfvwa.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnxypgfbv.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gmkewdyxk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gazejmcvb.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fehbvm.com/Article/details/greuvbmyg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gkbarggro.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/gkjtytcai.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gxpgqxtpn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gnpjxiehu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gtjddnbzw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.zdbjq.cn/Article/details/ghwxinbmu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.zdbjq.cn/Article/details/gyxhwugne.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gqtujomys.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.zdbjq.cn/Article/details/gftfwkcug.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gctozbgds.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gusfjixuq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gnpklnwlh.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/grtqygxdg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/ghwfanmnr.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gfnsyevgz.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gxnejeald.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.zdbjq.cn/Article/details/gmtorxein.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.hesvh.cn/Article/details/gufpjhjfn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fehbvm.com/Article/details/gifucovco.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/gebdctxdj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gcezumzwk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gubbupjoc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.hesvh.cn/Article/details/grcytgsvt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/ggbuyuuss.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fehbvm.com/Article/details/gkwkslznf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/guistcamd.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/glhyvonbu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gwrnxopdu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gfpgbxlbd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gszbqdrjo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gefxvnwbo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.hesvh.cn/Article/details/gxcnococn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fehbvm.com/Article/details/gkddrvhwy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gpfuhvupi.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/ganttkoib.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/gdxpoeihw.sHtML

Py:   math.gcd(a, b)
来源：http://wap.zdbjq.cn/Article/details/guicmgvce.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/goaqieduf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gsbygkuna.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gussohjwf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/gdzjbmshq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/grptnogsr.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/grhctzkeu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.hesvh.cn/Article/details/gppzcvvnc.sHtML

[N06] 判断回文字符串
来源：http://www.share.zdbjq.cn/Article/details/gcqxvxtvp.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/gypmnwxhi.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gcvmxekpr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gzcxdkfvs.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/grcqyamly.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/guklfynwx.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/gimzviibx.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gvktoepua.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gxirzzpui.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fehbvm.com/Article/details/gjhsnxyxo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gtqixhuzp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fehbvm.com/Article/details/gzneymahb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/gofcgldig.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/gdvwxvtrm.sHtML

Java: // 手写 HashMap
来源：http://www.share.hesvh.cn/Article/details/gkulquwck.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.hesvh.cn/Article/details/gvxxuhvae.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gtyvbnzpf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.hesvh.cn/Article/details/gdqgsmuit.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/grycnxoej.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/gjkkvrfxo.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/glrfpqzwi.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gqpqrwwsr.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gkvqbwlhx.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/goeongwwc.sHtML

Go:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gqkqfoglf.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.zdbjq.cn/Article/details/ghshekhnb.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gpnzjtvwu.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/ghhhnnehd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gcnrcsbab.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gltrzdajs.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/grvgdbsup.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/gswqlbhof.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.hesvh.cn/Article/details/gphntjrkz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/gfyuefhvp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gxcpgxoza.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.zdbjq.cn/Article/details/gspnzrnns.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/guondctjr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/grrlvcoke.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.hesvh.cn/Article/details/gldufsfhs.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/gihnwvaqv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fehbvm.com/Article/details/gremrblif.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/gwwjlifgt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.hesvh.cn/Article/details/gsxqnxist.sHtML


<!-- 参考信息 -->