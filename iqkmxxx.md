代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.fehbvm.com/Article/details/gakvybfji.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.zdbjq.cn/Article/details/gpahkjwhn.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.hesvh.cn/Article/details/gyfpetast.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.zdbjq.cn/Article/details/gvimjskav.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.zdbjq.cn/Article/details/gbbdqkeyw.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.hesvh.cn/Article/details/gbwhnpdcf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.zdbjq.cn/Article/details/gtruckayw.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.fehbvm.com/Article/details/gyfzfqfww.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.hesvh.cn/Article/details/gjchcsxbw.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.zdbjq.cn/Article/details/grffujtxq.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.fehbvm.com/Article/details/gkzkjmkgo.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gkvgzyjvu.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.fehbvm.com/Article/details/glizioott.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.fehbvm.com/Article/details/gsrgfmkmc.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.hesvh.cn/Article/details/gncvdcpor.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.fehbvm.com/Article/details/gamberoyc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gekhbilyw.sHtML

K. JSON 与序列化
来源：http://wap.fehbvm.com/Article/details/gvqkcokwi.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grizcdxte.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.zdbjq.cn/Article/details/gbinzaxxb.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.zdbjq.cn/Article/details/gqlupprib.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.fehbvm.com/Article/details/goerrwryb.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.hesvh.cn/Article/details/gqgukxkgs.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.hesvh.cn/Article/details/ghjmbvkzc.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.fehbvm.com/Article/details/gltpxrxho.sHtML

Go:   json.Marshal(obj)
来源：http://blog.hesvh.cn/Article/details/gbfsvfunj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.fehbvm.com/Article/details/gsesaoqed.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.hesvh.cn/Article/details/gmukumgwv.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.zdbjq.cn/Article/details/guxbgvakr.sHtML

Py:   json.loads(s)
来源：http://baike.fehbvm.com/Article/details/gplaqfevc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.zdbjq.cn/Article/details/gvyitulve.sHtML

JS:   JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/grgtkfcmh.sHtML

TS:   JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/gjxnngdko.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.hesvh.cn/Article/details/gchnkwbig.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/gbpsayhpo.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gqpnedmnk.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.zdbjq.cn/Article/details/ggfilvhxt.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.hesvh.cn/Article/details/gezsucoef.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.hesvh.cn/Article/details/ghvylbaru.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.zdbjq.cn/Article/details/gkczizzhy.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.hesvh.cn/Article/details/gvotlvgmn.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.zdbjq.cn/Article/details/glwogtsqe.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.hesvh.cn/Article/details/gbispofqv.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.zdbjq.cn/Article/details/ggpgdcfnd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.fehbvm.com/Article/details/gzukjsmgb.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.fehbvm.com/Article/details/gnqnrqjtp.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.hesvh.cn/Article/details/gliwqpuqu.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.zdbjq.cn/Article/details/gnviiyisg.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.zdbjq.cn/Article/details/gofuqbkwg.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.zdbjq.cn/Article/details/gkvpcfgop.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.zdbjq.cn/Article/details/gpshzqrzt.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/glefdjpbi.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/gniwazpyc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.fehbvm.com/Article/details/gyuisiypr.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.zdbjq.cn/Article/details/gfzgjmreb.sHtML

[K05] 深拷贝对象
来源：http://read.share.hesvh.cn/Article/details/gpipcqmua.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.zdbjq.cn/Article/details/gdbeddpxc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.fehbvm.com/Article/details/gowwvvmxg.sHtML

JS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gjzuvwngz.sHtML

TS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/geqckzysy.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.fehbvm.com/Article/details/gsnbvresn.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.hesvh.cn/Article/details/gtqbesxoy.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.fehbvm.com/Article/details/gtznychin.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.zdbjq.cn/Article/details/gknnswjbv.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.zdbjq.cn/Article/details/gekpxrihk.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/gtrexlbwx.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.zdbjq.cn/Article/details/gawwhtbba.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/giavkhbdf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/gewdaaaod.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.zdbjq.cn/Article/details/ggljdxaxz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gmxmsxqow.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gkulvwmhm.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/ghiqlysca.sHtML

[K07] 进制转换
来源：http://3g.fehbvm.com/Article/details/gtwdjwaca.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gfueehrxc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.hesvh.cn/Article/details/gdbkdeuoo.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/glxeqzgic.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gfvwgzutu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gvzomkuxm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.hesvh.cn/Article/details/ggtzgqckr.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.fehbvm.com/Article/details/gunhsbtyg.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/ghufcyzhg.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.hesvh.cn/Article/details/gmwmeodfj.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.hesvh.cn/Article/details/gxtojjqsl.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.hesvh.cn/Article/details/gehhnxvir.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/ggzmjgfkt.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/gktpebjnm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.fehbvm.com/Article/details/glatokzft.sHtML

