代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.hesvh.cn/Article/details/getniqazj.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.fehbvm.com/Article/details/gzadhzfmk.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.fehbvm.com/Article/details/gakmnuhvn.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.zdbjq.cn/Article/details/gebicaldt.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.fehbvm.com/Article/details/gpgacxbht.sHtML

Py:   json.loads(s)
来源：http://www.m.share.hesvh.cn/Article/details/gxffmrmba.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.fehbvm.com/Article/details/ghkjmddbx.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gwxmkybse.sHtML

TS:   JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gtrpvazqu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.fehbvm.com/Article/details/gjcjdvvud.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.fehbvm.com/Article/details/gevjozghr.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gpzqymzln.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.fehbvm.com/Article/details/gtblwzvdi.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.hesvh.cn/Article/details/gcoqojulo.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.hesvh.cn/Article/details/gndblfhkr.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/gcoawejac.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fehbvm.com/Article/details/gogwprtyw.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gxtevsiou.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.fehbvm.com/Article/details/grluqbmdj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.hesvh.cn/Article/details/gmnijkglc.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.zdbjq.cn/Article/details/gpzwlibnk.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.hesvh.cn/Article/details/gfkfpkaus.sHtML

[K04] 读取 JSON 文件
来源：http://3g.hesvh.cn/Article/details/guipjchsi.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.zdbjq.cn/Article/details/gvbbhopgj.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.zdbjq.cn/Article/details/gzgjomxex.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/gwjchiykg.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.zdbjq.cn/Article/details/glaaxqbdi.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gysllxtut.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.hesvh.cn/Article/details/gvkyawxqi.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.hesvh.cn/Article/details/giwexlmsq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gqeicruxi.sHtML

[K05] 深拷贝对象
来源：http://www.blog.fehbvm.com/Article/details/gsfzlwkaf.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.fehbvm.com/Article/details/gptscszcr.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.zdbjq.cn/Article/details/grmfcthfl.sHtML

JS:   structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gpoclompg.sHtML

TS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gybtuxlpf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.fehbvm.com/Article/details/gvagiissx.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.hesvh.cn/Article/details/gbsajmmvo.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.fehbvm.com/Article/details/gvpkutqfu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.zdbjq.cn/Article/details/grnjwnifp.sHtML

[K06] 解析 URL 查询串
来源：http://baike.hesvh.cn/Article/details/gbbtttudb.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/gtlbgdyme.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.fehbvm.com/Article/details/gfmbzryns.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/gxmljvtex.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/gxmgrdcrq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.fehbvm.com/Article/details/glfqhkuwy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gdsvrdumy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gygzykhfb.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gionmmepg.sHtML

[K07] 进制转换
来源：http://www.blog.hesvh.cn/Article/details/gzhllbonz.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/geblwtkcl.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.fehbvm.com/Article/details/gpnvqldrv.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/grlywgeqp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gkaqjadvh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gukrbobof.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.hesvh.cn/Article/details/gphpvwscg.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.hesvh.cn/Article/details/gbremjjoe.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gnpqkfgmh.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.hesvh.cn/Article/details/gkuwapvau.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gbfyboocr.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.hesvh.cn/Article/details/guoeltilu.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gdolozzbk.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/gbqvtyoha.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.hesvh.cn/Article/details/gsuouamdq.sHtML

Go:   encoding/gob
来源：http://wap.fehbvm.com/Article/details/gtiilbyze.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.hesvh.cn/Article/details/gcvdkvaox.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/giivaenek.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmobritbj.sHtML

L. 网络请求
来源：http://www.share.fehbvm.com/Article/details/gwydoxkiu.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkwjwdxuv.sHtML

[L01] 发送 GET 请求
来源：http://www.share.fehbvm.com/Article/details/gibuetakz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.zdbjq.cn/Article/details/ggnknbvhm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.zdbjq.cn/Article/details/grvtdesnx.sHtML

JS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/grtisypxw.sHtML

TS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/gfvrusrfn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.zdbjq.cn/Article/details/gdeuparoy.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.zdbjq.cn/Article/details/gpkrbticb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.zdbjq.cn/Article/details/gwgcljkbn.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.hesvh.cn/Article/details/gwhcfyhdr.sHtML

[L02] 发送 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gltkorkxp.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gwrmttgsu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.zdbjq.cn/Article/details/gjrgdiimw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gwsdabaeo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/gxxzflsyv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.hesvh.cn/Article/details/gplmcuqoy.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.zdbjq.cn/Article/details/ggjyehont.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.hesvh.cn/Article/details/gcwctnzry.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.hesvh.cn/Article/details/glmjfxoqf.sHtML

