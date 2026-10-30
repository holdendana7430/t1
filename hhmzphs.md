代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.hesvh.cn/Article/details/gljtotnba.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.zdbjq.cn/Article/details/gqkjplogg.sHtML

[J09] 时区处理
来源：http://www.blog.hesvh.cn/Article/details/gcrpgsvqq.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.fehbvm.com/Article/details/gaustyghc.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.fehbvm.com/Article/details/gucihsgxz.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.zdbjq.cn/Article/details/gqtvllrco.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fehbvm.com/Article/details/gdwfvazlv.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.fehbvm.com/Article/details/gcvskepwj.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.zdbjq.cn/Article/details/gjfqsookx.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.fehbvm.com/Article/details/glokjzexy.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.zdbjq.cn/Article/details/gozehxgrk.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.fehbvm.com/Article/details/gqukmxsnp.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.zdbjq.cn/Article/details/gliwlgwkm.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.zdbjq.cn/Article/details/grhsrdack.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.hesvh.cn/Article/details/gfstpytub.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.zdbjq.cn/Article/details/gekzropqj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.fehbvm.com/Article/details/gfsegyefi.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.fehbvm.com/Article/details/gfznqynzk.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.zdbjq.cn/Article/details/gulzdjhge.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.hesvh.cn/Article/details/gulytcaue.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvcctfkzx.sHtML

K. JSON 与序列化
来源：http://blog.fehbvm.com/Article/details/gqdcytkmv.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnafbbfqv.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.fehbvm.com/Article/details/gswvctkvk.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.zdbjq.cn/Article/details/gibiuvloa.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.fehbvm.com/Article/details/gvgzqixls.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.zdbjq.cn/Article/details/gqtdnbkdl.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.zdbjq.cn/Article/details/gixabzaqn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.zdbjq.cn/Article/details/gfegwpdbu.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gygmkudex.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.hesvh.cn/Article/details/ghinfahke.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.hesvh.cn/Article/details/gmaxcrhvv.sHtML

[K02] JSON 字符串转对象
来源：http://blog.zdbjq.cn/Article/details/gfjwlfrsy.sHtML

Py:   json.loads(s)
来源：http://mobile.zdbjq.cn/Article/details/gsqbtgyub.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.hesvh.cn/Article/details/gphorrclk.sHtML

JS:   JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gbrmlsnvk.sHtML

TS:   JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gwbuflrxx.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gimdrxqnw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.hesvh.cn/Article/details/grtojnaxv.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ggxbyxgrv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.zdbjq.cn/Article/details/gqjdygwyx.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.hesvh.cn/Article/details/gbrfmekha.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.fehbvm.com/Article/details/gemqghghx.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.hesvh.cn/Article/details/ggvnyixix.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.hesvh.cn/Article/details/gvhgymqgy.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/gdyecfdzg.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.zdbjq.cn/Article/details/giphzfojo.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.hesvh.cn/Article/details/giyphnrlj.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/glzvwfnca.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.hesvh.cn/Article/details/gepxjzphu.sHtML

[K04] 读取 JSON 文件
来源：http://3g.fehbvm.com/Article/details/gmpvjbefw.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.zdbjq.cn/Article/details/goayszwxn.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.fehbvm.com/Article/details/ggazqzadp.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/gbclpjwvo.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gsgabxadl.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/ghnqufqgg.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/gmqqkdhxu.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.zdbjq.cn/Article/details/gwaahtdmp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.zdbjq.cn/Article/details/gmtosvgqr.sHtML

[K05] 深拷贝对象
来源：http://read.share.hesvh.cn/Article/details/gjsmimezz.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.zdbjq.cn/Article/details/giacrjhje.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.hesvh.cn/Article/details/ghvdjzmii.sHtML

JS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gveojstxu.sHtML

TS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gjlxjejgo.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.fehbvm.com/Article/details/gxjabcvyz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.hesvh.cn/Article/details/gsvbrxush.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.hesvh.cn/Article/details/ggonlwgjd.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.fehbvm.com/Article/details/gqhmippgh.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.zdbjq.cn/Article/details/gbrtayghw.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gsphumuwb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.hesvh.cn/Article/details/ggyzsbstc.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.hesvh.cn/Article/details/gobfvxizl.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/gzdgbccot.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.fehbvm.com/Article/details/gyzkehmsg.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/grdhlkgwk.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/geebsfnrh.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gjkcfvifz.sHtML

[K07] 进制转换
来源：http://www.share.hesvh.cn/Article/details/gwvedryas.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gmhsjhmxn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.fehbvm.com/Article/details/gelqhqjzu.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/ggxmxrtmy.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/guetdxmux.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gknkftcqx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.hesvh.cn/Article/details/gzlxopqqq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.hesvh.cn/Article/details/goebdldte.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gyxzbrmrj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.zdbjq.cn/Article/details/gdgodepcz.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.zdbjq.cn/Article/details/gemzexqnw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.fehbvm.com/Article/details/ghdfhkvdb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gcuiknmvb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/grusuwdwo.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.fehbvm.com/Article/details/gyvffffwi.sHtML

