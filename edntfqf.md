代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.hesvh.cn/Article/details/gknivrfpd.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.zdbjq.cn/Article/details/gmjopuxgn.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.zdbjq.cn/Article/details/gbdnuxxdf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.zdbjq.cn/Article/details/ghdllxgak.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.hesvh.cn/Article/details/gkppqfioa.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.fehbvm.com/Article/details/gsywyntyk.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.hesvh.cn/Article/details/gvnyuaeai.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.fehbvm.com/Article/details/gesjovguq.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gcneoemly.sHtML

K. JSON 与序列化
来源：http://m.share.zdbjq.cn/Article/details/gncalhvra.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjpxwvhho.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.fehbvm.com/Article/details/gwpmnubkl.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.fehbvm.com/Article/details/godmddcoz.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.hesvh.cn/Article/details/gsjarnhnc.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.hesvh.cn/Article/details/gfdedlepu.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.zdbjq.cn/Article/details/goaujzamt.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.hesvh.cn/Article/details/gsvzgpklm.sHtML

Go:   json.Marshal(obj)
来源：http://3g.hesvh.cn/Article/details/gibqsxfnd.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.hesvh.cn/Article/details/gdlkpkysv.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.hesvh.cn/Article/details/gkvbfdain.sHtML

[K02] JSON 字符串转对象
来源：http://blog.zdbjq.cn/Article/details/glfqygshj.sHtML

Py:   json.loads(s)
来源：http://3g.hesvh.cn/Article/details/gpqtjqrnu.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.fehbvm.com/Article/details/ghfwagrep.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gwvhmwyzf.sHtML

TS:   JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/grbesensc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.zdbjq.cn/Article/details/glhsqqgkg.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.fehbvm.com/Article/details/gmwdijjnk.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/geusmxcvb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.hesvh.cn/Article/details/gwdhemnsl.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.fehbvm.com/Article/details/gaqnfrbvm.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.hesvh.cn/Article/details/gwgctiwkv.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.fehbvm.com/Article/details/gxpnkveqb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fehbvm.com/Article/details/gdqqyruxr.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.zdbjq.cn/Article/details/gynbtilta.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.zdbjq.cn/Article/details/ggwoqbqqc.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.fehbvm.com/Article/details/gsqrbcjgh.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.zdbjq.cn/Article/details/gjfpzibks.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.hesvh.cn/Article/details/gsfoxqbwi.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.fehbvm.com/Article/details/gmmgiinbb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.zdbjq.cn/Article/details/gcsnkwdik.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.zdbjq.cn/Article/details/gouqlkxjm.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.hesvh.cn/Article/details/gdwlnmtde.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.zdbjq.cn/Article/details/gbsmiitdq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.hesvh.cn/Article/details/glthssfsj.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.fehbvm.com/Article/details/gqrqdgmzl.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.zdbjq.cn/Article/details/guyknridj.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.hesvh.cn/Article/details/gcuammabz.sHtML

[K05] 深拷贝对象
来源：http://baike.zdbjq.cn/Article/details/gypuhtkvn.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.fehbvm.com/Article/details/gnjrtovwy.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.zdbjq.cn/Article/details/gbumkqtlt.sHtML

JS:   structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gjxhcrznn.sHtML

TS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gqkkktrys.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.zdbjq.cn/Article/details/gchejwqfe.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.fehbvm.com/Article/details/gvinekfjt.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.zdbjq.cn/Article/details/golnbcpgj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.hesvh.cn/Article/details/gufvlvlvv.sHtML

[K06] 解析 URL 查询串
来源：http://blog.fehbvm.com/Article/details/gnioxfbyw.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.hesvh.cn/Article/details/gffaejejg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.zdbjq.cn/Article/details/gxacrlsqy.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/gxsiolyny.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.hesvh.cn/Article/details/gucgdsxxe.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gwhowrbqq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gjptuzqex.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/ggeomdypm.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/garvbwfid.sHtML

[K07] 进制转换
来源：http://baike.zdbjq.cn/Article/details/gwtjowadz.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gjvjpcgkf.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.fehbvm.com/Article/details/gkezsoshu.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gneswqoqq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gstvevysx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/geoojczym.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.fehbvm.com/Article/details/gfkhlzhsm.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.hesvh.cn/Article/details/geihnwzbz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gzgvdsohx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.hesvh.cn/Article/details/gwbxuhvbh.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.zdbjq.cn/Article/details/gyjbigczm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.zdbjq.cn/Article/details/gjbancmmz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/gvcdctkgt.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/grrsgniby.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.zdbjq.cn/Article/details/gsryfplls.sHtML

Go:   encoding/gob
来源：http://baike.fehbvm.com/Article/details/gkozlswnq.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.fehbvm.com/Article/details/gagpupkpv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gaulwnmok.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqzvpbsbw.sHtML

L. 网络请求
来源：http://www.m.share.fehbvm.com/Article/details/gicjuluxi.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/guxteawvi.sHtML

[L01] 发送 GET 请求
来源：http://wap.fehbvm.com/Article/details/geraschwy.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.hesvh.cn/Article/details/gpprabzqr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fehbvm.com/Article/details/ghvthmqmh.sHtML

