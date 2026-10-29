代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.hesvh.cn/Article/details/geqefeerv.sHtML

Go:   json.Marshal(obj)
来源：http://wap.zdbjq.cn/Article/details/ghamkqrzn.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.hesvh.cn/Article/details/ghjimsnnh.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.zdbjq.cn/Article/details/gteqktsqd.sHtML

[K02] JSON 字符串转对象
来源：http://3g.hesvh.cn/Article/details/gigqlazqq.sHtML

Py:   json.loads(s)
来源：http://blog.hesvh.cn/Article/details/gydhwfive.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.hesvh.cn/Article/details/gykbetwmt.sHtML

JS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gttwptmgn.sHtML

TS:   JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/gtiquyoex.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.fehbvm.com/Article/details/gkctnbavj.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.zdbjq.cn/Article/details/ggzvoqewn.sHtML

Ruby: JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/garwmzwrl.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.hesvh.cn/Article/details/gealqavpx.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.fehbvm.com/Article/details/gqouuzmtu.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gdxtezsdh.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.fehbvm.com/Article/details/gpoewggvi.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.zdbjq.cn/Article/details/gtcbauuxy.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fehbvm.com/Article/details/grywcqvjy.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.fehbvm.com/Article/details/ghyjarqmm.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.hesvh.cn/Article/details/ggqldhbis.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.zdbjq.cn/Article/details/gpagbdufi.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.fehbvm.com/Article/details/gudwcqenx.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.hesvh.cn/Article/details/gdyllbaxt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.hesvh.cn/Article/details/gsezrzgsr.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.zdbjq.cn/Article/details/gywmrahcc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/guirhspgg.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/gaclzfcmg.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gkmwcxtix.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/gantirfqg.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.fehbvm.com/Article/details/gihrbgroh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.hesvh.cn/Article/details/gzsjinqfo.sHtML

[K05] 深拷贝对象
来源：http://www.share.fehbvm.com/Article/details/gykuemwip.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.zdbjq.cn/Article/details/gkeqsxowu.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.hesvh.cn/Article/details/gehnmrymp.sHtML

JS:   structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gdulaypcj.sHtML

TS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gsqzamcgv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.fehbvm.com/Article/details/ghegvfbrr.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.fehbvm.com/Article/details/giniuatth.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.zdbjq.cn/Article/details/gfuiloypm.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.zdbjq.cn/Article/details/gogknulra.sHtML

[K06] 解析 URL 查询串
来源：http://baike.fehbvm.com/Article/details/gufwjfble.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.fehbvm.com/Article/details/gbkuxlsdp.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.fehbvm.com/Article/details/gulswzokt.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/gysfcytdo.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.hesvh.cn/Article/details/gwskypbox.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.hesvh.cn/Article/details/glgtusmrl.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gxpkqxlcd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gmobfjpaq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/gcutthqao.sHtML

[K07] 进制转换
来源：http://mobile.zdbjq.cn/Article/details/gadhkyssu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gzktwpqrg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fehbvm.com/Article/details/gdjowpkop.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gnueniiuq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gsyjgzkyk.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gvplfonlx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.fehbvm.com/Article/details/gpiinbrbe.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.fehbvm.com/Article/details/gotokpvot.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.hesvh.cn/Article/details/grgijeokj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.hesvh.cn/Article/details/gratbpyue.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gbxxdcjsy.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gkstlwjvz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/glfzumiqb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/gnpprxphu.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.zdbjq.cn/Article/details/gkdyaskhu.sHtML

Go:   encoding/gob
来源：http://wap.zdbjq.cn/Article/details/gebgcqsxc.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.fehbvm.com/Article/details/gaalrxint.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/gfjwyxxtn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gtifwooff.sHtML

L. 网络请求
来源：http://www.blog.fehbvm.com/Article/details/gdtivpykz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdbfzskkp.sHtML

[L01] 发送 GET 请求
来源：http://m.share.zdbjq.cn/Article/details/gqhvpxjwd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fehbvm.com/Article/details/gyplvvmil.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fehbvm.com/Article/details/gdbevcqbi.sHtML

JS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/ggtexlbca.sHtML

TS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gnojcprjg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fehbvm.com/Article/details/gqvgvmxlp.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.fehbvm.com/Article/details/gryjpbech.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.hesvh.cn/Article/details/gdghbtouv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fehbvm.com/Article/details/gzuavldev.sHtML

[L02] 发送 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gykhglfcw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.fehbvm.com/Article/details/gscahfcvg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.zdbjq.cn/Article/details/gowqneagx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gfhymdlhn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/gfztosomv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fehbvm.com/Article/details/ggbimmtiu.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.hesvh.cn/Article/details/gpspceriw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.hesvh.cn/Article/details/gumoevqun.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.zdbjq.cn/Article/details/getibcbhg.sHtML

[L03] 设置自定义请求头
来源：http://3g.zdbjq.cn/Article/details/gjvvyirzv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.hesvh.cn/Article/details/gymmikebb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.hesvh.cn/Article/details/gadsicxru.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gloplapta.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gjtriyqdr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.zdbjq.cn/Article/details/giwmbumua.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/gauccftnh.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.zdbjq.cn/Article/details/gszhieswn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gfqrpqrdu.sHtML