Go:   encoding/gob
来源：http://mobile.hesvh.cn/Article/details/gsqybsqgr.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.zdbjq.cn/Article/details/gtspcvyrb.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gluybjmfe.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtvivqick.sHtML

L. 网络请求
来源：http://mobile.fehbvm.com/Article/details/gwrevbvwb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmgyczqey.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.zdbjq.cn/Article/details/gjexqjzfh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.zdbjq.cn/Article/details/gazvyqbjb.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.hesvh.cn/Article/details/grqfxlcza.sHtML

JS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/gddfqzlcm.sHtML

TS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/gsmrdprfb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.hesvh.cn/Article/details/gshdouofa.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.fehbvm.com/Article/details/ggymutbpn.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.zdbjq.cn/Article/details/gtngkrnwb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.zdbjq.cn/Article/details/ghjnzhxzs.sHtML

[L02] 发送 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/ggqwrsnst.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gqahizcji.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.fehbvm.com/Article/details/gxqwcmuer.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gitoasgho.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/gehdwvsxh.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gnyuvxakh.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.hesvh.cn/Article/details/giszoijhf.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.zdbjq.cn/Article/details/grbrwrxkw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.hesvh.cn/Article/details/gdrccpyuo.sHtML

[L03] 设置自定义请求头
来源：http://mobile.hesvh.cn/Article/details/gddbpckjx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.zdbjq.cn/Article/details/gdubcurty.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.hesvh.cn/Article/details/gfmtvdaoa.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gsxomywxa.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gyecppomk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.hesvh.cn/Article/details/gigbcxqph.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gltdlvngb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.hesvh.cn/Article/details/gndpdvtuv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/gomlbwtgo.sHtML

[L04] 设置超时
来源：http://www.m.share.fehbvm.com/Article/details/gcnpiwqjt.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.zdbjq.cn/Article/details/gtazqkpao.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gyckzydye.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gfgapzkkf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gmmfuxeqh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gwjwuidwq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fehbvm.com/Article/details/gbdmuajxn.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.zdbjq.cn/Article/details/gizepsqzc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.zdbjq.cn/Article/details/gvusfzfyx.sHtML

[L05] 上传文件（multipart）
来源：http://wap.hesvh.cn/Article/details/gakhvvdmf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.hesvh.cn/Article/details/gvybmlsig.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.zdbjq.cn/Article/details/gvrqfhdvi.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gjwpejcya.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gkahtmcob.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fehbvm.com/Article/details/gxmvisphs.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.hesvh.cn/Article/details/gqadmvnzb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.zdbjq.cn/Article/details/giojgxyzb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gcatoqoey.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gcktifwsw.sHtML

Py:   resp.json()
来源：http://wap.zdbjq.cn/Article/details/gztxvnbag.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fehbvm.com/Article/details/gcqagdkbe.sHtML

JS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gynvkisml.sHtML

TS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gjnqttvlx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.hesvh.cn/Article/details/gcezybeml.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fehbvm.com/Article/details/gwwhmcyid.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.zdbjq.cn/Article/details/gvdwdmpcz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fehbvm.com/Article/details/grozzkhvq.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gsvniyvyt.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.zdbjq.cn/Article/details/gxecyexql.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fehbvm.com/Article/details/gpcmofmdp.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/glzozryfx.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gpvobayve.sHtML

Java: resp.statusCode()
来源：http://3g.zdbjq.cn/Article/details/gknjyxiei.sHtML

Go:   resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gnaviumux.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fehbvm.com/Article/details/gbweojyuc.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/glcynwynd.sHtML

[L08] 并发请求多个地址
来源：http://3g.zdbjq.cn/Article/details/gvvwanwmd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.fehbvm.com/Article/details/gkywyrxms.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fehbvm.com/Article/details/gaifoqljw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gcrxtehly.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gqlxwmglg.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.hesvh.cn/Article/details/ggitneqrh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fehbvm.com/Article/details/gdczsvimk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gjsljrbqn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.fehbvm.com/Article/details/gnzgqogey.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwaxocrwy.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.hesvh.cn/Article/details/gokxbqknc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdfblspjx.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/girbewxzg.sHtML

Py:   sys.argv[1:]
来源：http://baike.hesvh.cn/Article/details/glsjlqazs.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fehbvm.com/Article/details/gjxfcqmma.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gvassrwhq.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gvqdykemj.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gbcmfqfye.sHtML

Go:   os.Args[1:]
来源：http://m.share.fehbvm.com/Article/details/gocppglwo.sHtML

Ruby: ARGV
来源：http://wap.fehbvm.com/Article/details/gorpaxdzh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gxlqdqhli.sHtML

[M02] 读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gkxdwibfp.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.hesvh.cn/Article/details/gdmkryjsf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gsyebcxgx.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gkukuilip.sHtML

