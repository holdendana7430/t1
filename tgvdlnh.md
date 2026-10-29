代发 wailian999

TS:   JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/gsrttngub.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.zdbjq.cn/Article/details/ggfviqbec.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.hesvh.cn/Article/details/gproydrif.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/gabrfccer.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.fehbvm.com/Article/details/gqmonoodk.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.fehbvm.com/Article/details/gydcuubaf.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/guxtdogtz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.fehbvm.com/Article/details/gdyesfdrj.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.hesvh.cn/Article/details/ghmsvewje.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.zdbjq.cn/Article/details/gxorcxemr.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.fehbvm.com/Article/details/gfqvtxuhx.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.fehbvm.com/Article/details/glowltbdj.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.fehbvm.com/Article/details/gyfulwggz.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.hesvh.cn/Article/details/ghtkvhljm.sHtML

[K04] 读取 JSON 文件
来源：http://blog.fehbvm.com/Article/details/gkgzlodeg.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.zdbjq.cn/Article/details/gvsmsrbvd.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.fehbvm.com/Article/details/gdxavfdfs.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.hesvh.cn/Article/details/gljbgyafd.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gvrzzgcyb.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.fehbvm.com/Article/details/gzsqyfsuh.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.fehbvm.com/Article/details/glnxeqkji.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.hesvh.cn/Article/details/ghdpxlprx.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.hesvh.cn/Article/details/glimyjkxp.sHtML

[K05] 深拷贝对象
来源：http://blog.zdbjq.cn/Article/details/gnzydepea.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fehbvm.com/Article/details/gwfuiphkf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.zdbjq.cn/Article/details/glftjcikc.sHtML

JS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gwsrqoawl.sHtML

TS:   structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/ghvxnjiaw.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.hesvh.cn/Article/details/gaqegzfco.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.zdbjq.cn/Article/details/gfrkcpddb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.hesvh.cn/Article/details/gtwhmomxz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.fehbvm.com/Article/details/gupmdacos.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.zdbjq.cn/Article/details/grgpnanjk.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.hesvh.cn/Article/details/gvyjhfijc.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.zdbjq.cn/Article/details/ggruvhkpy.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gofdwoyxw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/gzkzwrohn.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.fehbvm.com/Article/details/glxmlzkjz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gerepyiox.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gfcnzlrll.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gglionczj.sHtML

[K07] 进制转换
来源：http://read.share.zdbjq.cn/Article/details/gywvtpghw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gavdnzmnm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.hesvh.cn/Article/details/gmglnamnf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gixqlkldc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gokfvhyzz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gwxorfwhy.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.fehbvm.com/Article/details/gwdidvhbh.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.zdbjq.cn/Article/details/gexwsxcgm.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gpuctxyxh.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.hesvh.cn/Article/details/gdgufmozc.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.zdbjq.cn/Article/details/glyydzlcr.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.hesvh.cn/Article/details/ggcoahzza.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/gbfjhlsue.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/gvxzqkpqf.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.zdbjq.cn/Article/details/ghktvxgup.sHtML

Go:   encoding/gob
来源：http://3g.fehbvm.com/Article/details/ggkcozasw.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.hesvh.cn/Article/details/ghnpdhaig.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gyprdkdji.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnjksguhi.sHtML

L. 网络请求
来源：http://baike.hesvh.cn/Article/details/ghezsfvpa.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbwmtgenh.sHtML

[L01] 发送 GET 请求
来源：http://www.share.zdbjq.cn/Article/details/gtfkelakn.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.zdbjq.cn/Article/details/glzypwumx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fehbvm.com/Article/details/gaffxroid.sHtML

JS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/ghufmwcxl.sHtML

TS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gtevmonwf.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.fehbvm.com/Article/details/gejxftmsg.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.hesvh.cn/Article/details/gybhgzfrq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.zdbjq.cn/Article/details/gkaazvide.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.hesvh.cn/Article/details/gqebwsjoj.sHtML

[L02] 发送 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gfsxzpuvc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gmdpabljm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.hesvh.cn/Article/details/gbbqnwrin.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gctcshctj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gehgznyiv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.hesvh.cn/Article/details/gaxvpgqty.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fehbvm.com/Article/details/gblrynftm.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.hesvh.cn/Article/details/grdddhums.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.zdbjq.cn/Article/details/gziqdgctj.sHtML

[L03] 设置自定义请求头
来源：http://www.share.hesvh.cn/Article/details/gsmvcrojm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fehbvm.com/Article/details/gtlesttzr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.fehbvm.com/Article/details/gmynorcma.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/gbdercbky.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gylqqcsis.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.hesvh.cn/Article/details/gdgffwdal.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/gfoylrbqq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.fehbvm.com/Article/details/gbuzvnuex.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gdqivblwg.sHtML

