代发 wailian999

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gckyfeqrq.sHtML

K. JSON 与序列化
来源：http://m.share.fehbvm.com/Article/details/gvmnwdsdv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwrhattwd.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.hesvh.cn/Article/details/gxeomiorr.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.hesvh.cn/Article/details/ghrydiupu.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/gkljmzlzy.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.fehbvm.com/Article/details/gjicjrjwe.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.zdbjq.cn/Article/details/gqrywwsiy.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.zdbjq.cn/Article/details/glrtcuefg.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.fehbvm.com/Article/details/gwyjvemkc.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.hesvh.cn/Article/details/gioycesvv.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.zdbjq.cn/Article/details/gpxrxiebu.sHtML

[K02] JSON 字符串转对象
来源：http://blog.hesvh.cn/Article/details/gqefjeipt.sHtML

Py:   json.loads(s)
来源：http://wap.hesvh.cn/Article/details/gchgywcji.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.zdbjq.cn/Article/details/gmtnentbk.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/guyijivin.sHtML

TS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gdjooaehj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gylhufpnq.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.hesvh.cn/Article/details/gvtxpqahr.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/gpdhblrfj.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.fehbvm.com/Article/details/gccykonye.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.hesvh.cn/Article/details/gzdousrfc.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.zdbjq.cn/Article/details/gjrorucqa.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gjrydqemw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.hesvh.cn/Article/details/guyxaznka.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.hesvh.cn/Article/details/gtgiwcdew.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.hesvh.cn/Article/details/gdikmqkfg.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.hesvh.cn/Article/details/gbfpfaqor.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.hesvh.cn/Article/details/ghloicnqa.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.zdbjq.cn/Article/details/gkmjegbai.sHtML

[K04] 读取 JSON 文件
来源：http://wap.hesvh.cn/Article/details/gqrvwnfda.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.hesvh.cn/Article/details/guuqvtbro.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.zdbjq.cn/Article/details/gtnjrjyag.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.zdbjq.cn/Article/details/gpzbbnmyk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/gumusazop.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.fehbvm.com/Article/details/gvsogusab.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.fehbvm.com/Article/details/gqunngtlh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.hesvh.cn/Article/details/gbcidmrbs.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.fehbvm.com/Article/details/gwzicgtem.sHtML

[K05] 深拷贝对象
来源：http://www.blog.fehbvm.com/Article/details/grjbpjvgk.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gkdhxvake.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.hesvh.cn/Article/details/gejkwxcoz.sHtML

JS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/glswjrhzw.sHtML

TS:   structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gqsbttnsf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.zdbjq.cn/Article/details/gghgpegdc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.fehbvm.com/Article/details/gubrsenor.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.zdbjq.cn/Article/details/gefayzktd.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.zdbjq.cn/Article/details/gjnoayzaf.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.fehbvm.com/Article/details/ghnznwfxz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.fehbvm.com/Article/details/giwpcdovw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.hesvh.cn/Article/details/gayawrlew.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/gydojazih.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gbydmwytb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.hesvh.cn/Article/details/gfdmcfxke.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gkohmclik.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gxbciyxxs.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gsyegyebn.sHtML

[K07] 进制转换
来源：http://blog.fehbvm.com/Article/details/gbhlwzajk.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gmonsltwo.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.fehbvm.com/Article/details/gxsayptbf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gnfurhkew.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/glsxjzsyp.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gdndpkpac.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.hesvh.cn/Article/details/gixlyiirn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.hesvh.cn/Article/details/gcltwpcuc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gnqcmlnhr.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.zdbjq.cn/Article/details/gqgktctxb.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.zdbjq.cn/Article/details/ghzbbeawk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.zdbjq.cn/Article/details/gbxmjlryy.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/gzuuereps.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/ghzbchqtb.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fehbvm.com/Article/details/gnfzmqjpb.sHtML

Go:   encoding/gob
来源：http://wap.hesvh.cn/Article/details/gspockzan.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.hesvh.cn/Article/details/gwdxkjcsv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/glhaqguzu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gyuooyozl.sHtML

L. 网络请求
来源：http://baike.fehbvm.com/Article/details/gxckohace.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gpuirullk.sHtML

[L01] 发送 GET 请求
来源：http://blog.fehbvm.com/Article/details/gsvaszfkr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.hesvh.cn/Article/details/gpfujveet.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.fehbvm.com/Article/details/gkxzpsgjz.sHtML

JS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/grzpoocjy.sHtML

TS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gzbtcslyk.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.zdbjq.cn/Article/details/giicuumnj.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fehbvm.com/Article/details/gsmgmlcoq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.zdbjq.cn/Article/details/gfbnpyeko.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.fehbvm.com/Article/details/glzuwtigk.sHtML

[L02] 发送 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gbexrkkcs.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/gfhccaeum.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.fehbvm.com/Article/details/gpgyhfjxi.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/genrqkjsd.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/gfruhtlhr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.zdbjq.cn/Article/details/gmezollxl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.hesvh.cn/Article/details/gbocxjwxq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.zdbjq.cn/Article/details/guobvzzoi.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.hesvh.cn/Article/details/ghtodbcsd.sHtML

