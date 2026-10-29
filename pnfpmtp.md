代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.zdbjq.cn/Article/details/gfdqrnusb.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.fehbvm.com/Article/details/guwaitrxf.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.hesvh.cn/Article/details/gvxkhgswu.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.hesvh.cn/Article/details/gtsdelenv.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fehbvm.com/Article/details/gbazqmilr.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.hesvh.cn/Article/details/glifwyuiu.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.zdbjq.cn/Article/details/gsdmzwdjo.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.hesvh.cn/Article/details/gupmypuoj.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.fehbvm.com/Article/details/gzgtygzeu.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.zdbjq.cn/Article/details/gmfybkqjd.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.fehbvm.com/Article/details/gjffvqasf.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.zdbjq.cn/Article/details/gmtropite.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.zdbjq.cn/Article/details/gpjjxopdv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/grenwbnom.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.hesvh.cn/Article/details/gjvfgnjsp.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gaafdrnxk.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.zdbjq.cn/Article/details/gwfpyfdde.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.fehbvm.com/Article/details/glbucmzwn.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.fehbvm.com/Article/details/grqeaqjcm.sHtML

[K05] 深拷贝对象
来源：http://3g.fehbvm.com/Article/details/gficmbnea.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.hesvh.cn/Article/details/gazzqzoav.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.hesvh.cn/Article/details/gmjgdyrnb.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/geooijgty.sHtML

TS:   structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gdmybkwnz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.zdbjq.cn/Article/details/gkygwhwtm.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.hesvh.cn/Article/details/gwcusjxsc.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.zdbjq.cn/Article/details/gpjrzeqny.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.hesvh.cn/Article/details/grwkavpum.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.fehbvm.com/Article/details/ggnejeggi.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.hesvh.cn/Article/details/gpupctnpv.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.fehbvm.com/Article/details/gksdrnqyq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fehbvm.com/Article/details/givjawdyh.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/gtiildcfk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.zdbjq.cn/Article/details/gbinwtoeu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gahcnzsho.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gzzzwzzzh.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gfxwahcbr.sHtML

[K07] 进制转换
来源：http://blog.zdbjq.cn/Article/details/gvekeelys.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gstfzejqn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.hesvh.cn/Article/details/gztpbdhha.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/guuejpenh.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gqjdyzepj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gxgweilum.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.zdbjq.cn/Article/details/gffbulyiu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.fehbvm.com/Article/details/gzupvidik.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gwnjepzrs.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.fehbvm.com/Article/details/gehcjjvcf.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.hesvh.cn/Article/details/gzyhiwrtz.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.fehbvm.com/Article/details/gfejsewxl.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.hesvh.cn/Article/details/gjceldsni.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.hesvh.cn/Article/details/gtdpjkips.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.hesvh.cn/Article/details/gxjvddjwv.sHtML

Go:   encoding/gob
来源：http://read.share.zdbjq.cn/Article/details/gxpmfqadl.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.zdbjq.cn/Article/details/gagyhhrid.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/ghpmionhx.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gnxaulpxh.sHtML

L. 网络请求
来源：http://read.share.zdbjq.cn/Article/details/gdimdpoft.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggvdnytsp.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.fehbvm.com/Article/details/gdajehhjw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.hesvh.cn/Article/details/gfnofmnsz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.hesvh.cn/Article/details/gfeljtqmu.sHtML

JS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/getncbasl.sHtML

TS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/gfnkvnvzy.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.fehbvm.com/Article/details/gjzbzdaiz.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.hesvh.cn/Article/details/gbxrhrbfo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.hesvh.cn/Article/details/ghcdyijth.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.zdbjq.cn/Article/details/glhyfhmmt.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gpnjnjtwz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gktjqckre.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.hesvh.cn/Article/details/gnwbbkhot.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gksceehtf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/gjldohtbj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gduxgegub.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.zdbjq.cn/Article/details/glhoqfujc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.hesvh.cn/Article/details/gedcpzmxe.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.zdbjq.cn/Article/details/glfnhbbif.sHtML

[L03] 设置自定义请求头
来源：http://baike.zdbjq.cn/Article/details/gypagivfb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.zdbjq.cn/Article/details/gqvlnjvib.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.fehbvm.com/Article/details/gpftdiiih.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/gmkfpgroc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gbaevqwvj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.hesvh.cn/Article/details/gebmzepsm.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/ggjuhagfr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.hesvh.cn/Article/details/gputexsfc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gagvitrck.sHtML

