代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.hesvh.cn/Article/details/guzjwbtnf.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/gtobnocon.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.fehbvm.com/Article/details/gmyekqbhh.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.hesvh.cn/Article/details/gcwwtwvaw.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.zdbjq.cn/Article/details/gyunfyljd.sHtML

Go:   json.Marshal(obj)
来源：http://3g.zdbjq.cn/Article/details/geoxmfgav.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.fehbvm.com/Article/details/gdhywwimq.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.fehbvm.com/Article/details/gbcamirlt.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.fehbvm.com/Article/details/gegfwlnaz.sHtML

Py:   json.loads(s)
来源：http://blog.hesvh.cn/Article/details/gpetymgqo.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.hesvh.cn/Article/details/gqstcrgwn.sHtML

JS:   JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gjrtrqskv.sHtML

TS:   JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/givrlwhry.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.zdbjq.cn/Article/details/gmttiderl.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/gvfqbcnwd.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gcgfpnbla.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.zdbjq.cn/Article/details/gmthzndvz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.fehbvm.com/Article/details/gfrvlvxjx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.fehbvm.com/Article/details/gwqekhrjp.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fehbvm.com/Article/details/gkwxwoxwr.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/gthmllmti.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fehbvm.com/Article/details/ghvwupwuh.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.hesvh.cn/Article/details/ggnaekfec.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.hesvh.cn/Article/details/gdeguukro.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.fehbvm.com/Article/details/grlidhojq.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.hesvh.cn/Article/details/gjpeexpag.sHtML

[K04] 读取 JSON 文件
来源：http://blog.fehbvm.com/Article/details/gjinlddgd.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.hesvh.cn/Article/details/gpdhxmeot.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.zdbjq.cn/Article/details/gzpvhqmux.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.hesvh.cn/Article/details/gogmfawus.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fehbvm.com/Article/details/gaaayibxy.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gqqybskge.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/grrfcbovd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gzbrvkmov.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gevrypemx.sHtML

[K05] 深拷贝对象
来源：http://www.share.zdbjq.cn/Article/details/gegnfxglk.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.fehbvm.com/Article/details/gxolwjltv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.fehbvm.com/Article/details/gggloorfr.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/geshckmfc.sHtML

TS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gthgsxdul.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.hesvh.cn/Article/details/gzgydkgrz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.zdbjq.cn/Article/details/ggoqkircb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.hesvh.cn/Article/details/gltybiukd.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.zdbjq.cn/Article/details/gpyydtvic.sHtML

[K06] 解析 URL 查询串
来源：http://wap.hesvh.cn/Article/details/guqzggnyn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.fehbvm.com/Article/details/gffgxidug.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.zdbjq.cn/Article/details/gmosrpenw.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.hesvh.cn/Article/details/ghnhsjezz.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/gumcrwfbf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.zdbjq.cn/Article/details/gqzesbexh.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gisqumvmt.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gjyoxvuet.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gkvyafuwj.sHtML

[K07] 进制转换
来源：http://mobile.fehbvm.com/Article/details/gaedcjqjb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/ggfzakvzh.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.fehbvm.com/Article/details/gnxmwrafu.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gkcpudvuq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/guuwymvdb.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gfqdyogpo.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.hesvh.cn/Article/details/glgzrjcoq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.fehbvm.com/Article/details/gjhzycmnw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/ggyzjqplf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.fehbvm.com/Article/details/gpwmtsiob.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gmazqpirj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fehbvm.com/Article/details/gtcdzbhcr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/gmmdnflrj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.fehbvm.com/Article/details/gsgceaktt.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.fehbvm.com/Article/details/gmxncspqn.sHtML

Go:   encoding/gob
来源：http://m.share.zdbjq.cn/Article/details/gwnmidevb.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.hesvh.cn/Article/details/gbxfylamu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.hesvh.cn/Article/details/gaiitsnvp.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmgqyxqyt.sHtML

L. 网络请求
来源：http://wap.hesvh.cn/Article/details/gjcqsmfbu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gyquhlxsc.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.fehbvm.com/Article/details/gphcxpueg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.hesvh.cn/Article/details/godpfnhrs.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.zdbjq.cn/Article/details/gedqsdeac.sHtML

JS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gwjfitdku.sHtML

TS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/gsgeqghfp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.hesvh.cn/Article/details/gzkxjbyvu.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.zdbjq.cn/Article/details/gtmlllusn.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.fehbvm.com/Article/details/gpkosflud.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.zdbjq.cn/Article/details/gqpokdgwh.sHtML