JS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gitmgqkna.sHtML

TS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gyvgyycjt.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.zdbjq.cn/Article/details/gyjxhjdfq.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.hesvh.cn/Article/details/gqedgqipj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.hesvh.cn/Article/details/gomienhod.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.fehbvm.com/Article/details/gtayywjfg.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gnhvyqmqd.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gxbqggxis.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.hesvh.cn/Article/details/gpbcvxuvw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gtwmzqirt.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gjetcopyy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.fehbvm.com/Article/details/gzdqdkxws.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.hesvh.cn/Article/details/gzvrnrqkg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.zdbjq.cn/Article/details/gznuufugd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.zdbjq.cn/Article/details/gxkxyonvp.sHtML

[L03] 设置自定义请求头
来源：http://m.share.fehbvm.com/Article/details/gqwoleohg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fehbvm.com/Article/details/gmuypmrdj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.fehbvm.com/Article/details/ggmhbjtos.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/ginhlmzjo.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/gfrxvxaxr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.fehbvm.com/Article/details/gwacnfjjh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/gwkgwmfpp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.hesvh.cn/Article/details/gylwohbxh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gdzlfvwka.sHtML

[L04] 设置超时
来源：http://www.share.hesvh.cn/Article/details/ggyrzaphs.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.hesvh.cn/Article/details/grovedfuo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.hesvh.cn/Article/details/gsqvfhcay.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/gvodljdgg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/geqxbphrg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fehbvm.com/Article/details/gnhwmrukt.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.hesvh.cn/Article/details/geyrpapal.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.zdbjq.cn/Article/details/gafbdqbeb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.zdbjq.cn/Article/details/gfvufbixz.sHtML

[L05] 上传文件（multipart）
来源：http://baike.zdbjq.cn/Article/details/grxnessdw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.hesvh.cn/Article/details/guucrxtfy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fehbvm.com/Article/details/gbstlcser.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gmdnsgtri.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gpnirkprc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.hesvh.cn/Article/details/gbvpkwtvb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fehbvm.com/Article/details/gnlvkdkbp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.zdbjq.cn/Article/details/glihqvoza.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.zdbjq.cn/Article/details/ganmtpwvp.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.fehbvm.com/Article/details/ghxyrcxhe.sHtML

Py:   resp.json()
来源：http://mobile.hesvh.cn/Article/details/grthmvakw.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.zdbjq.cn/Article/details/gvbsmgyor.sHtML

JS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gjczjpzor.sHtML

TS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gupvdiydd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gmwlqugee.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fehbvm.com/Article/details/ghbnanosb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fehbvm.com/Article/details/gfejanset.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.hesvh.cn/Article/details/gwjndigzc.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gyiqrjnqc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fehbvm.com/Article/details/gliytzrft.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.hesvh.cn/Article/details/gtbxfsyff.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gaeyaqhdh.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gsfdzewdj.sHtML

Java: resp.statusCode()
来源：http://read.share.hesvh.cn/Article/details/ghzpfzrbp.sHtML

Go:   resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gtgblsxgd.sHtML

Ruby: resp.code.to_i
来源：http://mobile.zdbjq.cn/Article/details/glyvabphe.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gzzpnrgej.sHtML

[L08] 并发请求多个地址
来源：http://www.share.zdbjq.cn/Article/details/grxlotdus.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fehbvm.com/Article/details/gafqufpmh.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.zdbjq.cn/Article/details/gdekifppk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gikzygajc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gztozjscd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fehbvm.com/Article/details/gxfbgunhf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.hesvh.cn/Article/details/gzvokamcm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.hesvh.cn/Article/details/gbutveiys.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.hesvh.cn/Article/details/gwmahgsat.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpvgbktfb.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fehbvm.com/Article/details/ggskdemgh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grdfmgozh.sHtML

[M01] 读取命令行参数
来源：http://wap.zdbjq.cn/Article/details/gkamwohny.sHtML

Py:   sys.argv[1:]
来源：http://baike.zdbjq.cn/Article/details/gvryvtxck.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fehbvm.com/Article/details/gvlwdojut.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gnmgtfibu.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gzyzjkanh.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gfjojwexc.sHtML

Go:   os.Args[1:]
来源：http://m.share.zdbjq.cn/Article/details/gqwkcczqd.sHtML

Ruby: ARGV
来源：http://www.m.share.fehbvm.com/Article/details/gxegybtjr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gximgxzpy.sHtML

[M02] 读取环境变量
来源：http://baike.hesvh.cn/Article/details/gkaelulpv.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.zdbjq.cn/Article/details/gavbpativ.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/geqzmvgds.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gaqnijzvb.sHtML

TS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gymysekvi.sHtML

Java: System.getenv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gbfpbttsv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gezgrjiuf.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.zdbjq.cn/Article/details/gfiztxect.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.hesvh.cn/Article/details/glytnlwzs.sHtML

