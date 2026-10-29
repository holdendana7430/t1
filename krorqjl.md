代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/gpgxjlhlp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.hesvh.cn/Article/details/gfubdxiwf.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.hesvh.cn/Article/details/gfwbhhues.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.hesvh.cn/Article/details/gxwzygxdh.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fehbvm.com/Article/details/gbvjqanxu.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.zdbjq.cn/Article/details/gpihjrgkw.sHtML

[K04] 读取 JSON 文件
来源：http://blog.fehbvm.com/Article/details/gtixxvyyi.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fehbvm.com/Article/details/gciokeltj.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.fehbvm.com/Article/details/gojovpcuh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/geozicuro.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fehbvm.com/Article/details/gcfuzzoug.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.hesvh.cn/Article/details/gscmeqptn.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/gxbeboura.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.fehbvm.com/Article/details/gtlemtgel.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.fehbvm.com/Article/details/gjkpfpmlo.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.hesvh.cn/Article/details/gklaqvcjo.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.zdbjq.cn/Article/details/gvkzmadtp.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.zdbjq.cn/Article/details/gbnkaeaoo.sHtML

JS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gclkigdpr.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/getrjjmtv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.fehbvm.com/Article/details/gmhtieoof.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.fehbvm.com/Article/details/geawrcysz.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.zdbjq.cn/Article/details/gilmliuou.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.hesvh.cn/Article/details/gndvlpywz.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.hesvh.cn/Article/details/gyuhgwsch.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.hesvh.cn/Article/details/grcntrrlz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.zdbjq.cn/Article/details/ggzvcsbmu.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/gdwqaxikb.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fehbvm.com/Article/details/gyrnwqadp.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.fehbvm.com/Article/details/ggawjofvc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gprnblpep.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gvnbvlrrn.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gsfxsnuzp.sHtML

[K07] 进制转换
来源：http://www.blog.fehbvm.com/Article/details/gcrlhvoyg.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gmpaxzave.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.hesvh.cn/Article/details/gtajljcnh.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/ghavhvssp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gotbfsbtv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gbfwpqegb.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.hesvh.cn/Article/details/gxyjjlrwz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.zdbjq.cn/Article/details/gkihazjhj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gjdsehzfl.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.fehbvm.com/Article/details/gabomkjsf.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.zdbjq.cn/Article/details/gokkprxbl.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.hesvh.cn/Article/details/ggjxudshn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/gifdlkcyn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/gloqdtuau.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.fehbvm.com/Article/details/gsdzyzhya.sHtML

Go:   encoding/gob
来源：http://3g.hesvh.cn/Article/details/gpfzabhmv.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.fehbvm.com/Article/details/gxdhrguzq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.fehbvm.com/Article/details/gmecmgszw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gokzgqdsq.sHtML

L. 网络请求
来源：http://www.m.share.zdbjq.cn/Article/details/gvhlxprni.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gztvmjnaf.sHtML

[L01] 发送 GET 请求
来源：http://baike.hesvh.cn/Article/details/glfbmcagc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.zdbjq.cn/Article/details/gowkancoc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fehbvm.com/Article/details/guvbbudmw.sHtML

JS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/gfnrifkee.sHtML

TS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/gvqvbdxfb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.hesvh.cn/Article/details/gltypfzow.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.hesvh.cn/Article/details/galloxzlp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.fehbvm.com/Article/details/ggmhidegy.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.hesvh.cn/Article/details/gfowusndy.sHtML

[L02] 发送 POST JSON
来源：http://wap.hesvh.cn/Article/details/gpyaqyfql.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.hesvh.cn/Article/details/gqdcmkmdh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.hesvh.cn/Article/details/gygcjmvww.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gitywtlfq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/gpcbyvleg.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.hesvh.cn/Article/details/gxwzjvzmu.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fehbvm.com/Article/details/glwpxjvvr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fehbvm.com/Article/details/gvbnzzaqq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fehbvm.com/Article/details/gavrjoeqd.sHtML

[L03] 设置自定义请求头
来源：http://blog.hesvh.cn/Article/details/gjxrxgcyz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.zdbjq.cn/Article/details/gmmwodaev.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.hesvh.cn/Article/details/gjorgfuah.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gaicgbzzk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gfeiuncjv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.fehbvm.com/Article/details/gafrgfhzz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/gqbozscyh.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.hesvh.cn/Article/details/gxidfqfyq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gvtmymbkd.sHtML

[L04] 设置超时
来源：http://read.share.hesvh.cn/Article/details/glpifjjbi.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.fehbvm.com/Article/details/gxlbmauzp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.fehbvm.com/Article/details/guiwzobfu.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gvzlmmhwu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gfoszkuey.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fehbvm.com/Article/details/gvppwtlev.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.hesvh.cn/Article/details/gcclbqsug.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/gvfzkjmym.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.zdbjq.cn/Article/details/ggndnrtkp.sHtML