[L04] 设置超时
来源：http://wap.zdbjq.cn/Article/details/ggfbrtflt.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fehbvm.com/Article/details/gspevxgue.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.zdbjq.cn/Article/details/gwfmeuwpn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/gwrajjjxx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gmozuqygc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.hesvh.cn/Article/details/gwmbkvvue.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.zdbjq.cn/Article/details/geosxkclf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.hesvh.cn/Article/details/gvmkwmxur.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.hesvh.cn/Article/details/ghoxgbhgu.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.zdbjq.cn/Article/details/gmzydehcx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.zdbjq.cn/Article/details/gdvewxfjg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.hesvh.cn/Article/details/gurydklqu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gtvwvmwdb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gceulgecj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.zdbjq.cn/Article/details/gbbbxjuna.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fehbvm.com/Article/details/gbjiznbme.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.zdbjq.cn/Article/details/gwlpcnkoc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.hesvh.cn/Article/details/geanpuysr.sHtML

[L06] 解析响应为 JSON
来源：http://blog.zdbjq.cn/Article/details/gmzjbdfqn.sHtML

Py:   resp.json()
来源：http://read.share.hesvh.cn/Article/details/gdhccfawq.sHtML

PHP:  json_decode($body, true);
来源：http://blog.hesvh.cn/Article/details/gipnnzfue.sHtML

JS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gxjpbxznu.sHtML

TS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/gczifkrlg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/ggtqmhsjk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.zdbjq.cn/Article/details/gktujmjrb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fehbvm.com/Article/details/gcpkpyqxp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/gvummbbkr.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gngfogwze.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.zdbjq.cn/Article/details/gaulqnzmw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.zdbjq.cn/Article/details/gowbbpuxn.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gbaolzyjf.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gwccwfbzw.sHtML

Java: resp.statusCode()
来源：http://baike.fehbvm.com/Article/details/gknypzwlh.sHtML

Go:   resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/ggolmbidm.sHtML

Ruby: resp.code.to_i
来源：http://m.share.zdbjq.cn/Article/details/gzwqqeekk.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gzyvqdhqs.sHtML

[L08] 并发请求多个地址
来源：http://mobile.zdbjq.cn/Article/details/gqvavrmep.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.hesvh.cn/Article/details/gqaopxbqm.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.zdbjq.cn/Article/details/gvulurphd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gyzujvajg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gajgcatev.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/gnvcfrhth.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.hesvh.cn/Article/details/glxiyeded.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.hesvh.cn/Article/details/gyjoblghb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/gyphghgis.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grbqxklay.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.zdbjq.cn/Article/details/gqtdnlmaa.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpamhppfj.sHtML

[M01] 读取命令行参数
来源：http://www.share.hesvh.cn/Article/details/gvjuhlbij.sHtML

Py:   sys.argv[1:]
来源：http://3g.hesvh.cn/Article/details/gaeqhcjiu.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.hesvh.cn/Article/details/gmliqigxa.sHtML

JS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gfsvtllpk.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gliqvvozq.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gzcpftkjs.sHtML

Go:   os.Args[1:]
来源：http://m.share.zdbjq.cn/Article/details/gkcvhoxpc.sHtML

Ruby: ARGV
来源：http://read.share.zdbjq.cn/Article/details/gdxjarfvy.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gnyyagicf.sHtML

[M02] 读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gahjwohse.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fehbvm.com/Article/details/gzbepcpbq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gfkjmcmzx.sHtML

JS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gxmboyvbs.sHtML

TS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gidwjigfs.sHtML

Java: System.getenv("HOME")
来源：http://baike.fehbvm.com/Article/details/gdoxktufn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.hesvh.cn/Article/details/gekwabbrt.sHtML

Ruby: ENV["HOME"]
来源：http://wap.hesvh.cn/Article/details/gupguwbkk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/gzpuglowi.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gnsdhkssq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.hesvh.cn/Article/details/gjvvyxuts.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.hesvh.cn/Article/details/ggrgdxxmc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gpycrhkuj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/giynwdnlm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.zdbjq.cn/Article/details/gkuulxgng.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fehbvm.com/Article/details/gpdmnmehu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fehbvm.com/Article/details/guhslnamg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fehbvm.com/Article/details/gspxhwjul.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fehbvm.com/Article/details/geaggygim.sHtML

Py:   os.getcwd()
来源：http://wap.hesvh.cn/Article/details/gtouulxxh.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/gookvuerg.sHtML

JS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gjaeckclv.sHtML

TS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gdjcangpy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fehbvm.com/Article/details/ghgzarpqe.sHtML

Go:   os.Getwd()
来源：http://www.blog.hesvh.cn/Article/details/gatlktcig.sHtML

Ruby: Dir.pwd
来源：http://baike.fehbvm.com/Article/details/gqaejfjvh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.hesvh.cn/Article/details/gczdthvpx.sHtML

[M05] 设置退出码
来源：http://baike.fehbvm.com/Article/details/gtvobfxfx.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gpjpfewnx.sHtML