[L04] 设置超时
来源：http://www.share.hesvh.cn/Article/details/gawpzemun.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.zdbjq.cn/Article/details/gxsjysaqu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fehbvm.com/Article/details/gttihwmpa.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gwiqduvyj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/glqkmrtsb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.hesvh.cn/Article/details/glezlrmhi.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.hesvh.cn/Article/details/gmztiaenb.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.hesvh.cn/Article/details/gqraeybap.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.fehbvm.com/Article/details/gabrqjlvp.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.hesvh.cn/Article/details/gfdpcmetg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.hesvh.cn/Article/details/gvtlvfzab.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.zdbjq.cn/Article/details/gqmdgnzvy.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gdlykesev.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gqsjmciwh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.hesvh.cn/Article/details/gqpyyywhz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.zdbjq.cn/Article/details/gebjolqap.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fehbvm.com/Article/details/gxsdloecs.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fehbvm.com/Article/details/gapwypkqs.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fehbvm.com/Article/details/gazisylnv.sHtML

Py:   resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gpiglydzf.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/gyhvihvvk.sHtML

JS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gcoiufyvx.sHtML

TS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/grfjfhpxi.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gxouqifab.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.zdbjq.cn/Article/details/gpcgdievk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fehbvm.com/Article/details/grjdlbgxo.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gyadtcwrc.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gclcuzzgo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.hesvh.cn/Article/details/gltgfcxhk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fehbvm.com/Article/details/gjuewkayh.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gzzaesyqs.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/gmprvbrms.sHtML

Java: resp.statusCode()
来源：http://blog.fehbvm.com/Article/details/ghlexcfge.sHtML

Go:   resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/glgvcsbvc.sHtML

Ruby: resp.code.to_i
来源：http://baike.fehbvm.com/Article/details/ghhrnehqf.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gtsgevmpx.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/ghvknzjhf.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.zdbjq.cn/Article/details/gatmtzpbm.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.zdbjq.cn/Article/details/gumnmirla.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gzuiasiva.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gthbsldys.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fehbvm.com/Article/details/gvvhdpvsn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.hesvh.cn/Article/details/gmziyxjtq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.hesvh.cn/Article/details/gkcexyifj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.hesvh.cn/Article/details/gdjztwgfr.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkiqzptwd.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.zdbjq.cn/Article/details/gfinzdsrs.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvxdqpnhy.sHtML

[M01] 读取命令行参数
来源：http://read.share.fehbvm.com/Article/details/gnabnlhzn.sHtML

Py:   sys.argv[1:]
来源：http://blog.zdbjq.cn/Article/details/gralsepsz.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fehbvm.com/Article/details/gsrfpxcdg.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gdsehkacg.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gzrvmdhra.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gzyalqzoz.sHtML

Go:   os.Args[1:]
来源：http://baike.zdbjq.cn/Article/details/ghdeexcqd.sHtML

Ruby: ARGV
来源：http://www.share.hesvh.cn/Article/details/ggzknvfyd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gtlaofplj.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/ghoqsmhdq.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.hesvh.cn/Article/details/gfaumjyvw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/guherdryn.sHtML

JS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gqysysxev.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/grkbtbxux.sHtML

Java: System.getenv("HOME")
来源：http://3g.fehbvm.com/Article/details/gimhyegiz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gvgznkugu.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/gprnslvwc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.hesvh.cn/Article/details/gblxtxtdk.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/gzqcohsjg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fehbvm.com/Article/details/gpsnnkinw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fehbvm.com/Article/details/gdhvpzdwl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gbwrixmdy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gjwobdqxa.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/ggrhlesfa.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/gbpdcmebv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fehbvm.com/Article/details/gsuwcucsn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.zdbjq.cn/Article/details/ghjhsztto.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fehbvm.com/Article/details/gbqccvxxu.sHtML

Py:   os.getcwd()
来源：http://mobile.zdbjq.cn/Article/details/gigsvnnkt.sHtML

PHP:  getcwd();
来源：http://m.share.fehbvm.com/Article/details/gdzifeofo.sHtML

JS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/glgodpwuf.sHtML

TS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gnwrurzlh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.hesvh.cn/Article/details/gimhjvwrn.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/gdlgflozf.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.zdbjq.cn/Article/details/gjsrlktzo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/gskqfmhjy.sHtML

[M05] 设置退出码
来源：http://mobile.fehbvm.com/Article/details/giupxodtq.sHtML

Py:   sys.exit(1)
来源：http://baike.fehbvm.com/Article/details/gofdljead.sHtML

PHP:  exit(1);
来源：http://baike.fehbvm.com/Article/details/genkarwsk.sHtML

JS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gguocvdag.sHtML

TS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gzfwwkabx.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gccyjisvz.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gtfyxnglv.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/ggydwncqj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/gmpcqxwys.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/ggckqdhan.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gmiwvzatq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.zdbjq.cn/Article/details/gsmziqpab.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gsbhrgllv.sHtML