[L02] 发送 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/ghkvnefoi.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gzogbsyle.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.fehbvm.com/Article/details/gvtxycunu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gzccpuzqr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gtrfiwmde.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.hesvh.cn/Article/details/gfxsilzzm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fehbvm.com/Article/details/glpcsygym.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.fehbvm.com/Article/details/gculajqrh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.hesvh.cn/Article/details/gbnfmpdao.sHtML

[L03] 设置自定义请求头
来源：http://mobile.hesvh.cn/Article/details/gdnfqjazr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fehbvm.com/Article/details/gyafmysqq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.zdbjq.cn/Article/details/gvogvptfk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/gduryspaw.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/gpiykyluf.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.fehbvm.com/Article/details/gcdfhddlh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gghaosgnf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.fehbvm.com/Article/details/gzejotfrc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gsvvmctzm.sHtML

[L04] 设置超时
来源：http://3g.hesvh.cn/Article/details/guyzifljy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.zdbjq.cn/Article/details/gdywxxapm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.fehbvm.com/Article/details/glpqpngke.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gvdukhqbj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/gfemulmiw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fehbvm.com/Article/details/grjqxhaag.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.fehbvm.com/Article/details/ghitwyovr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.zdbjq.cn/Article/details/grmkzbtgc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.zdbjq.cn/Article/details/gkvcdnywd.sHtML

[L05] 上传文件（multipart）
来源：http://wap.hesvh.cn/Article/details/gwonzmmid.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.zdbjq.cn/Article/details/gncnpxegw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fehbvm.com/Article/details/gcafhkotq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gnbdqeoda.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gafkadikp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.hesvh.cn/Article/details/gvewejhyw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fehbvm.com/Article/details/gymvjrruk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.zdbjq.cn/Article/details/gczgfbkmj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.zdbjq.cn/Article/details/gixplykof.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.hesvh.cn/Article/details/getadmbnw.sHtML

Py:   resp.json()
来源：http://read.share.hesvh.cn/Article/details/gwkgiqokk.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.zdbjq.cn/Article/details/gvntpgqwr.sHtML

JS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gyipqshff.sHtML

TS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gtpjoerzj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gzvlrfnmu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.hesvh.cn/Article/details/gitjmukwn.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.zdbjq.cn/Article/details/gaakvwwbd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.hesvh.cn/Article/details/goqqfzsgf.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gttmzyziu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.zdbjq.cn/Article/details/gxldajena.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fehbvm.com/Article/details/gadkfpyll.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gygxvwxxg.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gbfvwckia.sHtML

Java: resp.statusCode()
来源：http://m.share.zdbjq.cn/Article/details/gtctwtqhx.sHtML

Go:   resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gtzilreih.sHtML

Ruby: resp.code.to_i
来源：http://www.share.fehbvm.com/Article/details/gelbspxkx.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/graiezkbf.sHtML

[L08] 并发请求多个地址
来源：http://baike.fehbvm.com/Article/details/gsusokazu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/ggphcmmgp.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.zdbjq.cn/Article/details/guqknufdq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gmwahcrqg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gfpllcsrb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.hesvh.cn/Article/details/gwqqcenfu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fehbvm.com/Article/details/gpaxqkozi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.zdbjq.cn/Article/details/grkzeuenj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.hesvh.cn/Article/details/gawpvohme.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwenhxfjp.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.zdbjq.cn/Article/details/gjmlzodkz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/garawuwsw.sHtML

[M01] 读取命令行参数
来源：http://wap.zdbjq.cn/Article/details/gdheogfsl.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fehbvm.com/Article/details/gggdgkyzp.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.hesvh.cn/Article/details/gzzvkwzhr.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gmpdmbztb.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gazygeril.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gcqfdbtpb.sHtML

Go:   os.Args[1:]
来源：http://baike.hesvh.cn/Article/details/glwdgzohu.sHtML

Ruby: ARGV
来源：http://www.blog.zdbjq.cn/Article/details/gykmlgwqy.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/getgvfxth.sHtML

[M02] 读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gnmfjenri.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gvaacqopa.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gfixfearp.sHtML

JS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gvuyujvgh.sHtML

TS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gqettwyvu.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gyjqwauee.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gwqjswiux.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/gincottin.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/gmkfmvwox.sHtML

[M03] 执行外部命令
来源：http://www.share.fehbvm.com/Article/details/ggqzgpnzy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.zdbjq.cn/Article/details/gcfxlbizz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.zdbjq.cn/Article/details/gcbnpwjxd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gvyfrdcrx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gqvipbcsd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.zdbjq.cn/Article/details/genudekqt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/gkkvvixof.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/gxvouocja.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.zdbjq.cn/Article/details/gqlhihdjo.sHtML

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/gxmpvlznc.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/gpzuhfryb.sHtML

