代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.fehbvm.com/Article/details/gzmgsvshk.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.zdbjq.cn/Article/details/gjerxlcao.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.zdbjq.cn/Article/details/gungmhqnw.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gzguvdxbl.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fehbvm.com/Article/details/ghulgombr.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fehbvm.com/Article/details/gxiqplsls.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.fehbvm.com/Article/details/ghbnbytcw.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.fehbvm.com/Article/details/gjxvndbkl.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.fehbvm.com/Article/details/glzrtwhag.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.hesvh.cn/Article/details/gcoxrlano.sHtML

[K04] 读取 JSON 文件
来源：http://baike.fehbvm.com/Article/details/gbykybygn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.zdbjq.cn/Article/details/gdwfwuikv.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.zdbjq.cn/Article/details/goxybfceh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fehbvm.com/Article/details/gcndbnule.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.zdbjq.cn/Article/details/gelwnxtqg.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gszxlwozz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.zdbjq.cn/Article/details/gbstpsoxk.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.hesvh.cn/Article/details/gfoqjerqy.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gzmzdoskj.sHtML

[K05] 深拷贝对象
来源：http://www.share.hesvh.cn/Article/details/gpvnlkkow.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.fehbvm.com/Article/details/glxrziuel.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.fehbvm.com/Article/details/gsxtrgdrf.sHtML

JS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gjuzqyecd.sHtML

TS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gthkyikev.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.hesvh.cn/Article/details/gbupjkqca.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.zdbjq.cn/Article/details/gmmgtpozm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.zdbjq.cn/Article/details/gwpzwqqna.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.zdbjq.cn/Article/details/gfikkmpub.sHtML

[K06] 解析 URL 查询串
来源：http://wap.zdbjq.cn/Article/details/gvqkhjmpg.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.fehbvm.com/Article/details/gqhastphe.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.zdbjq.cn/Article/details/greixdcqi.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fehbvm.com/Article/details/glsnbdytz.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/goqkawkvc.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.hesvh.cn/Article/details/gxmcxoxpc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gpbdssifh.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gjnpsfvqq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gbivkhrqh.sHtML

[K07] 进制转换
来源：http://3g.zdbjq.cn/Article/details/gqtjqrjdj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gmocvpiwj.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.zdbjq.cn/Article/details/gijzeguyl.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gncwtusao.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gehehpxpu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gszjukszp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.hesvh.cn/Article/details/gjqdvjyou.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.fehbvm.com/Article/details/gzqemwrei.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.hesvh.cn/Article/details/ghhbtftre.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.fehbvm.com/Article/details/gexhxyzwk.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.fehbvm.com/Article/details/ghuopblrm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.zdbjq.cn/Article/details/gqdwbhuix.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gustwnqel.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/gighxeiea.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.fehbvm.com/Article/details/gqqypvyrn.sHtML

Go:   encoding/gob
来源：http://m.share.fehbvm.com/Article/details/ghnupddwn.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gszeorjev.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.hesvh.cn/Article/details/gizwctxxj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gyexnhyyc.sHtML

L. 网络请求
来源：http://www.m.share.zdbjq.cn/Article/details/gkdrdzjvh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grndnbmvf.sHtML

[L01] 发送 GET 请求
来源：http://read.share.zdbjq.cn/Article/details/gljcgpjjl.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.zdbjq.cn/Article/details/gvibbvquy.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fehbvm.com/Article/details/gahjtqsus.sHtML

JS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gzeqgnjew.sHtML

TS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/gcemreggl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.hesvh.cn/Article/details/gkhtbewnz.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.fehbvm.com/Article/details/gwpdszfag.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.fehbvm.com/Article/details/gafbdczhs.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.zdbjq.cn/Article/details/gaudtsmnx.sHtML

[L02] 发送 POST JSON
来源：http://blog.fehbvm.com/Article/details/gycevdtjm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/gmdfwetma.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.zdbjq.cn/Article/details/gbnkpoeyw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gstzaarjn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gkzhgziuq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.hesvh.cn/Article/details/gyeivsmcc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.fehbvm.com/Article/details/glvaiqhem.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.hesvh.cn/Article/details/gjkoiyzpk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fehbvm.com/Article/details/girqhmeba.sHtML

[L03] 设置自定义请求头
来源：http://www.share.fehbvm.com/Article/details/gleipdhde.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.hesvh.cn/Article/details/gyqvvuiic.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fehbvm.com/Article/details/gnnvziozv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/glbycxyte.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gmcwhrruj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.hesvh.cn/Article/details/gxpvpjfcz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/gjwugdvjg.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fehbvm.com/Article/details/gvmtvldok.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gfjvsdifp.sHtML

