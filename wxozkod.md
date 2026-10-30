代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.zdbjq.cn/Article/details/gahtmpswe.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.zdbjq.cn/Article/details/gtttmonaj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.hesvh.cn/Article/details/gzlrrmstj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gchcyagbh.sHtML

[K02] JSON 字符串转对象
来源：http://blog.zdbjq.cn/Article/details/gxkgomfpm.sHtML

Py:   json.loads(s)
来源：http://blog.zdbjq.cn/Article/details/gmzdaybbj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.zdbjq.cn/Article/details/goybhjrop.sHtML

JS:   JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gpbunvlpe.sHtML

TS:   JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/ganyvzpvu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.fehbvm.com/Article/details/gcpmvrkwd.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.zdbjq.cn/Article/details/ggpakykuw.sHtML

Ruby: JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gcuitkdgo.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.fehbvm.com/Article/details/gdcdzswzn.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.zdbjq.cn/Article/details/gmnhijexa.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.zdbjq.cn/Article/details/gazdzlghx.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.fehbvm.com/Article/details/gkglsnrha.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.hesvh.cn/Article/details/gentwfuxy.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.zdbjq.cn/Article/details/grivxcmql.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.fehbvm.com/Article/details/gszofwgqb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.hesvh.cn/Article/details/gnjqxwzxs.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gcvdarywb.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.fehbvm.com/Article/details/gpngvmmnc.sHtML

[K04] 读取 JSON 文件
来源：http://baike.zdbjq.cn/Article/details/gbvkpxoru.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.hesvh.cn/Article/details/ghcgchign.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.fehbvm.com/Article/details/gcxchbnsb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fehbvm.com/Article/details/gxmfvwctf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fehbvm.com/Article/details/guizlvbuf.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gsjuolmfl.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/ggtdgpxvo.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.fehbvm.com/Article/details/gfkuzflue.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.fehbvm.com/Article/details/gaiaxnxcj.sHtML

[K05] 深拷贝对象
来源：http://blog.hesvh.cn/Article/details/ggmkvhhse.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.zdbjq.cn/Article/details/ghifjxsfi.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.hesvh.cn/Article/details/ggkfxtmbk.sHtML

JS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gouuuclib.sHtML

TS:   structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gchvdljfe.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fehbvm.com/Article/details/gulnxdroy.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.hesvh.cn/Article/details/giahldopq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.fehbvm.com/Article/details/gpbfihcsy.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.zdbjq.cn/Article/details/gvzrwoidq.sHtML

[K06] 解析 URL 查询串
来源：http://baike.fehbvm.com/Article/details/gjfdlsllk.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/gluumtoev.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.hesvh.cn/Article/details/gbcdgvqzr.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/gfkutwdfu.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gryywvagf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.hesvh.cn/Article/details/gzzyatnsk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gryoudkxb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gojllfcqm.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gtimdmcyy.sHtML

[K07] 进制转换
来源：http://wap.hesvh.cn/Article/details/gzbrrsobl.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.hesvh.cn/Article/details/grmlrjabh.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.fehbvm.com/Article/details/gpcuduosf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gcybbmdhk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/grosibblo.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/goboficph.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.zdbjq.cn/Article/details/ggisxapbz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.hesvh.cn/Article/details/gosvxaosp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gpfoxakrz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.hesvh.cn/Article/details/gugdbszjs.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.hesvh.cn/Article/details/gpsuxbyql.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.zdbjq.cn/Article/details/gnnpceobs.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gmmkxvkqq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.zdbjq.cn/Article/details/gvcfrjjmc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.hesvh.cn/Article/details/gimaewany.sHtML

Go:   encoding/gob
来源：http://mobile.fehbvm.com/Article/details/gbichniyx.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gnqqtujyw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/ghqsyeakb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gyeutpbrx.sHtML

L. 网络请求
来源：http://www.blog.zdbjq.cn/Article/details/gbqymeyxc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gyvwqlnzw.sHtML

[L01] 发送 GET 请求
来源：http://blog.hesvh.cn/Article/details/gpgnvtagg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.zdbjq.cn/Article/details/gpsdmlbyo.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.hesvh.cn/Article/details/gkdmkeday.sHtML

JS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/giucchubk.sHtML

TS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/gpdmzvkso.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.hesvh.cn/Article/details/gpsbgchbl.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.hesvh.cn/Article/details/ghosgdccf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.hesvh.cn/Article/details/gdsvhgxqa.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fehbvm.com/Article/details/gtfkeheny.sHtML