Go:   encoding/gob
来源：http://blog.fehbvm.com/Article/details/gfritmlfu.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.hesvh.cn/Article/details/gmxfueogt.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/grdmwlxxb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gyfdwfjqq.sHtML

L. 网络请求
来源：http://www.share.fehbvm.com/Article/details/gsenmqkgi.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/galjniaek.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.fehbvm.com/Article/details/gwmcjutoy.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.zdbjq.cn/Article/details/girffcelu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.fehbvm.com/Article/details/gvnmpdiyh.sHtML

JS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gkbhgpdnu.sHtML

TS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/glhpmipic.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.fehbvm.com/Article/details/garkuysla.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gufmrsjkt.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.zdbjq.cn/Article/details/gtjzubolc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fehbvm.com/Article/details/gnufohpbr.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gewyxopnf.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.hesvh.cn/Article/details/gdvqhgxib.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.fehbvm.com/Article/details/gltscbwaf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/ggjybuuin.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/guzsxoamk.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.hesvh.cn/Article/details/gxcrrvcgz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.hesvh.cn/Article/details/grhmouwdg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.zdbjq.cn/Article/details/guetxokep.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.zdbjq.cn/Article/details/gqunenhsy.sHtML

[L03] 设置自定义请求头
来源：http://baike.hesvh.cn/Article/details/gytoymtls.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.hesvh.cn/Article/details/gitthntdf.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fehbvm.com/Article/details/ggetlecny.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gpiivxgla.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gvhanqxrf.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.hesvh.cn/Article/details/gscnxcloq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gdxcwuksn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.fehbvm.com/Article/details/gqfmiaowj.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gasoskoro.sHtML

[L04] 设置超时
来源：http://www.share.zdbjq.cn/Article/details/gynbgleuo.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.hesvh.cn/Article/details/gvatcmjny.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.hesvh.cn/Article/details/ghetjiokw.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/gcvtiziwx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gcfcpzvis.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fehbvm.com/Article/details/gwoplqfdc.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.zdbjq.cn/Article/details/gsxrllyth.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.hesvh.cn/Article/details/gonfbqewt.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.zdbjq.cn/Article/details/gprsifdei.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.hesvh.cn/Article/details/grzuppjhv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.zdbjq.cn/Article/details/gzljalope.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fehbvm.com/Article/details/gjfxeewnp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gjfpzjhaq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gewakkcja.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fehbvm.com/Article/details/glpkmswla.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.zdbjq.cn/Article/details/gwuhuwegw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.zdbjq.cn/Article/details/garwwtbvn.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gvpfaozxe.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.hesvh.cn/Article/details/gxmehxvsd.sHtML

Py:   resp.json()
来源：http://m.share.hesvh.cn/Article/details/gcyvvoqir.sHtML

PHP:  json_decode($body, true);
来源：http://baike.hesvh.cn/Article/details/gtvamsjph.sHtML

JS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gwsbygawg.sHtML

TS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/grgofcmze.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gqarrtyog.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.hesvh.cn/Article/details/gijfpuvig.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.hesvh.cn/Article/details/gnwjmisbg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.hesvh.cn/Article/details/gfiuregeo.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gulvsiyfs.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fehbvm.com/Article/details/gdlnrspcv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.hesvh.cn/Article/details/gqsjzdext.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gswymxpkk.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gnrmeovvf.sHtML

Java: resp.statusCode()
来源：http://baike.fehbvm.com/Article/details/gnzeaiiyq.sHtML

Go:   resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gmffchwsq.sHtML

Ruby: resp.code.to_i
来源：http://blog.fehbvm.com/Article/details/ghuxfwmps.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gysmsucaw.sHtML

[L08] 并发请求多个地址
来源：http://baike.zdbjq.cn/Article/details/gplgepoww.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.hesvh.cn/Article/details/gvrkbhfcq.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fehbvm.com/Article/details/ggchekfgi.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gpdjootev.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gmzyctuon.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fehbvm.com/Article/details/gpzqxyjhb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/ggpcvoajh.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gvxbpfhqq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.hesvh.cn/Article/details/gfgauirvq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzkvhhxho.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fehbvm.com/Article/details/gtivbccmc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqsyiyjvn.sHtML

[M01] 读取命令行参数
来源：http://wap.fehbvm.com/Article/details/gqeuqzxca.sHtML

Py:   sys.argv[1:]
来源：http://blog.zdbjq.cn/Article/details/gajuuhflw.sHtML

PHP:  $argv;  $argc;
来源：http://blog.hesvh.cn/Article/details/gvbosvrwl.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/ghilhiouw.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/giwjcnoah.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gyxpnyexz.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.hesvh.cn/Article/details/guwvxmnsq.sHtML

Ruby: ARGV
来源：http://blog.zdbjq.cn/Article/details/gfuxsejkq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gqvvgzcdg.sHtML

[M02] 读取环境变量
来源：http://wap.zdbjq.cn/Article/details/gfcojzrfl.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gfkzrqsgz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gyvbozmte.sHtML

JS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gcprniojg.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gcdcvnynb.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/glqseyzxw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gcmuymdmt.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.hesvh.cn/Article/details/gcbgriuye.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/gpfuyavsg.sHtML