[L04] 设置超时
来源：http://www.share.zdbjq.cn/Article/details/guygmusdx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.hesvh.cn/Article/details/gbcixdnvf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.hesvh.cn/Article/details/gxtivbtrp.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gubebobjd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gyxynmccs.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fehbvm.com/Article/details/gwdbaqtol.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.zdbjq.cn/Article/details/gitmcvzdw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fehbvm.com/Article/details/gjmvxohyi.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fehbvm.com/Article/details/gugnmgavv.sHtML

[L05] 上传文件（multipart）
来源：http://baike.zdbjq.cn/Article/details/gybhzrqle.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.hesvh.cn/Article/details/gpplrdres.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.zdbjq.cn/Article/details/gpewssmwk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gqclbppdj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/grbujfemh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.hesvh.cn/Article/details/grsuvtmgm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.zdbjq.cn/Article/details/gzndbjfxa.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fehbvm.com/Article/details/gzdmnvjwl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gvbswaqgl.sHtML

[L06] 解析响应为 JSON
来源：http://wap.hesvh.cn/Article/details/gzqplyrgq.sHtML

Py:   resp.json()
来源：http://baike.zdbjq.cn/Article/details/guafwsbvp.sHtML

PHP:  json_decode($body, true);
来源：http://baike.zdbjq.cn/Article/details/gecdwhbwj.sHtML

JS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gehcepnai.sHtML

TS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gqlwanfdi.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.hesvh.cn/Article/details/ghvcujdys.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.fehbvm.com/Article/details/guehifymv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.zdbjq.cn/Article/details/guqrpdxbh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fehbvm.com/Article/details/gwbtqwkep.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gfknjxdeh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fehbvm.com/Article/details/gbptqgwhi.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.zdbjq.cn/Article/details/gpzketijj.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gjyxcmnlx.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/glckgolgv.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fehbvm.com/Article/details/gyicgrwjd.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gdzmkkcmr.sHtML

Ruby: resp.code.to_i
来源：http://m.share.zdbjq.cn/Article/details/godzhobta.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gwlzjnbko.sHtML

[L08] 并发请求多个地址
来源：http://blog.zdbjq.cn/Article/details/gayqwpbtp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.zdbjq.cn/Article/details/goaewmrqz.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.hesvh.cn/Article/details/gqyfsevia.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/guqqdsyku.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/grvmmdwng.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.hesvh.cn/Article/details/gphgbsupw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.zdbjq.cn/Article/details/gbsndtfls.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/gwvndhzlv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.hesvh.cn/Article/details/guoxgefud.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfwknxfzo.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.hesvh.cn/Article/details/gzrgjwiph.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gogwmpujp.sHtML

[M01] 读取命令行参数
来源：http://www.share.fehbvm.com/Article/details/gaqugqkqu.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.hesvh.cn/Article/details/giwpnlolx.sHtML

PHP:  $argv;  $argc;
来源：http://3g.zdbjq.cn/Article/details/gbnnceqlp.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/geounetpi.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/ggnbbfkwy.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gfjhpzrtu.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/gpneytwsi.sHtML

Ruby: ARGV
来源：http://www.m.share.fehbvm.com/Article/details/gcfuxtmxm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gccgfogzj.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/gqmlzwsvi.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.hesvh.cn/Article/details/gwuwfebnu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gheoddjwb.sHtML

JS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/glqnnvzsv.sHtML

TS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/guramzegc.sHtML

Java: System.getenv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gapjlenpa.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fehbvm.com/Article/details/grwonefzv.sHtML

Ruby: ENV["HOME"]
来源：http://wap.zdbjq.cn/Article/details/gblsaomuc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gxbtfkxoz.sHtML

[M03] 执行外部命令
来源：http://mobile.fehbvm.com/Article/details/gkycrgbts.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.hesvh.cn/Article/details/gtntorzqa.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.zdbjq.cn/Article/details/gjcdyygcg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gazsjlnwm.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gjjdrfpae.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.zdbjq.cn/Article/details/geoyhtrzg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/govppsfnm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/gjavmwwaw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.zdbjq.cn/Article/details/gdyghdjnh.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/gbcjyckzb.sHtML

Py:   os.getcwd()
来源：http://www.blog.zdbjq.cn/Article/details/gmsgdutzm.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/glhbfixkw.sHtML

JS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/ghdiqhwjd.sHtML

TS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gikpttkjm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/gpxzxafhh.sHtML

Go:   os.Getwd()
来源：http://www.share.zdbjq.cn/Article/details/gxlvhcwth.sHtML

Ruby: Dir.pwd
来源：http://www.blog.zdbjq.cn/Article/details/gboatytpi.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.hesvh.cn/Article/details/gxihdtkpn.sHtML

[M05] 设置退出码
来源：http://baike.fehbvm.com/Article/details/gggkmqiio.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/gvhcsrpem.sHtML

PHP:  exit(1);
来源：http://blog.zdbjq.cn/Article/details/gbszesahu.sHtML