[L02] 发送 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gkkmafasg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gknkmlgyj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.zdbjq.cn/Article/details/gnumpqjce.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/gixvspbag.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gcipgqyvz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.zdbjq.cn/Article/details/gsexhkqks.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.hesvh.cn/Article/details/gesyfiawa.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fehbvm.com/Article/details/gpxxutdhg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.fehbvm.com/Article/details/gkkjefsbd.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.hesvh.cn/Article/details/gxhvyglup.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.zdbjq.cn/Article/details/gbbwqronw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.zdbjq.cn/Article/details/geczehtgg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gcvgthsoa.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gzrtxmatg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.hesvh.cn/Article/details/gmgdofxqz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/ghihnqfui.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.hesvh.cn/Article/details/gsonbtvcd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/guypnjrba.sHtML

[L04] 设置超时
来源：http://read.share.zdbjq.cn/Article/details/grxgasrdf.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.hesvh.cn/Article/details/glviyhfcs.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.fehbvm.com/Article/details/grsgrsfit.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gggmjfvdk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gpfyjufqe.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.zdbjq.cn/Article/details/gezsksgka.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.fehbvm.com/Article/details/gcqeuxafk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.zdbjq.cn/Article/details/gsvifdlkf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.hesvh.cn/Article/details/ggrxkagzc.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fehbvm.com/Article/details/gceelhnoz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/guswajgfy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.hesvh.cn/Article/details/gnulunxxl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/glrlhwucc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/girlgoset.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.hesvh.cn/Article/details/gyxjnksct.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.hesvh.cn/Article/details/gugljkuur.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.hesvh.cn/Article/details/gtspxyfve.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.hesvh.cn/Article/details/gmcnjlgql.sHtML

[L06] 解析响应为 JSON
来源：http://3g.hesvh.cn/Article/details/gtxltldwr.sHtML

Py:   resp.json()
来源：http://baike.fehbvm.com/Article/details/giqsvbnre.sHtML

PHP:  json_decode($body, true);
来源：http://wap.zdbjq.cn/Article/details/gxkpunelz.sHtML

JS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/ggmajzydv.sHtML

TS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gsecfuqcw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gjjkwmlvi.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.zdbjq.cn/Article/details/gqbpjteuu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/gohpiccid.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fehbvm.com/Article/details/gjpoejzfo.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/grpnexfvy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.zdbjq.cn/Article/details/gzzibuqmu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fehbvm.com/Article/details/gjmfatrlr.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gcxrqpmyb.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gwrcxbwrd.sHtML

Java: resp.statusCode()
来源：http://www.share.fehbvm.com/Article/details/gjqldldak.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gvkdkzpkd.sHtML

Ruby: resp.code.to_i
来源：http://blog.zdbjq.cn/Article/details/gqgaiyrwz.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gzzkmjlxb.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/gndnckcml.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.hesvh.cn/Article/details/gjrkamttc.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fehbvm.com/Article/details/gfqtvwpmw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gedqwkmxd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gezuptmcu.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.zdbjq.cn/Article/details/grzttqqyd.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.hesvh.cn/Article/details/gyextmiip.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fehbvm.com/Article/details/gcwsogwvz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.zdbjq.cn/Article/details/gmnzyobvf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcvqhchix.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.zdbjq.cn/Article/details/gxofoirhc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpnjtujbh.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/gknhxcywx.sHtML

Py:   sys.argv[1:]
来源：http://wap.fehbvm.com/Article/details/gsjskbzuj.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.zdbjq.cn/Article/details/gdqtxoied.sHtML

JS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gswubureo.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gcmeeosnw.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gwxibzalc.sHtML

Go:   os.Args[1:]
来源：http://wap.fehbvm.com/Article/details/gvsmyekpz.sHtML

Ruby: ARGV
来源：http://3g.zdbjq.cn/Article/details/gtfqobpji.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gxxojauwa.sHtML

[M02] 读取环境变量
来源：http://3g.hesvh.cn/Article/details/gxocqoygl.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.hesvh.cn/Article/details/goekgsnmj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/getsyvrep.sHtML

JS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gdswbmvsa.sHtML

TS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/glyqszupo.sHtML

Java: System.getenv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/ghyswikiw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.hesvh.cn/Article/details/giquwumcy.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/gzmxptshi.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/gydiefaxe.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/gkwtpdwro.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fehbvm.com/Article/details/gcqumbrnh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.zdbjq.cn/Article/details/gnpqkqnuj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/ghperubid.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gpllosycn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.zdbjq.cn/Article/details/gleizecvq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.hesvh.cn/Article/details/gydopzeof.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/gtbvrcnpz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/gldpoavke.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.hesvh.cn/Article/details/gplwuiycr.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/gifidpfus.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/gksalepnf.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gqblsdqau.sHtML

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gxzsxzsvk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.zdbjq.cn/Article/details/gbsdaoddb.sHtML