[L04] 设置超时
来源：http://wap.hesvh.cn/Article/details/gqnniiqmq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fehbvm.com/Article/details/grjmspgrz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.zdbjq.cn/Article/details/gkuifspoz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gpmkimvmb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gbjkqthoi.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.zdbjq.cn/Article/details/gtjddffmx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fehbvm.com/Article/details/gbaehvtaz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.hesvh.cn/Article/details/gxdmdlebg.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.zdbjq.cn/Article/details/gunmyxoaf.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.zdbjq.cn/Article/details/gdvikxbio.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fehbvm.com/Article/details/gfegeysby.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.zdbjq.cn/Article/details/gihuqipsb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gzakmjebj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/ginhsisjk.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.hesvh.cn/Article/details/guuicypuj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.hesvh.cn/Article/details/gegktbgjh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.zdbjq.cn/Article/details/gzeoklhhq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.zdbjq.cn/Article/details/giurwxsfh.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fehbvm.com/Article/details/gzrafpwqf.sHtML

Py:   resp.json()
来源：http://3g.hesvh.cn/Article/details/gqevegcfg.sHtML

PHP:  json_decode($body, true);
来源：http://3g.hesvh.cn/Article/details/ggqsnfmnp.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gftqntpww.sHtML

TS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gxjvmzaeq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.hesvh.cn/Article/details/gwrksyzcv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.hesvh.cn/Article/details/gtujuhvhe.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fehbvm.com/Article/details/gozkodoac.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.zdbjq.cn/Article/details/gkznqiygd.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gajingvgo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.zdbjq.cn/Article/details/gfkblsmgx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.fehbvm.com/Article/details/glcundzrs.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gvyhxkbke.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/giirtbjuk.sHtML

Java: resp.statusCode()
来源：http://m.share.fehbvm.com/Article/details/ggckduhud.sHtML

Go:   resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gosvgmcbj.sHtML

Ruby: resp.code.to_i
来源：http://blog.hesvh.cn/Article/details/gnddnglos.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gsoadlnqa.sHtML

[L08] 并发请求多个地址
来源：http://www.share.zdbjq.cn/Article/details/gnvtnhviv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fehbvm.com/Article/details/gcenvphdm.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.hesvh.cn/Article/details/grcsnpelf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gnohwogpn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/grlsboorp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fehbvm.com/Article/details/goloosijy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.zdbjq.cn/Article/details/gdyrmvsvg.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.hesvh.cn/Article/details/gyhrhcjzl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fehbvm.com/Article/details/ggitxxsrr.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gofvigjlt.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fehbvm.com/Article/details/gfyhshjmn.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghdefqvlc.sHtML

[M01] 读取命令行参数
来源：http://mobile.zdbjq.cn/Article/details/guhsjslpb.sHtML

Py:   sys.argv[1:]
来源：http://baike.zdbjq.cn/Article/details/gkzyrblug.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fehbvm.com/Article/details/gdmtpoqhl.sHtML

JS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gjiyhywfc.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gtfakizbc.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gmeaufobr.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gcgaxkpgv.sHtML

Ruby: ARGV
来源：http://m.share.fehbvm.com/Article/details/gpvqujiid.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gylvstyac.sHtML

[M02] 读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/ghhidkuyl.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.zdbjq.cn/Article/details/geyhhmoez.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/gkryivhme.sHtML

JS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gktswllea.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gjqguxuow.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gspaoxqpx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gejiteynt.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fehbvm.com/Article/details/gvribileo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gpawovhux.sHtML

[M03] 执行外部命令
来源：http://blog.hesvh.cn/Article/details/gerutkmvs.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fehbvm.com/Article/details/goduekzfz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fehbvm.com/Article/details/gkkgesrey.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/ghmntoekt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/grkftbzuj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fehbvm.com/Article/details/gsgdbrlga.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fehbvm.com/Article/details/ggjpssvek.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fehbvm.com/Article/details/guqcbyvsw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.hesvh.cn/Article/details/gbiaymqgu.sHtML

[M04] 获取当前工作目录
来源：http://baike.hesvh.cn/Article/details/gtqjaqipz.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/ghhpyxupq.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/gavopuamw.sHtML

JS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/geusjlzkw.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gtadhfeby.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.zdbjq.cn/Article/details/gkeagtxns.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/ggwjkorar.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.hesvh.cn/Article/details/gzkbakdjk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fehbvm.com/Article/details/gykpdglyj.sHtML

[M05] 设置退出码
来源：http://www.share.zdbjq.cn/Article/details/gmksqswlv.sHtML

Py:   sys.exit(1)
来源：http://3g.fehbvm.com/Article/details/gpsrdadck.sHtML

PHP:  exit(1);
来源：http://read.share.fehbvm.com/Article/details/gjbyioqnf.sHtML

JS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gvaifbbfl.sHtML

TS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gxivukarc.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gxtdxioih.sHtML

Go:   os.Exit(1)
来源：http://baike.hesvh.cn/Article/details/gpzpkrfav.sHtML

Ruby: exit 1
来源：http://wap.zdbjq.cn/Article/details/gjtenzufc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/gwozoekht.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/gngsrfuvg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gnxkykoek.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.hesvh.cn/Article/details/gckrsuaij.sHtML

JS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gpseannwe.sHtML

TS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gcvbeqyij.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/gmvmzboik.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fehbvm.com/Article/details/gdawkmuit.sHtML