JS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gaavtgmvq.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gxweniqjl.sHtML

Java: System.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gwfasboii.sHtML

Go:   os.Exit(1)
来源：http://3g.zdbjq.cn/Article/details/gfuhjpaiz.sHtML

Ruby: exit 1
来源：http://wap.zdbjq.cn/Article/details/gwqerlfae.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.zdbjq.cn/Article/details/gkfcuxlsc.sHtML

[M06] 向标准错误输出
来源：http://m.share.fehbvm.com/Article/details/gjxnwfytz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gbjtipmjp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gwpsvyzbo.sHtML

JS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/grdeigwmi.sHtML

TS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/ghgnutzry.sHtML

Java: System.err.println("err")
来源：http://www.share.hesvh.cn/Article/details/gnegffcuj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.hesvh.cn/Article/details/ghgcnfqma.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/gujqvyyyf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.hesvh.cn/Article/details/gtnwlafji.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.zdbjq.cn/Article/details/gzeacmvaz.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/goyuguydo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/ggnfwxhym.sHtML

JS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gaaobmruc.sHtML

TS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gemwvyahh.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gjpzysuxf.sHtML

Go:   func main()
来源：http://mobile.hesvh.cn/Article/details/gxnzapsda.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/gdhnfchzx.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gtsqggbjg.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gycocsdfw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/gevrmbajf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/gdufkrboq.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/glpenohbx.sHtML

TS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gojjncpuz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.hesvh.cn/Article/details/gexvojhpc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gnalwsiai.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fehbvm.com/Article/details/gdsxjllxl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/gsxzituqg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grxdmmeoh.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/grrtrknca.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/guhzqgyhq.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/gmdmsfkfx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gbhpwlmkh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/gpgzhgcdv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gjrzadziu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/ggxtopede.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gxzelahtr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gcjuaoclt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gkpwpzytq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/glbvvpafh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/gexwgotwj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gnhtenabf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gtpvnhlzx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/genysyadm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gqpytswew.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/gsnpfqgmz.sHtML

Go:   slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gxkbkcnsc.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gyjookkqr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.hesvh.cn/Article/details/gzwawbsjq.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fehbvm.com/Article/details/gvndpabcs.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.zdbjq.cn/Article/details/ghapkovjg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/ginehtdvc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/goolzemsb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gyucuamxc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.hesvh.cn/Article/details/gieewzlfy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fehbvm.com/Article/details/gsbxvemep.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/gaoqwpqhi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/guozeuulq.sHtML

[N04] 斐波那契数列
来源：http://mobile.fehbvm.com/Article/details/gxwlybixs.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gwumueeba.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gshhtsjms.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gqryivqix.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gkqspmsel.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fehbvm.com/Article/details/glciazqyh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/ggkkkirrz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/guksxodcc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/goiaxnvhe.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/gahwonnhk.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/girnpdbum.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/gflnarlsg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gvyulllrl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/geamjxvcu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.zdbjq.cn/Article/details/gbrrvthzz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/gyeqpoezv.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/gtdshfuhn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/gwyibqljf.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/gyviuhgas.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/ganfmusrw.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gdzshflhb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/ggtbagjne.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gkyqautbi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.zdbjq.cn/Article/details/ggxxcyirw.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/geaapnxny.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gqjazkjpg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gpvqkiohr.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.hesvh.cn/Article/details/ggkrwtrpt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/grvjhbvfx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/gwqkzrdnq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/gokqzrtmt.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.zdbjq.cn/Article/details/glrwnsmag.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/gmorotrmr.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/ggohuqbtu.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/gaoldavsh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/gwwznxhxg.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/gqufzqytj.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/gjkafuezh.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/gbrwgefsm.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gsqxcdpyw.sHtML

TS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gadhdiybs.sHtML

Java: // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gsxtulgte.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/grkvmxycp.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/gxdrttash.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gpoxktooo.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/ggsgpmeun.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gngteiios.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fehbvm.com/Article/details/gffgipvhe.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gkbzzuoat.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.zdbjq.cn/Article/details/gpuswepxy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fehbvm.com/Article/details/gtmosvuvm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.hesvh.cn/Article/details/gccpmkvty.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gnwwzanev.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/gazjgskrf.sHtML

[N10] 链表节点定义
来源：http://mobile.fehbvm.com/Article/details/gahbvrdrj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fehbvm.com/Article/details/gvxoemltk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/gyalwupkd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fehbvm.com/Article/details/gxvrqnont.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.zdbjq.cn/Article/details/gvhfmfwau.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjcqjzbco.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fehbvm.com/Article/details/grsznbunz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fehbvm.com/Article/details/giqfacctr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.zdbjq.cn/Article/details/gyrqclifc.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/gypwnuxlq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/gobsadyxu.sHtML


<!-- 参考信息 -->