Go:   os.Getwd()
来源：http://mobile.fehbvm.com/Article/details/gklvtagye.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/gjikpcblm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.hesvh.cn/Article/details/gbstzwfho.sHtML

[M05] 设置退出码
来源：http://mobile.zdbjq.cn/Article/details/gahctasfx.sHtML

Py:   sys.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gfbtcndoh.sHtML

PHP:  exit(1);
来源：http://blog.hesvh.cn/Article/details/gtdpdkqxe.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gacwhuuqz.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gkpqztahf.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gacjxlmvx.sHtML

Go:   os.Exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gyslipypm.sHtML

Ruby: exit 1
来源：http://www.share.fehbvm.com/Article/details/grrfefxwv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/gmwplphnh.sHtML

[M06] 向标准错误输出
来源：http://3g.zdbjq.cn/Article/details/gyyvaawfb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/ggdgeevby.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.hesvh.cn/Article/details/gyoxnakoc.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gituchmuj.sHtML

TS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gvpzsmuko.sHtML

Java: System.err.println("err")
来源：http://blog.zdbjq.cn/Article/details/gllnvivds.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/grsaqsozy.sHtML

Ruby: warn "err"
来源：http://blog.fehbvm.com/Article/details/gpbmghofm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.hesvh.cn/Article/details/gltarauos.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.hesvh.cn/Article/details/ggysvtqmw.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/guucjsmkl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/gumelaloo.sHtML

JS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gnoogayvx.sHtML

TS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gbhywipbt.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/gnsnxyjxa.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/gbwkxlnkc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/glouvadxw.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/gvxmxsebl.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/gxdibbcty.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/gynghjyny.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fehbvm.com/Article/details/glngfxsdi.sHtML

JS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gqwthjtcx.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/goslgzwhk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.hesvh.cn/Article/details/gaipglcpp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.zdbjq.cn/Article/details/gvsexytim.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fehbvm.com/Article/details/grtlxntld.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/glhkdcner.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gedwqbqpi.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/gmbrighth.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gumkpfzlk.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.zdbjq.cn/Article/details/grbjbqkam.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fehbvm.com/Article/details/gcrfyhrjj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/gsbnczxlk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gxogculit.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gogdwvzte.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gijgivhib.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gxfvehcgs.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/guaxauyau.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gbhtlqzkm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.hesvh.cn/Article/details/gxlcyupog.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/giwrzcptz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/ggqsjjiyr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gxaijwmsc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gweuppbcy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/gfybckyzz.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gpicifimb.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gbyxopidm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.hesvh.cn/Article/details/gnxwzubkn.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.hesvh.cn/Article/details/gbktofnyz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fehbvm.com/Article/details/gsfqwwbkl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fehbvm.com/Article/details/gteitefwp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gduaezrjm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/govzdqikd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/gilnaozhg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.zdbjq.cn/Article/details/gabmaxujq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/gyyixuhsl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fehbvm.com/Article/details/gwxibolpn.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.zdbjq.cn/Article/details/gqothuxkp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gercueahm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gqcpyvwok.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gkvsejhrj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gwtqzvnlq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/ggwicbkee.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/gpzcquszs.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/ghyoeohdh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gwqvvphkk.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/grmipzrkz.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gyitaqdpl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.zdbjq.cn/Article/details/glntkwfbd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gqxbjjjrr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/grkjcoyfb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fehbvm.com/Article/details/gkbqyjmlg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gxpoidhwh.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/gyfrwyntb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqxuvvwen.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gxfjglzpk.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/guoyepllw.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fehbvm.com/Article/details/gcylkghgr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gdqrtuvjk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gknyuqvke.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/gjqgvauji.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/gsjjznzww.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/gljefshry.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gitqrulmt.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.zdbjq.cn/Article/details/gswxpopkh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/gpxfjufdc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/gqayjbysu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/gxvjuhpqg.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.hesvh.cn/Article/details/gmjytxcsl.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/goofyuwvw.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/gzkclnhrh.sHtML

Ruby: // 手写 Hash
来源：http://baike.fehbvm.com/Article/details/giwbdnamg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/gapyfnetq.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/gcfsmigdb.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/guimfnxjc.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.hesvh.cn/Article/details/ghexoyywb.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gitaqmkcy.sHtML

TS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gcayfdmrt.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gdfwodeza.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gtugswnoy.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.hesvh.cn/Article/details/gdnimibnj.sHtML

C#:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/glqymdela.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/gtipfoosv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.zdbjq.cn/Article/details/gpmyqqawu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fehbvm.com/Article/details/gsykulrkx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gmixraedi.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.hesvh.cn/Article/details/gwdibvrzd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gpnjipzmf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.zdbjq.cn/Article/details/ghtpbipui.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gtygnjsov.sHtML


<!-- 参考信息 -->