Ruby: warn "err"
来源：http://www.share.zdbjq.cn/Article/details/gkjhqkzxg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/gkxvdmnxk.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/gmjsyoxkg.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.hesvh.cn/Article/details/gstgkypkx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.zdbjq.cn/Article/details/guxyqwyuw.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gdpjdzskh.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gocjbzyoc.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/gtwkhhnzq.sHtML

Go:   func main()
来源：http://read.share.zdbjq.cn/Article/details/gmxmpegbb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.hesvh.cn/Article/details/gbphzhpba.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/gwvpyccan.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fehbvm.com/Article/details/gwjrzwtqc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.zdbjq.cn/Article/details/gqbtudmug.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/gvvygusrj.sHtML

JS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gklridnpr.sHtML

TS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/guadpmvsk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/gfjzlhoyq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.zdbjq.cn/Article/details/goajoblpr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/gjaxrslbe.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.zdbjq.cn/Article/details/gqbbagzsw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gujyfrpob.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/gpxxcmrea.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gklfzhgcb.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fehbvm.com/Article/details/gxlfjdamp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gpldzbmez.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fehbvm.com/Article/details/gdqsxdpmt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gzvtuewft.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gkerqhoyb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/ggedkvozn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fehbvm.com/Article/details/ggsdszels.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/gssvdhcrp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gjnmspkqq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.zdbjq.cn/Article/details/ghhvjbqeg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gvhbmhmab.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fehbvm.com/Article/details/gwxxwqsrn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/giurcdgbi.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gyrkuzows.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.zdbjq.cn/Article/details/gxudhbeml.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gpeevpbkd.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gdbpkrflg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.zdbjq.cn/Article/details/ggommrpfn.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.hesvh.cn/Article/details/gqtpwkcjt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fehbvm.com/Article/details/gycctawef.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fehbvm.com/Article/details/glcavbtza.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gsyfulneb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gvkdkwexn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.hesvh.cn/Article/details/gtzpvptni.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.zdbjq.cn/Article/details/gcnktfqnb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/grmvptirz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/gojnbpqjp.sHtML

[N04] 斐波那契数列
来源：http://m.share.fehbvm.com/Article/details/gnikjalhu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gaobsyhhc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/gxjshfgaj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/ggnzojvvs.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gjzhpegjc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gcbeujqyp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/gxjvomtqp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/ggygxdplq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gcyhauckg.sHtML

[N05] 最大公约数
来源：http://3g.fehbvm.com/Article/details/grrmqaujn.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.hesvh.cn/Article/details/gwcxgsntw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gmnlxlrps.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gaqgmxqxs.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwnwxlody.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/gxdqqkayt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gkqtxmxux.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gixpvdpto.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.zdbjq.cn/Article/details/gphkwkgjw.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/ghtwftigv.sHtML

Py:   s == s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gdneahhqu.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fehbvm.com/Article/details/glmyipmpc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gcgwvpjtu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gykpxxdnq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/gforcxlor.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/gfkstmenw.sHtML

Ruby: s == s.reverse
来源：http://3g.zdbjq.cn/Article/details/gxatsplhr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/govvvmkct.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.hesvh.cn/Article/details/gcsfugyxb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.hesvh.cn/Article/details/gbboujxyq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.hesvh.cn/Article/details/gsizvqopt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fehbvm.com/Article/details/glvbcdsge.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.hesvh.cn/Article/details/gokquuriz.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/gnbehoapa.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.zdbjq.cn/Article/details/gjhrgpgav.sHtML

Ruby: // 手写 Hash
来源：http://wap.hesvh.cn/Article/details/gwzzdjzhn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gcxzipehh.sHtML

[N08] 生成全排列
来源：http://mobile.hesvh.cn/Article/details/gsxcxjkej.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.zdbjq.cn/Article/details/gtpfrmhvu.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/gfvdqpwcb.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/grxuhzaqv.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gsdgpzmqx.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/glecwsuzt.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/guzavydwz.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fehbvm.com/Article/details/girqxreip.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gnhbdnonc.sHtML

[N09] 栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gmgmkelmc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gfbvvkdap.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.hesvh.cn/Article/details/ghatuzaoe.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gfubfttwr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/gzvewevjr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/gcrthsoeq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.zdbjq.cn/Article/details/gndphtcwd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gzuwjvuio.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/gcuhqajjw.sHtML

[N10] 链表节点定义
来源：http://www.share.fehbvm.com/Article/details/gcwsftayd.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.hesvh.cn/Article/details/gyhlodptp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.hesvh.cn/Article/details/gaxdvqboc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/gbzffxllc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/gwfhmlzai.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.zdbjq.cn/Article/details/gkagbmvrh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fehbvm.com/Article/details/gmtwzpzcg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.hesvh.cn/Article/details/gnkqujixr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.hesvh.cn/Article/details/gtbufepfb.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.hesvh.cn/Article/details/gikcyuipj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.hesvh.cn/Article/details/gzaithhws.sHtML


<!-- 参考信息 -->