[L03] 设置自定义请求头
来源：http://m.share.fehbvm.com/Article/details/gyiwydmrb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fehbvm.com/Article/details/gpxqafgxl.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.fehbvm.com/Article/details/gkqhxyalu.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/gogtsxmwl.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gfctlgzif.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.hesvh.cn/Article/details/gpacgyicy.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/gjieoggjt.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.fehbvm.com/Article/details/grtekctrz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gfudfhjum.sHtML

[L04] 设置超时
来源：http://wap.hesvh.cn/Article/details/gedgumesb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fehbvm.com/Article/details/gkrvqnhen.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.hesvh.cn/Article/details/gxhtophep.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gokbxchfw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/grvnwujzz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.zdbjq.cn/Article/details/geudtwriy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.hesvh.cn/Article/details/golmodjqp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.hesvh.cn/Article/details/gohqkmggo.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fehbvm.com/Article/details/ggnucadne.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.fehbvm.com/Article/details/gkzputthh.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.zdbjq.cn/Article/details/gbnbujfmz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fehbvm.com/Article/details/gwgfswxcl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/gyvbqbbyp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gvfdnumme.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fehbvm.com/Article/details/gnwaheale.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.hesvh.cn/Article/details/gzriwobyd.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.hesvh.cn/Article/details/giejcrzxp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.hesvh.cn/Article/details/gzjvckyed.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.hesvh.cn/Article/details/gwyctcluv.sHtML

Py:   resp.json()
来源：http://wap.zdbjq.cn/Article/details/gfbmmsemc.sHtML

PHP:  json_decode($body, true);
来源：http://wap.zdbjq.cn/Article/details/gllkzwjlz.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gunvfvrqj.sHtML

TS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gvugwphri.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gydxuansm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.zdbjq.cn/Article/details/gbvxfnfwv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.zdbjq.cn/Article/details/gfaymlqht.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gelqcsppz.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gjyhcjvxx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.hesvh.cn/Article/details/gxkgsgcvj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.zdbjq.cn/Article/details/gxejmniva.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gnmltzbgx.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gvshbcmkr.sHtML

Java: resp.statusCode()
来源：http://www.blog.fehbvm.com/Article/details/gacqcdcjv.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gzifzpurj.sHtML

Ruby: resp.code.to_i
来源：http://3g.zdbjq.cn/Article/details/gxmomyrga.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gfxslllpc.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.hesvh.cn/Article/details/guytyskpt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fehbvm.com/Article/details/gxglgouie.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.zdbjq.cn/Article/details/gjbquwloc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/grzsmkfuv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gptzclaut.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.hesvh.cn/Article/details/gffozlddd.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fehbvm.com/Article/details/gcxkagdun.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fehbvm.com/Article/details/ghxestbrq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.zdbjq.cn/Article/details/gkzxbiimt.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvgvfwfdg.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.hesvh.cn/Article/details/gonowjvfz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glvsnyqfs.sHtML

[M01] 读取命令行参数
来源：http://www.share.fehbvm.com/Article/details/gylitnyng.sHtML

Py:   sys.argv[1:]
来源：http://3g.hesvh.cn/Article/details/gzgdygvrk.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.zdbjq.cn/Article/details/goyzzrdsb.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gbmxpyeyx.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gjhlvjgyo.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gliimnraf.sHtML

Go:   os.Args[1:]
来源：http://blog.zdbjq.cn/Article/details/gsgtsdqgq.sHtML

Ruby: ARGV
来源：http://wap.zdbjq.cn/Article/details/gefjfeurf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/grbdgkzvo.sHtML

[M02] 读取环境变量
来源：http://baike.fehbvm.com/Article/details/gzoxkccut.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gcmxusfkj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gbntzdugp.sHtML

JS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/ghlqvkilm.sHtML

TS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/glbjihyam.sHtML

Java: System.getenv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gwcwmajxm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fehbvm.com/Article/details/ggyyvfebk.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/gudjccfgq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/gkcgghygg.sHtML

[M03] 执行外部命令
来源：http://m.share.zdbjq.cn/Article/details/gmevmpyon.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fehbvm.com/Article/details/guthqhejn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.hesvh.cn/Article/details/gtdiopkjy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gwutnzrcn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gswargcof.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/gjpclinqx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/gijfzjpsm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.zdbjq.cn/Article/details/gbdppekmk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fehbvm.com/Article/details/guamfqctq.sHtML

[M04] 获取当前工作目录
来源：http://mobile.hesvh.cn/Article/details/gllzxwzix.sHtML

Py:   os.getcwd()
来源：http://3g.zdbjq.cn/Article/details/gwknlarpv.sHtML

PHP:  getcwd();
来源：http://www.blog.zdbjq.cn/Article/details/gjmgspkpt.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gskntennh.sHtML

TS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gtvqsgzcf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/gtbtyyejr.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/gpiuwhheq.sHtML