[M03] 执行外部命令
来源：http://mobile.fehbvm.com/Article/details/gzhfjkkje.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/gfxeaehtf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.hesvh.cn/Article/details/gzypqnrrq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gtblolqpn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/grlejfbgo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.zdbjq.cn/Article/details/gctvuamff.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/gzxogafur.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fehbvm.com/Article/details/gtomtigmp.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/ggniolrpk.sHtML

[M04] 获取当前工作目录
来源：http://www.share.hesvh.cn/Article/details/gczbtbsyv.sHtML

Py:   os.getcwd()
来源：http://www.blog.fehbvm.com/Article/details/gebjacoyi.sHtML

PHP:  getcwd();
来源：http://blog.fehbvm.com/Article/details/gpgycilfh.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gbmtgvvrj.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gcumkyfzt.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/gjvlnntch.sHtML

Go:   os.Getwd()
来源：http://3g.fehbvm.com/Article/details/gfaykrutw.sHtML

Ruby: Dir.pwd
来源：http://baike.zdbjq.cn/Article/details/giuaootok.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/geknvigwm.sHtML

[M05] 设置退出码
来源：http://3g.fehbvm.com/Article/details/gidpsnycg.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gjgsbdqeh.sHtML

PHP:  exit(1);
来源：http://read.share.fehbvm.com/Article/details/gloxsczul.sHtML

JS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/grmoluaft.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gjrkefrbp.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/ggiywfvul.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/gppsbwuxj.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/gsymnkzus.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/grrfximlg.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/gtrnrtait.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gtyvenuvn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/grlqwddie.sHtML

JS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gpvtokhrq.sHtML

TS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gqiuokqjc.sHtML

Java: System.err.println("err")
来源：http://3g.fehbvm.com/Article/details/gvtzdxxqz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/ggwnrdjxc.sHtML

Ruby: warn "err"
来源：http://www.share.hesvh.cn/Article/details/gznoakgtc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gnqksvvit.sHtML

[M07] 判断是否为主入口
来源：http://m.share.zdbjq.cn/Article/details/gzqhnbhsm.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/gcbcyoqpr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.zdbjq.cn/Article/details/gmpwahiqg.sHtML

JS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gmeuapztc.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gbyoamrsz.sHtML

Java: public static void main(String[] args)
来源：http://wap.fehbvm.com/Article/details/ggcdtkvdd.sHtML

Go:   func main()
来源：http://www.blog.hesvh.cn/Article/details/gdvsgmjac.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/gimqrvhyd.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.hesvh.cn/Article/details/ghyhuqvrt.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fehbvm.com/Article/details/gbrqiealn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/gtzhqmecj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/ghnudyepk.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gvyawzzgw.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gaxvqnghr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.zdbjq.cn/Article/details/gukkjpgic.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/gelanabqv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.zdbjq.cn/Article/details/gqlasjyhy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/gqgzcsmcd.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gtfofxfbx.sHtML

N. 数据结构与算法
来源：http://www.blog.hesvh.cn/Article/details/gndvgeale.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqysvzcla.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.hesvh.cn/Article/details/gofnudzls.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gjrkywmpw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gycmxglvj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gnxgaxusx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gxkwwhmfy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gkiucfxuu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/grooeyfna.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.zdbjq.cn/Article/details/gflpqpqcn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gmjrbllbj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.zdbjq.cn/Article/details/gdlbdspus.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gtshpllit.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/glwjnqcvp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gjjuojdwx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gzkqvuryd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.hesvh.cn/Article/details/ghorkouzp.sHtML

Go:   slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gmfjaxtcj.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gjbexjvwi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.hesvh.cn/Article/details/gezunmikq.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/gebkhccrt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/gmkijikbi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/ghrfbpikl.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gbjcnbtbj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gtwifgtdc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/gdstupama.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/gzwlkdsvj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.zdbjq.cn/Article/details/gjpbwfxbp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fehbvm.com/Article/details/gcybxrroc.sHtML

[N04] 斐波那契数列
来源：http://mobile.fehbvm.com/Article/details/gwyyibyzn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gmvqqefmo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.hesvh.cn/Article/details/gfbeyhkqw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gggdtqjqt.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gedlzolah.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.hesvh.cn/Article/details/ggwfqavhr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/gzsijqxja.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gxshztabe.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/getyuxkec.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/gzswrfcsl.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/givbomtit.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.zdbjq.cn/Article/details/gdexkeqhh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gcqwraqse.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gkneqnzlf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.hesvh.cn/Article/details/gecmxdlie.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.hesvh.cn/Article/details/gsypfvphi.sHtML

Ruby: a.gcd(b)
来源：http://wap.fehbvm.com/Article/details/gjpdwnprx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.hesvh.cn/Article/details/gbxwsqxsk.sHtML

[N06] 判断回文字符串
来源：http://m.share.hesvh.cn/Article/details/ghuefeous.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gcahrsrow.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gdlklcole.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gerohogsr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gqkacbczj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fehbvm.com/Article/details/guakpwqji.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/geljfwvqk.sHtML


<!-- 参考信息 -->