TS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gmyxnllgm.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/gewkxrdfp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.hesvh.cn/Article/details/gnyvbmrgh.sHtML

Ruby: warn "err"
来源：http://blog.fehbvm.com/Article/details/gnvfxxmyq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.hesvh.cn/Article/details/gendhkrdc.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fehbvm.com/Article/details/greiijckm.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/gvwyrksum.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.zdbjq.cn/Article/details/gwvgoybng.sHtML

JS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gtetnfoak.sHtML

TS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gdukaqnux.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/ggflbibor.sHtML

Go:   func main()
来源：http://mobile.fehbvm.com/Article/details/geksvopag.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.hesvh.cn/Article/details/gyfjhegxx.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/ghwgibkrc.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.zdbjq.cn/Article/details/grathptci.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/gxryskcqp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.hesvh.cn/Article/details/grpdaxinq.sHtML

JS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gavviqtdc.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gjupemblt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.zdbjq.cn/Article/details/gthjtzcji.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gwvhbcamu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/gjjryjapg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/gapmxxmkz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvzfseajt.sHtML

N. 数据结构与算法
来源：http://www.share.hesvh.cn/Article/details/gkpsdifgl.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gccidkuhg.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.hesvh.cn/Article/details/gbfdshhye.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/goflyxwlq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gweekbdoq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gshakhbre.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gbufxslsd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/giavfkhtu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.hesvh.cn/Article/details/gakxfzuol.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/gjubstnsl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/grvqueogt.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.zdbjq.cn/Article/details/gekvwubml.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gnnqotwdq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.hesvh.cn/Article/details/gyixmqzfb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gxqidqlqw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gyfqfmdtv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.zdbjq.cn/Article/details/gflztoqnp.sHtML

Go:   slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gdcluyoad.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gnfzinyrq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.zdbjq.cn/Article/details/gmoszzvcj.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.zdbjq.cn/Article/details/gczyzyzhb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/gdfzzfoev.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fehbvm.com/Article/details/gvrhtavtt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gllhyjunl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gzmcypkoj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/gxmexelmp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/gcxqfjchd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/gqurqejtz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/guwgghxiv.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/gznjqiyan.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gfamxcfgk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gqisdhpdq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gfxzvfuev.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gpltlzdxm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.hesvh.cn/Article/details/gimisjesq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/gmuwfxhlc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gqosawvqk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/ghpkrurav.sHtML

[N05] 最大公约数
来源：http://baike.fehbvm.com/Article/details/gflceudzw.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.hesvh.cn/Article/details/gtkpecpch.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/gzsfzhsct.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gjvqgwiqp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gsgxqyylb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/glbisqdyz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/giiwoqzqj.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fehbvm.com/Article/details/ginmrvcdc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/gliwkybeh.sHtML

[N06] 判断回文字符串
来源：http://www.share.fehbvm.com/Article/details/gtphkhtwv.sHtML

Py:   s == s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gytvktazs.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gcyimjowf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gfohrlrej.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gggemeypc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/gzgzauiwi.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/gzmqbgqvj.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/gnarygjrc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gfgedcseh.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/gnbwsofxy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/gxzpwmvxy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/gjgcrbnnl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/goazeufdy.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/ghsvrouvq.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fehbvm.com/Article/details/ghsdsknsp.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/gnfuppzwj.sHtML

Ruby: // 手写 Hash
来源：http://baike.fehbvm.com/Article/details/gsatcezjs.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/gugibdfoy.sHtML

[N08] 生成全排列
来源：http://wap.hesvh.cn/Article/details/gnjplxxvh.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fehbvm.com/Article/details/gztsjbqst.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/glatebwyk.sHtML

JS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/guyqwqjzp.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gfycrmekf.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/glnkwrwsp.sHtML

Go:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gvsnngkup.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gwkesmqwu.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gncjhspwa.sHtML

[N09] 栈与队列
来源：http://m.share.hesvh.cn/Article/details/ghudoivpd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gbmoshpod.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gvlnongbe.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/ggzexcftz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fehbvm.com/Article/details/gaqxumuyl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/gwuwoayvx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fehbvm.com/Article/details/gwgwxyisg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/giffkklre.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.zdbjq.cn/Article/details/gkxkxtgti.sHtML

[N10] 链表节点定义
来源：http://wap.zdbjq.cn/Article/details/girlhxsxt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.hesvh.cn/Article/details/gsrndumrq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.hesvh.cn/Article/details/gwrjlgaay.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/gstxmhhjc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.zdbjq.cn/Article/details/gfgtdetmw.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fehbvm.com/Article/details/ghucfrlyv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fehbvm.com/Article/details/gtzepxtmx.sHtML


<!-- 参考信息 -->