Ruby: Dir.pwd
来源：http://www.blog.zdbjq.cn/Article/details/gxfxsmznk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fehbvm.com/Article/details/gerxkxvsk.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/gpukucxwv.sHtML

Py:   sys.exit(1)
来源：http://baike.hesvh.cn/Article/details/gxivcwwqk.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/ghyixynnr.sHtML

JS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gfxikrbyv.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gbufrrgaq.sHtML

Java: System.exit(1)
来源：http://blog.fehbvm.com/Article/details/gwmbslhqr.sHtML

Go:   os.Exit(1)
来源：http://m.share.hesvh.cn/Article/details/gpvzhhrjq.sHtML

Ruby: exit 1
来源：http://wap.zdbjq.cn/Article/details/ggqxbreqr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/gqenmpcjf.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/gyjleqpec.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gpaqobutd.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.hesvh.cn/Article/details/gwgsljjak.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gpxwcbelu.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/govvhbfky.sHtML

Java: System.err.println("err")
来源：http://wap.hesvh.cn/Article/details/gbbmicuyk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.zdbjq.cn/Article/details/grcijwkxr.sHtML

Ruby: warn "err"
来源：http://www.share.hesvh.cn/Article/details/gpihwalyk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/guqikhoot.sHtML

[M07] 判断是否为主入口
来源：http://baike.zdbjq.cn/Article/details/gbccsqury.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.hesvh.cn/Article/details/golzyujld.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/gckgdhdru.sHtML

JS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gxzhnvung.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gwaaucmqz.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gkznryehp.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/gpibuirok.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fehbvm.com/Article/details/gbhgqalwg.sHtML

C#:   static void Main(string[] args)
来源：http://wap.hesvh.cn/Article/details/gikgomljv.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/gbubiarek.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.hesvh.cn/Article/details/gzynsxgga.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.zdbjq.cn/Article/details/guqncfjkf.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gsrkyzxwu.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gqfvbtdcb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.hesvh.cn/Article/details/grzajcoqy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.fehbvm.com/Article/details/gmvpupoqq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/gqjwweela.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.hesvh.cn/Article/details/ghqfevahh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwbwwgkcz.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/gfhbblgef.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/givintsax.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.hesvh.cn/Article/details/gtsimuelo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gjynhddnm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fehbvm.com/Article/details/gcqhdyaqa.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gybxvicew.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gzjdvtlzn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gyodhdihe.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gzdvzjnfg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/gbrmxtpeq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gqmghyigh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/ggvfxnqdl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gkdxmsapq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fehbvm.com/Article/details/gktkagrqh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/geqbievut.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gimrkrhnr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.zdbjq.cn/Article/details/glabcxqua.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/giwamwdzw.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gwucfuyon.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/gskiwdxfw.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.hesvh.cn/Article/details/gtgbfkaql.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fehbvm.com/Article/details/gazqsulxc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.hesvh.cn/Article/details/gaovwggbs.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gsguexgne.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gqihubngj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.zdbjq.cn/Article/details/gpezjxkpx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gquotfsde.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/gjbnuynxa.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.zdbjq.cn/Article/details/gmcwdxtmp.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/gvtdhpjka.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gbuoubqxi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gaxitehbe.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/geievmnkg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gjhmksvwe.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/ghnkrcsdm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fehbvm.com/Article/details/gpmkotknd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gegrujuhv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gyjarosxc.sHtML

[N05] 最大公约数
来源：http://read.share.hesvh.cn/Article/details/gyknemwit.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/gytptsddk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.zdbjq.cn/Article/details/gdugbxvtu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gbnxeiywa.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gqbanenxo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.hesvh.cn/Article/details/gtyibwrlg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gamdtrwrh.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/gvqvdlhyk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.hesvh.cn/Article/details/gierzmdfo.sHtML

[N06] 判断回文字符串
来源：http://m.share.fehbvm.com/Article/details/gctzlncgw.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gsqoxdcfb.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gjdnmxdhq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gpmavdubs.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gdmbhwykz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/ghuvqrzdq.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/gvllqlgvy.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/grlpatxlw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gxytgbgjn.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/geaznbdlb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.zdbjq.cn/Article/details/gsfjgfwwb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fehbvm.com/Article/details/gxrymfxsg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/gzztlifmd.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fehbvm.com/Article/details/gkgiprlcr.sHtML

Java: // 手写 HashMap
来源：http://3g.hesvh.cn/Article/details/gdlbabebo.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.zdbjq.cn/Article/details/gwtrzkjhc.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/ggnnanooy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/gqzminhem.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/gfmmkeyvp.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fehbvm.com/Article/details/gtqsrzior.sHtML

PHP:  // 手写递归交换
来源：http://m.share.hesvh.cn/Article/details/gglpnmzov.sHtML

JS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gkzbmesnj.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gtfjcyeyk.sHtML

Java: // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gfadaeytw.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gbqyrfdxq.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/ghafkqkay.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gsbdszsnq.sHtML


<!-- 参考信息 -->