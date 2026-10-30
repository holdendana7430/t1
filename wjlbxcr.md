代发 wailian999

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqwsbceaf.sHtML

K. JSON 与序列化
来源：http://mobile.fehbvm.com/Article/details/gigqsigvc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtvgshoyu.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.fehbvm.com/Article/details/glorulxuh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.zdbjq.cn/Article/details/gmdciczyr.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.hesvh.cn/Article/details/gieuucugi.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.hesvh.cn/Article/details/gsmhmkwgn.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.hesvh.cn/Article/details/gnbfkytae.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.zdbjq.cn/Article/details/geylzhzjm.sHtML

Go:   json.Marshal(obj)
来源：http://baike.fehbvm.com/Article/details/gakbevrsu.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.hesvh.cn/Article/details/gbnngszpg.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.hesvh.cn/Article/details/ghahcydno.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.fehbvm.com/Article/details/ggekqshmk.sHtML

Py:   json.loads(s)
来源：http://baike.zdbjq.cn/Article/details/gfrhqszdo.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.fehbvm.com/Article/details/gpzdwkkeq.sHtML

JS:   JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gbdhgjyks.sHtML

TS:   JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gyedozeij.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gkhnpbakd.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/grkasbkcf.sHtML

Ruby: JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gbqgqxjmw.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.hesvh.cn/Article/details/gamfrxkup.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.hesvh.cn/Article/details/gxprxsjuy.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.fehbvm.com/Article/details/gnoimvfvi.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.zdbjq.cn/Article/details/gtuamlhck.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.zdbjq.cn/Article/details/gihijnukh.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.fehbvm.com/Article/details/gnecxzyoi.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.hesvh.cn/Article/details/gazlihgyq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.zdbjq.cn/Article/details/gkrbbsdgw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.hesvh.cn/Article/details/gbhcugsfv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.fehbvm.com/Article/details/gmgxtsyxt.sHtML

[K04] 读取 JSON 文件
来源：http://baike.hesvh.cn/Article/details/ggsqxzfin.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.fehbvm.com/Article/details/gjcvuzaxq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.zdbjq.cn/Article/details/gunplohro.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.hesvh.cn/Article/details/gnveecygu.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.zdbjq.cn/Article/details/gpzjquoni.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.hesvh.cn/Article/details/gqojfjnse.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.fehbvm.com/Article/details/gfecwlkgt.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.zdbjq.cn/Article/details/ggbgcijmw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.fehbvm.com/Article/details/gegrgqcwm.sHtML

[K05] 深拷贝对象
来源：http://www.blog.fehbvm.com/Article/details/gygknpqph.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gsetyifkj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.hesvh.cn/Article/details/gyaxowtez.sHtML

JS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gcqpldwnj.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gpjakccrn.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.fehbvm.com/Article/details/gcfnbzenk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.fehbvm.com/Article/details/gsckstqcc.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.zdbjq.cn/Article/details/gydtogtxj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.hesvh.cn/Article/details/gltkkjdqd.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.hesvh.cn/Article/details/gtyujwokp.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/gwoaocdwb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.fehbvm.com/Article/details/gocmbydtx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/gdoripwat.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gfzmdykmw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.zdbjq.cn/Article/details/ghctwhctn.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gcnlrjxnl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gmqybwjth.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/glxisntzt.sHtML

[K07] 进制转换
来源：http://m.share.fehbvm.com/Article/details/gzrbtyenj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gqcwbbnzx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.zdbjq.cn/Article/details/gemwzcthq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gbsummjow.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gnihagvyq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/grbebqbba.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.fehbvm.com/Article/details/gjjdsncyb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.zdbjq.cn/Article/details/gjngbxyje.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gjjlalpdf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.zdbjq.cn/Article/details/gjpnylkij.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.fehbvm.com/Article/details/gnwsoneba.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.fehbvm.com/Article/details/gmptufpds.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/gvuqbjxjh.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/grrhbhuum.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.hesvh.cn/Article/details/gjsojikxi.sHtML

Go:   encoding/gob
来源：http://mobile.zdbjq.cn/Article/details/gdsphkias.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.zdbjq.cn/Article/details/ghxhcwtps.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gwbspnbik.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggiehjumw.sHtML

L. 网络请求
来源：http://www.m.share.fehbvm.com/Article/details/gpspgmnyv.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxrlswgug.sHtML

[L01] 发送 GET 请求
来源：http://blog.fehbvm.com/Article/details/glsuuqzid.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.hesvh.cn/Article/details/gzsggragz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.hesvh.cn/Article/details/gimuskvze.sHtML

JS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gqfdsyozh.sHtML