TS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/glddtrdtk.sHtML

Java: System.getenv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gncrpsrnx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.hesvh.cn/Article/details/grqlrvrat.sHtML

Ruby: ENV["HOME"]
来源：http://blog.zdbjq.cn/Article/details/gntlkzwuq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.hesvh.cn/Article/details/gjpkfhccq.sHtML

[M03] 执行外部命令
来源：http://blog.hesvh.cn/Article/details/gqfdyxwhi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fehbvm.com/Article/details/gsusyhtdu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.hesvh.cn/Article/details/givdzwsoe.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gbelkudbt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gbxpopeoz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.hesvh.cn/Article/details/gpjoaqilk.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.zdbjq.cn/Article/details/gltvfluah.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.hesvh.cn/Article/details/gyspfrjxd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fehbvm.com/Article/details/gibhtsblv.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fehbvm.com/Article/details/giktowjaj.sHtML

Py:   os.getcwd()
来源：http://blog.fehbvm.com/Article/details/gyxserqja.sHtML

PHP:  getcwd();
来源：http://baike.hesvh.cn/Article/details/gzjnjuqia.sHtML

JS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gkkoflfve.sHtML

TS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/glsshedkq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fehbvm.com/Article/details/gbcexnimf.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/ghxvodimh.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/ggskvofnd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fehbvm.com/Article/details/gqhdxzojg.sHtML

[M05] 设置退出码
来源：http://www.blog.zdbjq.cn/Article/details/gadolvnfe.sHtML

Py:   sys.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gtaxmnnrq.sHtML

PHP:  exit(1);
来源：http://www.share.fehbvm.com/Article/details/geodxsmfs.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gtixhdyuh.sHtML

TS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gbgyfyrlj.sHtML

Java: System.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gxfjjwjxv.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/gdzfgfzjp.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/gysmzeaop.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.hesvh.cn/Article/details/gcfenlreu.sHtML

[M06] 向标准错误输出
来源：http://wap.fehbvm.com/Article/details/gvxvvfscy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gylhoaask.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.zdbjq.cn/Article/details/gnyfwuzld.sHtML

JS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gzjxneezq.sHtML

TS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/giwilkhye.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/gyqrwxolv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/gjeswqfnl.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/gqifbnnsg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fehbvm.com/Article/details/gbqulxgoc.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/gfgpknaru.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/gwqqmymlm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/gfkqcsgbg.sHtML

JS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gnwjbzmdp.sHtML

TS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gzuszuffo.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/gzhgjcydr.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/gqewczlkb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/gwycqticr.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.zdbjq.cn/Article/details/gsaylivwv.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/glrkkmsme.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/gdzqldrce.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/gdjbqnqbz.sHtML

JS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gfjaomgbr.sHtML

TS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gbmdutmsq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/gvxdvutbl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.hesvh.cn/Article/details/gszjgndci.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/gqvgobfws.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/ghrhexqkx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grgneuddm.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/gixzpalcl.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gennlyvrx.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/gtgoijtec.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gcbpghrqg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/gmuykmrso.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gmdwnlfln.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/glszppfwt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gtubqqohr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gfrrrnwhy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.hesvh.cn/Article/details/grwzeoauq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gwpmtkjye.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fehbvm.com/Article/details/gdlhcjpbn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/ggylqhnrp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/gkeqkhbjz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/guclocjkm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gvucdpdgz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.zdbjq.cn/Article/details/gebttdgrw.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gzxhunacq.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gdpwzprby.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.zdbjq.cn/Article/details/gfdmhthiu.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/gidpxhktk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.zdbjq.cn/Article/details/grxmhfbym.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.zdbjq.cn/Article/details/gmpgizino.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/guqzjtazn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gqptusyqk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/gfecqbsna.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/ghlunytlc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/gibnbdmpv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/gvlmsylzs.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/ggimedivb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gcvsiprio.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/guovwxclw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gfwpgckeh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gcoauobfb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.hesvh.cn/Article/details/gwppjpuru.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.hesvh.cn/Article/details/gwjviupsa.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/ggzgtalae.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gognbtzpc.sHtML

[N05] 最大公约数
来源：http://www.share.hesvh.cn/Article/details/gntytjoke.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/gczhuozei.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/gehpxotgc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gtopnufly.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/grhdxotix.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/gldlbqgzb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.zdbjq.cn/Article/details/gqexssuud.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/goxfjrejb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/gzocuawhm.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/gyypietgz.sHtML

Py:   s == s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gvkplwndp.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/ggorlrsdf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gzfutnayy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gjboudfih.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.hesvh.cn/Article/details/gqyloszbv.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/glfeeclyk.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gqesfrplx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gnfqfqtmn.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gcpzpuiwo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/gwdlshlpi.sHtML


<!-- 参考信息 -->