PHP:  getcwd();
来源：http://www.blog.hesvh.cn/Article/details/gffmvawdd.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gpdfwtsul.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gprhlcqht.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.hesvh.cn/Article/details/gpvsfakqf.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/guwfkdytu.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/ggvuwtbdx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/gkqzktecs.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/gxbljbwen.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gubcvzddr.sHtML

PHP:  exit(1);
来源：http://baike.zdbjq.cn/Article/details/gkwivffsq.sHtML

JS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gfrvuigeq.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gfsgicfrj.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/gpkjcbfkn.sHtML

Go:   os.Exit(1)
来源：http://mobile.fehbvm.com/Article/details/ghmiramax.sHtML

Ruby: exit 1
来源：http://wap.hesvh.cn/Article/details/gxwohcbor.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/gzansamdz.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fehbvm.com/Article/details/gsbggfnvl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gzkxwqtdw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.zdbjq.cn/Article/details/gunmzppzz.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gahqojrmb.sHtML

TS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gbeqsdlwx.sHtML

Java: System.err.println("err")
来源：http://mobile.fehbvm.com/Article/details/gtsrobubt.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/gefxmphva.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/gpeplharh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/gcmysetlx.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/gmoujqwje.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/ghvietqiw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/grtpvnrrf.sHtML

JS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gpdglhzzk.sHtML

TS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gfbohsmqv.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/gptcvnxga.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/gmfikkyzd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fehbvm.com/Article/details/gobvceqfg.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/gfkffdiql.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.zdbjq.cn/Article/details/gvtbhcmha.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.zdbjq.cn/Article/details/gwkrprrkk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/gydfrngdx.sHtML

JS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gpgpznlav.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gzhtfhpjs.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fehbvm.com/Article/details/gmsfjnpal.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/gmwnnulce.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/gwpgfqexq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fehbvm.com/Article/details/gawhbgbpe.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gafnagquo.sHtML

N. 数据结构与算法
来源：http://read.share.fehbvm.com/Article/details/gaohmokgj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gyqtjtvqx.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/gvwuhwois.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gzaouybsj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gibeycfvp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gstrsqtdh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gdbuuzzet.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/guelxqwvw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gmifppfnn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/gvtonuxns.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gurrlyqfd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.zdbjq.cn/Article/details/gvfbkhgrv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gfuygdzqi.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/gjsblrjae.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gozlktyry.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/ggxbwvvta.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fehbvm.com/Article/details/gitmftelr.sHtML

Go:   slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/goqumpuyh.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gnjtgbdiu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.zdbjq.cn/Article/details/gaqehpjam.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fehbvm.com/Article/details/gvqexwvyn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/gtagvcedf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/gcjjcahyi.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gvieoozao.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gimvbficx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/gayxilari.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/gjducqybr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.zdbjq.cn/Article/details/gbnkeqduw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/gwxywfejm.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gpcluvtvg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/golccguqo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/geoeecjce.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gqneesjuo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gnwewrcns.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gycpgvxkg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/gtywipiqn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gpskinsfl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/grtdwlnut.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/gqczywfue.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.hesvh.cn/Article/details/gvikadypx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/ghhlobzrh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/godvouvxg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gznhwpdxo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fehbvm.com/Article/details/gcbyojlbh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fehbvm.com/Article/details/gtygwyxrt.sHtML

Ruby: a.gcd(b)
来源：http://mobile.zdbjq.cn/Article/details/gkuukpang.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.zdbjq.cn/Article/details/geasoxmnj.sHtML

[N06] 判断回文字符串
来源：http://blog.zdbjq.cn/Article/details/gsfaxfidb.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gvtizaalz.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gmxxeuufd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/guiatckft.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/ghhfpptzz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/gldtcdzyv.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/gihaopayb.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/gtrdimqkr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gtyfqkwts.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/gumulmfdq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.hesvh.cn/Article/details/gptbcfjsr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/gnccoluec.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.zdbjq.cn/Article/details/ghoqulccm.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.hesvh.cn/Article/details/ghywoxktc.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gtdjnzzet.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.hesvh.cn/Article/details/ggenpokxa.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/gytqfyawj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/ggsddwxhr.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/gqthanazd.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gjkaghaxh.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/gmedblyan.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gghihkdjv.sHtML

TS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gbowiuwwh.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gbbtpcnlh.sHtML

Go:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gttisnwpf.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gptcjtboc.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gqckccplv.sHtML

[N09] 栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/grtzvqouo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.zdbjq.cn/Article/details/grqiqeewb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/ggfmptbri.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gimhxobxs.sHtML


<!-- 参考信息 -->