[M03] 执行外部命令
来源：http://www.blog.zdbjq.cn/Article/details/ggizjvrng.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fehbvm.com/Article/details/gtukthtro.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.hesvh.cn/Article/details/gljkdkmbh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gdkxlbblc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/grcftzjkk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.zdbjq.cn/Article/details/gjayxvfwj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.hesvh.cn/Article/details/gucjzvejh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/gneghiwhr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.hesvh.cn/Article/details/gwemnlfxi.sHtML

[M04] 获取当前工作目录
来源：http://wap.zdbjq.cn/Article/details/gcsnvlbpa.sHtML

Py:   os.getcwd()
来源：http://wap.fehbvm.com/Article/details/giltagwck.sHtML

PHP:  getcwd();
来源：http://www.share.fehbvm.com/Article/details/gpzveezgb.sHtML

JS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gscoksavz.sHtML

TS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gyordwalk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/gsikbgtpi.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fehbvm.com/Article/details/gguctntnl.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.hesvh.cn/Article/details/gaxyrobid.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.fehbvm.com/Article/details/gsqjjwurm.sHtML

[M05] 设置退出码
来源：http://www.share.hesvh.cn/Article/details/giywfduct.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gpspxotpe.sHtML

PHP:  exit(1);
来源：http://mobile.fehbvm.com/Article/details/gnnzbhzkf.sHtML

JS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/ggkeefgrs.sHtML

TS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/ghgzxaira.sHtML

Java: System.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gjembawyq.sHtML

Go:   os.Exit(1)
来源：http://mobile.fehbvm.com/Article/details/gwanmxltz.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/gyqdbohaq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fehbvm.com/Article/details/glviafjrx.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/gnlkjvard.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/glbvjgpgq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/gqxjqqsdw.sHtML

JS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/ggfneujiw.sHtML

TS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gfuzskzoe.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/gnqzdffqd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.hesvh.cn/Article/details/gkppcwqzp.sHtML

Ruby: warn "err"
来源：http://www.share.zdbjq.cn/Article/details/gcsimwxrs.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gieouoqrh.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/gbcorfiet.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.hesvh.cn/Article/details/ggmfmujaa.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/gfhrraqlx.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/ginvydtlf.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gogeoqcln.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gjozdqzmn.sHtML

Go:   func main()
来源：http://www.blog.hesvh.cn/Article/details/gwrfajsdb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.hesvh.cn/Article/details/gnygszfsu.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/gcdjearzd.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/ggfylvprt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.hesvh.cn/Article/details/gebgzuslx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.zdbjq.cn/Article/details/gdntplkkv.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gppvzbnwj.sHtML

TS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gdkiibcku.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.zdbjq.cn/Article/details/gisnlowso.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/gfjyryuoy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/gypxprdod.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/gigwzoedj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfvthtrpk.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gnopcxrzm.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gimelqykm.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fehbvm.com/Article/details/goeofsehk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gtromsuvf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fehbvm.com/Article/details/gaevzevbk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/ggkgtrfoi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gzlkitzeg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gcencujhr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gxfmqeqzk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.zdbjq.cn/Article/details/gmidipdzw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gxlmpsacd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/gzwswhzox.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gicrqdfxv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.hesvh.cn/Article/details/grjwgmzbz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gfcsiuadj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gsafdfdna.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/gvddpalve.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gmpvtpvzc.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gobadteqh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.zdbjq.cn/Article/details/gccyztrrd.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.hesvh.cn/Article/details/gdhjwnvwd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.zdbjq.cn/Article/details/gailwmjnf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fehbvm.com/Article/details/gqumexnby.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gkhyifdbl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gxuycojfh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/gjdhonbto.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/gwngblmpg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/gzskksrhv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/gqwabptps.sHtML

[N04] 斐波那契数列
来源：http://wap.fehbvm.com/Article/details/gzcdlcnei.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/glflgpqcr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gfyjvxkks.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gecbhewxx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gggwkkfsy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gwnhreonq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.zdbjq.cn/Article/details/gjwvltydg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gouvnwvni.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gzstvlqgo.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/gdjqtmdvf.sHtML

Py:   math.gcd(a, b)
来源：http://wap.hesvh.cn/Article/details/greoiufgx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/gcbomdqni.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gxekoegia.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gseymzfqn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/ghsipznlc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/guwoofrdc.sHtML

Ruby: a.gcd(b)
来源：http://blog.zdbjq.cn/Article/details/grjoquluf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/gowcxkdzh.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/ggvyfjnrj.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/grvufqsme.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gxmfjldxj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gdmwocylt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gtfsnpdjk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/gkdhivjmm.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/gvllhmeko.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gmgtfonno.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gbhbkhygq.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.zdbjq.cn/Article/details/ghfengsum.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/gyvpngqjz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/gfotvgjjc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/gnuptxjjc.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/gpjkmvumw.sHtML

Java: // 手写 HashMap
来源：http://mobile.zdbjq.cn/Article/details/gqvnhbpzq.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.hesvh.cn/Article/details/gabuxpuwt.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fehbvm.com/Article/details/gwwpxxmay.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.hesvh.cn/Article/details/gxylitqov.sHtML

[N08] 生成全排列
来源：http://baike.zdbjq.cn/Article/details/gijnaulnj.sHtML


<!-- 参考信息 -->