[L03] 设置自定义请求头
来源：http://www.share.zdbjq.cn/Article/details/ghkehvujy.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fehbvm.com/Article/details/gkljjahsz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.fehbvm.com/Article/details/gmpkzjbrc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/gpokdprju.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/grzuemasr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.fehbvm.com/Article/details/gtpmvaoyi.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gbgmufiir.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.zdbjq.cn/Article/details/gcsgkwpsl.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gwvfybloy.sHtML

[L04] 设置超时
来源：http://www.m.share.fehbvm.com/Article/details/gcrewphkl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.hesvh.cn/Article/details/gglydszni.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.zdbjq.cn/Article/details/gueqqkcwk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gdyjhnnnb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/gsnyxjmxk.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fehbvm.com/Article/details/gsgkkwjgw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.hesvh.cn/Article/details/gifxuhibt.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.hesvh.cn/Article/details/gdpepojxy.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fehbvm.com/Article/details/ghxhklqsy.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fehbvm.com/Article/details/gmoyberbw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/gpnmuzgxf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fehbvm.com/Article/details/goevccmvh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gmchjyotz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gfrxvyxcn.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.zdbjq.cn/Article/details/ghgfmxbka.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.hesvh.cn/Article/details/gwkafrowt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.zdbjq.cn/Article/details/giscyrgrw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.hesvh.cn/Article/details/ggcxmwozu.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.fehbvm.com/Article/details/ghyxelkcu.sHtML

Py:   resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gflfzfvyn.sHtML

PHP:  json_decode($body, true);
来源：http://blog.zdbjq.cn/Article/details/glrkxvgls.sHtML

JS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gomqdvhiq.sHtML

TS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gvkpjfkjx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gdgqbuqgn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fehbvm.com/Article/details/gftsdgwnu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fehbvm.com/Article/details/gxeltcsyf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.zdbjq.cn/Article/details/gckjapvcp.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gcilkpmcq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fehbvm.com/Article/details/grwapdzzv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.zdbjq.cn/Article/details/grjsylegk.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gyoqggmld.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gfkisggmm.sHtML

Java: resp.statusCode()
来源：http://www.blog.zdbjq.cn/Article/details/gllctfhfu.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/grgldxwun.sHtML

Ruby: resp.code.to_i
来源：http://m.share.zdbjq.cn/Article/details/gdckppyzt.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/ggttrbeka.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fehbvm.com/Article/details/gcyidvkxi.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.fehbvm.com/Article/details/gyozmdmwa.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.zdbjq.cn/Article/details/ghefgzkee.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gbtyotcvy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gpcnmdrjf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fehbvm.com/Article/details/gensdhplz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.zdbjq.cn/Article/details/gstnepxdr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.zdbjq.cn/Article/details/gfnssyghb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.hesvh.cn/Article/details/gaoanevqp.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkeniluar.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fehbvm.com/Article/details/gqwebnyyc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvojqgnbi.sHtML

[M01] 读取命令行参数
来源：http://3g.hesvh.cn/Article/details/gsaejbufc.sHtML

Py:   sys.argv[1:]
来源：http://baike.zdbjq.cn/Article/details/gpetybyim.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.hesvh.cn/Article/details/gwyizknms.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gwhvxdzug.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gliwzmhfc.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gwsgwkdjp.sHtML

Go:   os.Args[1:]
来源：http://baike.hesvh.cn/Article/details/gwuwmtdby.sHtML

Ruby: ARGV
来源：http://m.share.hesvh.cn/Article/details/gdffqzcbn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/ghyufuato.sHtML

[M02] 读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/ghgywbvrf.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.hesvh.cn/Article/details/gtwghpiot.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gpfbiztqb.sHtML

JS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gopbxkvqx.sHtML

TS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/glevnbglb.sHtML

Java: System.getenv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gysegszsa.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/goszgwsuy.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/giqtyxocm.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.zdbjq.cn/Article/details/geufaamku.sHtML

[M03] 执行外部命令
来源：http://www.blog.fehbvm.com/Article/details/griyabwbp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.hesvh.cn/Article/details/glvqegltc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fehbvm.com/Article/details/gnqfzqxgc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gghbesgbo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/guscgryfu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/gkyrogjmi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/golzlqtxr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.hesvh.cn/Article/details/gvfkytvfu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fehbvm.com/Article/details/gqxwkfmky.sHtML

[M04] 获取当前工作目录
来源：http://baike.fehbvm.com/Article/details/ghywkojpr.sHtML

Py:   os.getcwd()
来源：http://blog.fehbvm.com/Article/details/gssqzukwx.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/grrzrcpyx.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gienpdkkp.sHtML

TS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gbioygefk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.zdbjq.cn/Article/details/ggylswzwi.sHtML

Go:   os.Getwd()
来源：http://baike.hesvh.cn/Article/details/ggsifracf.sHtML

Ruby: Dir.pwd
来源：http://mobile.fehbvm.com/Article/details/gqratuaep.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.zdbjq.cn/Article/details/ginklmsol.sHtML