PHP:  exit(1);
来源：http://www.blog.hesvh.cn/Article/details/gpkfojfyv.sHtML

JS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gcrpsssnd.sHtML

TS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gpprffacs.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gatwywjhf.sHtML

Go:   os.Exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gmmkowfin.sHtML

Ruby: exit 1
来源：http://www.blog.fehbvm.com/Article/details/gwdumhbod.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.zdbjq.cn/Article/details/gqrekyvbh.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/gbbifzptc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gcttvehht.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fehbvm.com/Article/details/gvhrnqwew.sHtML

JS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gsdbbxsvl.sHtML

TS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gysvoiyvl.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/gzvgctclf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.hesvh.cn/Article/details/gwzfhohpy.sHtML

Ruby: warn "err"
来源：http://www.m.share.fehbvm.com/Article/details/gwiivbawu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/gwknjuhij.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.hesvh.cn/Article/details/gnrnukwsn.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.zdbjq.cn/Article/details/grwwvrfgz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/ghrycqust.sHtML

JS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gaidxfzyn.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/ghwtdccbv.sHtML

Java: public static void main(String[] args)
来源：http://read.share.hesvh.cn/Article/details/gaaldgucn.sHtML

Go:   func main()
来源：http://baike.zdbjq.cn/Article/details/gzxpdopqe.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/gjbusgkpk.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fehbvm.com/Article/details/gnpkuogjf.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/gwbbjzrjo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/goojholll.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/gwmcddroa.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gxxbvtbdf.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gqlpfxlki.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.hesvh.cn/Article/details/gmtdoajee.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fehbvm.com/Article/details/gsdoigcpm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.hesvh.cn/Article/details/gdggtzhlx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/gmugsbfmd.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxxsziozv.sHtML

N. 数据结构与算法
来源：http://m.share.fehbvm.com/Article/details/gkalouwxl.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grzzukcqt.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/gwupmajkr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gcqmjrhmd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gigvqbdnw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gfibzfdkr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gmzedustl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gvvupumnz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gdhmcenjt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.zdbjq.cn/Article/details/gdcqegnfq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gcwqdpvit.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.hesvh.cn/Article/details/gmcgijhia.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gvwszurhb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gtwvmeald.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gpjocqout.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gdmoasvcm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gcplnzyac.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/ghqdpddcl.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gthofpinc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/grgdqkmpx.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fehbvm.com/Article/details/gskoqgfqd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fehbvm.com/Article/details/geufpdizt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.hesvh.cn/Article/details/gevwqtcgx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gstygfiwi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gwnyyxyro.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fehbvm.com/Article/details/gzoqgubvn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.hesvh.cn/Article/details/gktpfoekf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/gnvebmtnn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.zdbjq.cn/Article/details/ggluntxrf.sHtML

[N04] 斐波那契数列
来源：http://www.blog.zdbjq.cn/Article/details/gpqehkzhe.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gyfpeqzta.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gxxfkhcfx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gzqqunyyk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gejzthncv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/glwbkqyxv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/gzohnhtvu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gybqsmupc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gmpbpsbwi.sHtML

[N05] 最大公约数
来源：http://blog.zdbjq.cn/Article/details/gpwynkbvu.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gaxsuxrxz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/gptgfmgku.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gpopddmrq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gqxknqjcl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.hesvh.cn/Article/details/guaxsetyr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/ggvpohomr.sHtML

Ruby: a.gcd(b)
来源：http://baike.fehbvm.com/Article/details/gpnzvutiz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.hesvh.cn/Article/details/gphqprucz.sHtML

[N06] 判断回文字符串
来源：http://mobile.zdbjq.cn/Article/details/gaiwkmhhw.sHtML

Py:   s == s[::-1]
来源：http://mobile.hesvh.cn/Article/details/girctsibz.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gtullimzw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gpxdzrfcv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gkuimeqnm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.zdbjq.cn/Article/details/ggoafsbrf.sHtML

Go:   // 双指针从两端比较
来源：http://baike.hesvh.cn/Article/details/gvvwbkypp.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/gfkyclrbv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gcbggswsj.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/gthgbyidi.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/gajrtlntw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.zdbjq.cn/Article/details/gqtxisvvf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/gvtxyqyfz.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.hesvh.cn/Article/details/grqrtyvfc.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.zdbjq.cn/Article/details/gruuvjmwl.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.hesvh.cn/Article/details/gkpsaidhc.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/guviborjq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.hesvh.cn/Article/details/gmjgwkbbs.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/gnaadkwvg.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gmvskzjmj.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fehbvm.com/Article/details/grqbcodyb.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gmprgugmq.sHtML

TS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gtqtqtczy.sHtML

Java: // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gjrdgawxi.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gcovukazu.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/ghthnenld.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gadyqxzsg.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/gnckcgvap.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/guisrnmul.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fehbvm.com/Article/details/gframbxwy.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gnpoecprf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/geegxmldp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gmhkjbwop.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.zdbjq.cn/Article/details/govwrbfvi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/ghhgxhnkn.sHtML


<!-- 参考信息 -->