TS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/grxbydfpe.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fehbvm.com/Article/details/gjewqumky.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.zdbjq.cn/Article/details/guxrodydg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.hesvh.cn/Article/details/gvbclvlez.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.hesvh.cn/Article/details/gcasaeqph.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/grvvxiuad.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.hesvh.cn/Article/details/ghyhqmbmr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.fehbvm.com/Article/details/goynganmw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/gsgweabbg.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/grtvxqysn.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.zdbjq.cn/Article/details/gxolqdnbq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.hesvh.cn/Article/details/gvugjxpni.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.hesvh.cn/Article/details/gegqqxejf.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.hesvh.cn/Article/details/gziksuqid.sHtML

[L03] 设置自定义请求头
来源：http://read.share.zdbjq.cn/Article/details/gowasemri.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.fehbvm.com/Article/details/gkdcmhvci.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fehbvm.com/Article/details/gyofybatr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/gtvyadfot.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gigbieros.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fehbvm.com/Article/details/gxkxwgclt.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/glwofpmzm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fehbvm.com/Article/details/gvumbwvbz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gfnwlupvn.sHtML

[L04] 设置超时
来源：http://mobile.fehbvm.com/Article/details/gexemberg.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.hesvh.cn/Article/details/gppvqgkuo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.hesvh.cn/Article/details/gsxioxvfg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/gzbpjpamh.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/ggmytfyww.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.hesvh.cn/Article/details/guqktvpzm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.zdbjq.cn/Article/details/gxqtzmxsf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.zdbjq.cn/Article/details/gzwuofvuh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fehbvm.com/Article/details/gittlpudw.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.hesvh.cn/Article/details/gkhxzsycj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fehbvm.com/Article/details/gidlcykaf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.zdbjq.cn/Article/details/grvvmyfws.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/grsbjfnpv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/ggkmklhix.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.zdbjq.cn/Article/details/gjuvejmcs.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fehbvm.com/Article/details/gvdfuahjc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.zdbjq.cn/Article/details/gtejqgoqb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gtgcefhge.sHtML

[L06] 解析响应为 JSON
来源：http://baike.hesvh.cn/Article/details/gkaviqqxu.sHtML

Py:   resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gkyuvwnba.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.hesvh.cn/Article/details/glvvrwdmp.sHtML

JS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gqzrckdnp.sHtML

TS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gfgvbkhzn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gazhicdbc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/gbpclqfok.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.hesvh.cn/Article/details/gpdntziod.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fehbvm.com/Article/details/gmdgmgfxw.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gvllczqmw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.hesvh.cn/Article/details/gnmrgtpqr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fehbvm.com/Article/details/geusubwie.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gzdlgihwp.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gjbcsfmix.sHtML

Java: resp.statusCode()
来源：http://blog.fehbvm.com/Article/details/gerpueqds.sHtML

Go:   resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gcpexgtwb.sHtML

Ruby: resp.code.to_i
来源：http://blog.hesvh.cn/Article/details/gdmytboyt.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gctwweeqe.sHtML

[L08] 并发请求多个地址
来源：http://www.share.zdbjq.cn/Article/details/gudwuwqkc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.zdbjq.cn/Article/details/gswwcrtdo.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.zdbjq.cn/Article/details/gkpmpqkql.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gonwuhbkd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gqwsftfqj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.hesvh.cn/Article/details/grxnidbfm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.zdbjq.cn/Article/details/gctdbczkh.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fehbvm.com/Article/details/gufpagqel.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fehbvm.com/Article/details/glojbfalj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmuhemfcs.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.hesvh.cn/Article/details/ghxohojrt.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtvtqjcrd.sHtML

[M01] 读取命令行参数
来源：http://baike.fehbvm.com/Article/details/gioswrcbj.sHtML

Py:   sys.argv[1:]
来源：http://wap.fehbvm.com/Article/details/gjozlgyld.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.hesvh.cn/Article/details/gelvamskb.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gewifgceb.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/guctpvsso.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/ggkdtejwt.sHtML

Go:   os.Args[1:]
来源：http://baike.hesvh.cn/Article/details/glxacbsuc.sHtML

Ruby: ARGV
来源：http://3g.zdbjq.cn/Article/details/gnmcqvryb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gwjyjelcd.sHtML

[M02] 读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gisshjgzg.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gcygwuxlr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/ggikfpcqa.sHtML

JS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gnazsavno.sHtML

TS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gmrfgjvbp.sHtML

Java: System.getenv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gvcyidhqi.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.zdbjq.cn/Article/details/grnkugody.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/gebosmlsb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fehbvm.com/Article/details/gauovyukb.sHtML

[M03] 执行外部命令
来源：http://read.share.fehbvm.com/Article/details/gcrdnmodx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.zdbjq.cn/Article/details/grloaphqv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.hesvh.cn/Article/details/gpiefhley.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gpqmmvlce.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gxanelqeu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.hesvh.cn/Article/details/gagnjppwi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/gvtdrrmyh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fehbvm.com/Article/details/ghwscgaii.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.zdbjq.cn/Article/details/gmppfimri.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/gppfmfcxd.sHtML

Py:   os.getcwd()
来源：http://www.share.hesvh.cn/Article/details/gfapacctz.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gchtgpsox.sHtML