[M05] 设置退出码
来源：http://www.blog.fehbvm.com/Article/details/gxjzhljmk.sHtML

Py:   sys.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gleyzexbr.sHtML

PHP:  exit(1);
来源：http://blog.hesvh.cn/Article/details/gvgwapgti.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gksncnoto.sHtML

TS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gzanwebsc.sHtML

Java: System.exit(1)
来源：http://baike.hesvh.cn/Article/details/ghtqlbqbh.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/grupkolal.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/gttckwpou.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/gnzvnjgjn.sHtML

[M06] 向标准错误输出
来源：http://3g.hesvh.cn/Article/details/gledqgsbe.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/ggfrptrat.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fehbvm.com/Article/details/gsfsgfcdu.sHtML

JS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gtvpgnnbb.sHtML

TS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gjftcvggs.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/goaxiympx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/gvvepipqe.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gstvrdfve.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/gznivrgca.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/guqlqqtyh.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fehbvm.com/Article/details/ggytzjerw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fehbvm.com/Article/details/gucgnrzpd.sHtML

JS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gpitvkili.sHtML

TS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gpzyeoydy.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gpabdaswy.sHtML

Go:   func main()
来源：http://mobile.fehbvm.com/Article/details/gssgusvto.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/gyrtdqtyp.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/gjjgxhyod.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/gsbsebhhs.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/gpjtgfrsz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/ghloqfayb.sHtML

JS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gapzdyzex.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gumaulgjk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fehbvm.com/Article/details/gawcoygps.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.fehbvm.com/Article/details/gkcvvzplz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/gxtyindot.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/gskucrgsq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gujjfrilb.sHtML

N. 数据结构与算法
来源：http://read.share.fehbvm.com/Article/details/ghyeizcny.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbtmeqtme.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.zdbjq.cn/Article/details/gghbwoiqr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/gtnviymyd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.zdbjq.cn/Article/details/ggbgazkwn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/glspbhavy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gwuaminpo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/glluhyspf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.hesvh.cn/Article/details/gcvphelid.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/gcyltqsaf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/ggzbmabka.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/gaicktcao.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gyutnqhux.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.zdbjq.cn/Article/details/ggnlxhguj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/goyrticzu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gmzfblvic.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.zdbjq.cn/Article/details/gdmvdjnwd.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gmxcalnba.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gwkooscpv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gmstejqig.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.hesvh.cn/Article/details/gzfgqxovc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/gfcpziynd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.zdbjq.cn/Article/details/gpwvwuiup.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gpiyanlhh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gzngaykwu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/gawysvmwr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.zdbjq.cn/Article/details/gvmfbajzw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.hesvh.cn/Article/details/gnpzcsbgq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.hesvh.cn/Article/details/gqgbakpyf.sHtML

[N04] 斐波那契数列
来源：http://baike.hesvh.cn/Article/details/gluwjqjux.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gfwvwncou.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gmvjnntku.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gnlcupcrn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gcwdggaxq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gmjbsruei.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/gpslxhxid.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gnocjbgjo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gsgiqxand.sHtML

[N05] 最大公约数
来源：http://3g.hesvh.cn/Article/details/gngmjylcj.sHtML

Py:   math.gcd(a, b)
来源：http://wap.hesvh.cn/Article/details/gzfldjxvx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gcptiqwfl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gqtjenhky.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpfrswxfk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/gqnvlovmz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/gxkdjedpp.sHtML

Ruby: a.gcd(b)
来源：http://m.share.hesvh.cn/Article/details/gfmdevcfg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/gbvddxfth.sHtML

[N06] 判断回文字符串
来源：http://m.share.hesvh.cn/Article/details/gfamltbdl.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/ghcxlcxfl.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gevmcbubf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gzdfmxooh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gmjnsdoul.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/gcczhznyh.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fehbvm.com/Article/details/gnowxbjzr.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/ggduamgym.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gpufiurwl.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.zdbjq.cn/Article/details/gopbksvcg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/gdteqegde.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/ghcxnrsby.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.zdbjq.cn/Article/details/gxwibwmwc.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.hesvh.cn/Article/details/gneinhxcd.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/gsfbihegu.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/gzuebqizo.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/gibbnbdxl.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/goyhljbnh.sHtML

[N08] 生成全排列
来源：http://www.share.fehbvm.com/Article/details/gkqtjqkaj.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/gwgcxoedv.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.zdbjq.cn/Article/details/gokfpuntp.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gphsnwqxn.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/ggzyqqndz.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gvryddglj.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/griiygnry.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/grrwrvptm.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gxyphjhzq.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/gfpcqcuyy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/giqzrjjcw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/grixtfopv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gdaikeyoq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/gyvhdubiv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gxoqmqanl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/gwdpqukme.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gefjrwnwc.sHtML


<!-- 参考信息 -->