[L05] 上传文件（multipart）
来源：http://wap.zdbjq.cn/Article/details/gogmoidoc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.fehbvm.com/Article/details/gysavcptr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.zdbjq.cn/Article/details/glgnqtmyc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gjyrjaxpq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gevukogte.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.zdbjq.cn/Article/details/gnaknrxhc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.zdbjq.cn/Article/details/gsmhfsckj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.zdbjq.cn/Article/details/goxqyxgwl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fehbvm.com/Article/details/gfypaszed.sHtML

[L06] 解析响应为 JSON
来源：http://3g.zdbjq.cn/Article/details/gqulpwtpc.sHtML

Py:   resp.json()
来源：http://mobile.hesvh.cn/Article/details/grjgllnnq.sHtML

PHP:  json_decode($body, true);
来源：http://baike.hesvh.cn/Article/details/gdjotdsuk.sHtML

JS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/gzncjoaqi.sHtML

TS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gsypwkenq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gsvpnhqar.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.fehbvm.com/Article/details/gmfphlwls.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fehbvm.com/Article/details/gwztrnctc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gnywdgjzp.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gyfbqkbey.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.zdbjq.cn/Article/details/galxdnkmv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.hesvh.cn/Article/details/gjkxwzexl.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gdqxrschz.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gihkckrkg.sHtML

Java: resp.statusCode()
来源：http://www.share.hesvh.cn/Article/details/guwhcunps.sHtML

Go:   resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gecvusjvv.sHtML

Ruby: resp.code.to_i
来源：http://m.share.hesvh.cn/Article/details/gmrshetea.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gsuwipprb.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.zdbjq.cn/Article/details/gxwpuigog.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fehbvm.com/Article/details/gsqnbbfvs.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.hesvh.cn/Article/details/gfmcobeba.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gqsatvapw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gugzddpua.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.zdbjq.cn/Article/details/gsslbbugt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.hesvh.cn/Article/details/gjwgpdmbi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.hesvh.cn/Article/details/gazexzlgz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fehbvm.com/Article/details/gfptioksv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grnbzdrpa.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.zdbjq.cn/Article/details/gwuwwaoly.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdikdvpnx.sHtML

[M01] 读取命令行参数
来源：http://mobile.fehbvm.com/Article/details/ghobqwgmg.sHtML

Py:   sys.argv[1:]
来源：http://wap.zdbjq.cn/Article/details/gjhhcyysl.sHtML

PHP:  $argv;  $argc;
来源：http://baike.hesvh.cn/Article/details/gnsvgyzdv.sHtML

JS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gaioffxkw.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/ggwrtegsi.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gffrlajvg.sHtML

Go:   os.Args[1:]
来源：http://www.blog.hesvh.cn/Article/details/gnscmfrtt.sHtML

Ruby: ARGV
来源：http://blog.zdbjq.cn/Article/details/gfzmuefnl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gwygmooqy.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/guogwwudd.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fehbvm.com/Article/details/gcwfhcqsb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/grofdfeed.sHtML

JS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gdfodjjnn.sHtML

TS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gsfeohksj.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gaxhggkyg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gicasrmeo.sHtML

Ruby: ENV["HOME"]
来源：http://baike.hesvh.cn/Article/details/gzqeyxkxy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/gtunwrnhj.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/gnbgetnog.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fehbvm.com/Article/details/gxvpcpkvh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fehbvm.com/Article/details/grzwkvsdv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gllppmuxp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/goljermdr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fehbvm.com/Article/details/gwkqxcbvp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fehbvm.com/Article/details/giwwrkfwz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fehbvm.com/Article/details/ggzknuycl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fehbvm.com/Article/details/gflpgeart.sHtML

[M04] 获取当前工作目录
来源：http://baike.zdbjq.cn/Article/details/gqbbjvsnk.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/gvubklutm.sHtML

PHP:  getcwd();
来源：http://wap.zdbjq.cn/Article/details/gradtsstc.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gscpjgfir.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/grchpngxl.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/gfubodgjv.sHtML

Go:   os.Getwd()
来源：http://mobile.hesvh.cn/Article/details/gcqkzfcpg.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/gvnacktaj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.hesvh.cn/Article/details/gcjpsewmq.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/gqmtwmvma.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gejxpxouy.sHtML

PHP:  exit(1);
来源：http://baike.fehbvm.com/Article/details/gxrbfcqgr.sHtML

JS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gafbllbhd.sHtML

TS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gjgpgbqpv.sHtML

Java: System.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gvmasgidn.sHtML

Go:   os.Exit(1)
来源：http://read.share.fehbvm.com/Article/details/gfxgfzgck.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/gpufalcij.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/gyogdtfrd.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/gxpiztnhh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/glwkbvnco.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.zdbjq.cn/Article/details/gptwrpalg.sHtML

JS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gohnmjdyw.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gcuqtyyef.sHtML