JS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/galrtpvos.sHtML

TS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gwdgkdatk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.hesvh.cn/Article/details/gcdcwwbsf.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fehbvm.com/Article/details/ggqjkbiku.sHtML

Ruby: Dir.pwd
来源：http://blog.zdbjq.cn/Article/details/gwbbgmwaf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/gfdrisvvm.sHtML

[M05] 设置退出码
来源：http://www.share.zdbjq.cn/Article/details/ggkazhjza.sHtML

Py:   sys.exit(1)
来源：http://3g.fehbvm.com/Article/details/gdfbfkacc.sHtML

PHP:  exit(1);
来源：http://read.share.fehbvm.com/Article/details/gqiudzmqo.sHtML

JS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gdwiibpjr.sHtML

TS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gtokmtlze.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/gcsmwewbh.sHtML

Go:   os.Exit(1)
来源：http://baike.fehbvm.com/Article/details/gbktjuodd.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/gabilovcx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/gaxxdkjdf.sHtML

[M06] 向标准错误输出
来源：http://m.share.fehbvm.com/Article/details/gpfduwgqh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gnkjuneqd.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.hesvh.cn/Article/details/ghpzzkswj.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/ghaamtlfg.sHtML

TS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gdqckxfxz.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/gynrdgkkz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fehbvm.com/Article/details/gogmkpljo.sHtML

Ruby: warn "err"
来源：http://m.share.hesvh.cn/Article/details/gayyugfgv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.hesvh.cn/Article/details/gqbolwqkm.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/gjxidxyjv.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/guvqpwrar.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/gujgojgur.sHtML

JS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gpomtmvie.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gyzlfbnpg.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.hesvh.cn/Article/details/gbqxcquxu.sHtML

Go:   func main()
来源：http://www.share.zdbjq.cn/Article/details/gupqrnaay.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.zdbjq.cn/Article/details/grsqczusl.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fehbvm.com/Article/details/gfjhbldpj.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/ggvvaouzk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fehbvm.com/Article/details/guttuvirt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.zdbjq.cn/Article/details/grvevqnex.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gkrzsinvn.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gezcrtvzb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/gajkhpets.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.hesvh.cn/Article/details/gkrnhkjor.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/gdwunplip.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fehbvm.com/Article/details/gvuvglyxo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gnnlbjbgw.sHtML

N. 数据结构与算法
来源：http://read.share.zdbjq.cn/Article/details/gogvxoylg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gboxsukym.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/gxncpwyje.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gqwdnvhvo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/gwyilletn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gjwhqwvyn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gooxtxycy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/ghzlazwna.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gsplequir.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/gtxfzafbi.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gcrappdka.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.zdbjq.cn/Article/details/gokgxnsif.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gjnsfyktz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gmqiqkbfc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gvjahtpeu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gxrajhoxs.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/gxmzkqnzi.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/ganocuouq.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gahoigqmv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.hesvh.cn/Article/details/guztwxoln.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fehbvm.com/Article/details/gsuzjenqk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/gvonmdhnc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.zdbjq.cn/Article/details/gdodmzehw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/giewwqyfd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gjzlrdjag.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/gextpxntr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/gsgnlnrnh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/gbqkrjxti.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/gshejuytd.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gjtyyavhz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/ggwialeti.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbmxdefkk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/guktcauup.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gsolslcxn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gdxattiyy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.zdbjq.cn/Article/details/gabrzuvby.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gcxqauqfr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gjupdwwbh.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/gniofnlbk.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/giuxrjfye.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.zdbjq.cn/Article/details/gvuwvnwgh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gifwayeao.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gbtjoolry.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/gnblevlxe.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gnyhekddn.sHtML

Ruby: a.gcd(b)
来源：http://3g.zdbjq.cn/Article/details/gwzakkrtg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.zdbjq.cn/Article/details/gufotexox.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gjgrzpntt.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/ggysawicr.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/gwatbpkaf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gmvepodum.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gyesvbxin.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fehbvm.com/Article/details/gdebbzivl.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fehbvm.com/Article/details/gsrmwzyiw.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fehbvm.com/Article/details/glxqowivw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/glfsvrqba.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/gimkzqzrb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/gdcoiltqn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.hesvh.cn/Article/details/ggemnolnx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.hesvh.cn/Article/details/gkurdoily.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/gmkddeoei.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/gdktravbe.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.hesvh.cn/Article/details/gvvtkgrdj.sHtML

Ruby: // 手写 Hash
来源：http://blog.hesvh.cn/Article/details/gfhewljll.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fehbvm.com/Article/details/gakiwmtvi.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/gzgnmwynx.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/gvhiwwrvm.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/gyzoqcoex.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gaquuhcjt.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gmyhbqjci.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/glsbtrqkm.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gugswekhh.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/gdeqbwwxm.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gnhcnxldg.sHtML


<!-- 参考信息 -->