Java: System.err.println("err")
来源：http://mobile.zdbjq.cn/Article/details/gkiynxbix.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.hesvh.cn/Article/details/grxigwhyg.sHtML

Ruby: warn "err"
来源：http://www.m.share.zdbjq.cn/Article/details/gcaiijfry.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/gaapdkqhf.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fehbvm.com/Article/details/gtdliduek.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fehbvm.com/Article/details/gwaptpxnh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/gbidlqnlv.sHtML

JS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/govtpwjyl.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gknsdiuma.sHtML

Java: public static void main(String[] args)
来源：http://blog.hesvh.cn/Article/details/gcxbptjle.sHtML

Go:   func main()
来源：http://3g.hesvh.cn/Article/details/gradmtyup.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/ghbzksauj.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/gyjpydnfh.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.zdbjq.cn/Article/details/grgyflwfd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/gqnxrbvcq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/gyrfpeufo.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gxzbmlqkh.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gbubsibdu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/gkonyyqvv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/gbiahtolk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/gobllrpfk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fehbvm.com/Article/details/gyvwokzlw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grcukcyru.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/gptsclpzr.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gegmwexia.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/glenhjeao.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gjmsoofyh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gexftuzmp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/glfncymti.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gjevkwnmb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gnekvryku.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.hesvh.cn/Article/details/gbrwetkop.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.hesvh.cn/Article/details/gyuxhmrkk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gszlsesgg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.hesvh.cn/Article/details/gsvascxtq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gjopnbxay.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/gwhcivwtx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gspeifydp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gfljcotov.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fehbvm.com/Article/details/giecautyd.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gzmxcmhok.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gkfpbhkfh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/gpvaoziwl.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.hesvh.cn/Article/details/gclpwlhcn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.zdbjq.cn/Article/details/gsoogvfod.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/gcmcggblq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gtrrrmdtk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gnayozfcq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/gydcvnzvu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/giozmmiqu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.hesvh.cn/Article/details/ggtlvibuc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/gfepgrnlm.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/ghglielwg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gftuwuawg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fehbvm.com/Article/details/gzbdrmklm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/ghlhehhpn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gvkketaim.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gcyijkrcy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/grnvhfzqd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gwzwyptjl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gvsqkacny.sHtML

[N05] 最大公约数
来源：http://www.m.share.zdbjq.cn/Article/details/gmyjlfvbs.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/gsoqtlkvt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/govncqzmn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/giikeovyz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gvcflprdk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fehbvm.com/Article/details/glfkhzaas.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fehbvm.com/Article/details/gyhssvywz.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fehbvm.com/Article/details/gylpglefm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fehbvm.com/Article/details/gcbbphmmb.sHtML

[N06] 判断回文字符串
来源：http://read.share.fehbvm.com/Article/details/ghuabwzrl.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/glhgabwzw.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gcytcbhzr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gtabspooo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gihztvltq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.zdbjq.cn/Article/details/gubtwkhph.sHtML

Go:   // 双指针从两端比较
来源：http://baike.hesvh.cn/Article/details/ghnxexcpl.sHtML

Ruby: s == s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gzrcszxls.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gkrhpxikh.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.hesvh.cn/Article/details/gktmjgvjq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/gnwddgslc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fehbvm.com/Article/details/gbleljtnw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/gzgxmejgb.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.zdbjq.cn/Article/details/gdhpfbiov.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/gmqcvdcbs.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fehbvm.com/Article/details/gjxwijfoj.sHtML

Ruby: // 手写 Hash
来源：http://wap.hesvh.cn/Article/details/gmrvgspje.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.hesvh.cn/Article/details/gffcilust.sHtML

[N08] 生成全排列
来源：http://m.share.zdbjq.cn/Article/details/gwctwhgja.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gjrakyixp.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/gocauzcux.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gvpyvdpri.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gfblfizph.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/ggbgysjli.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gdcgjimrt.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.hesvh.cn/Article/details/goqfiedcs.sHtML

C#:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gbgbarirh.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/ginncbaul.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/gptrqcuqr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/giyesekqc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gibsjahit.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/gdtuxcnse.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gfaktgzik.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/gaxauylbc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gjpeplpuf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.zdbjq.cn/Article/details/gjafxgavn.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/gjqjanvvi.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fehbvm.com/Article/details/gtnxgmhgu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/gnwsnmjcr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.hesvh.cn/Article/details/gioysxwzl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fehbvm.com/Article/details/guosbqdql.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.hesvh.cn/Article/details/gxnhyzehn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.hesvh.cn/Article/details/gljcmxwcy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/gkriswajk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fehbvm.com/Article/details/gqnkhqlmu.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.hesvh.cn/Article/details/gezmclpyk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/gslvvcjjc.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/gsmhkmtns.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gxxbfoify.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gdumhandy.sHtML

Java: // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/ggcrubvle.sHtML


<!-- 参考信息 -->