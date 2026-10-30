代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.hesvh.cn/Article/details/gjmgqvria.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.hesvh.cn/Article/details/gacetrymp.sHtML

[J09] 时区处理
来源：http://www.blog.zdbjq.cn/Article/details/gzucjbrih.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.fehbvm.com/Article/details/gkvswfuac.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.zdbjq.cn/Article/details/gvsdxsggr.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.zdbjq.cn/Article/details/gakfcbgaz.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.hesvh.cn/Article/details/geulsnjho.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.zdbjq.cn/Article/details/ganrzlsyv.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.fehbvm.com/Article/details/glknzxnob.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.fehbvm.com/Article/details/gkzdsagdi.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.fehbvm.com/Article/details/ghurbnnqe.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.zdbjq.cn/Article/details/gdoranmda.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.fehbvm.com/Article/details/gskwuhidr.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.zdbjq.cn/Article/details/gowlzgtpc.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.hesvh.cn/Article/details/ghmewugah.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.fehbvm.com/Article/details/ggnxxhjda.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.fehbvm.com/Article/details/gxgyyxzqf.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.hesvh.cn/Article/details/gjpptlanc.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.zdbjq.cn/Article/details/gqqscrkwf.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.fehbvm.com/Article/details/gtillmbze.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmbeoddru.sHtML

K. JSON 与序列化
来源：http://www.share.fehbvm.com/Article/details/gyrfvqevi.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjzqbzkdb.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.hesvh.cn/Article/details/gxkrfxjdd.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.fehbvm.com/Article/details/gvnwkagib.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.hesvh.cn/Article/details/gbdbjhnll.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.hesvh.cn/Article/details/gbqgfhrnh.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.hesvh.cn/Article/details/gcbbsqkfq.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.hesvh.cn/Article/details/gcxtcrbmw.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.hesvh.cn/Article/details/gwvksreqc.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.hesvh.cn/Article/details/gcnuwkgwr.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.zdbjq.cn/Article/details/glgmjwcgu.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.fehbvm.com/Article/details/gvoxnviyx.sHtML

Py:   json.loads(s)
来源：http://read.share.fehbvm.com/Article/details/gifppkrou.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.zdbjq.cn/Article/details/gorjujxfm.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/gfsfmsqmo.sHtML

TS:   JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gzwsgntmu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gppazdwfo.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/gcjglzpxa.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gxrbmezer.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.zdbjq.cn/Article/details/gzyxmxmxp.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.zdbjq.cn/Article/details/gvyqzejvt.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.fehbvm.com/Article/details/gpccyuvip.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.hesvh.cn/Article/details/gocvdvpdw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fehbvm.com/Article/details/gzycpnreb.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.hesvh.cn/Article/details/gxeggsgjl.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.zdbjq.cn/Article/details/gvwrcvolb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.zdbjq.cn/Article/details/ghszanddw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.hesvh.cn/Article/details/gowndzlhv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.zdbjq.cn/Article/details/gludgbcys.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.hesvh.cn/Article/details/gxcwbzhut.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gaszaaydc.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.zdbjq.cn/Article/details/gawvqlloc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/gwcyrongl.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.zdbjq.cn/Article/details/gffllbzzc.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.fehbvm.com/Article/details/gqrjyynyy.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/gsqffdwxu.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.hesvh.cn/Article/details/ghwzekpea.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/ggdzisviu.sHtML

[K05] 深拷贝对象
来源：http://www.share.zdbjq.cn/Article/details/gmnagjokz.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.zdbjq.cn/Article/details/guaompkqq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.fehbvm.com/Article/details/gtdevdipt.sHtML

JS:   structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/gyxodzjui.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gmtpmulmo.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.zdbjq.cn/Article/details/gtmeerwxd.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.zdbjq.cn/Article/details/geewxeuhm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fehbvm.com/Article/details/gncgucqyh.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.fehbvm.com/Article/details/ghmeqymox.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.fehbvm.com/Article/details/gnmbzpdmv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gfovxzqvm.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.fehbvm.com/Article/details/gmxgbbdjo.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.hesvh.cn/Article/details/ggjmtziqb.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/grgeftwnz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.hesvh.cn/Article/details/goqxdrigh.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gqiqsreay.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gxuwahjrk.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gxokmdxdc.sHtML

[K07] 进制转换
来源：http://read.share.fehbvm.com/Article/details/gjitbdyny.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gzvuqxmup.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.fehbvm.com/Article/details/glmzmuhnw.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gvsbfaofw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gonftubts.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/ghclqvbtl.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.zdbjq.cn/Article/details/gmjwyujus.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.fehbvm.com/Article/details/gxgtebhtg.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gwdhdsvju.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.zdbjq.cn/Article/details/gushoiwkq.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.zdbjq.cn/Article/details/gqaovjewo.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.zdbjq.cn/Article/details/gxthywtvn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/gkxjykilq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/gzbpffcdr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.fehbvm.com/Article/details/gqwwkhlxr.sHtML

Go:   encoding/gob
来源：http://3g.fehbvm.com/Article/details/ggsuufqer.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.zdbjq.cn/Article/details/gcaouiqui.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/gqayyhajs.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gclgokphm.sHtML

L. 网络请求
来源：http://read.share.fehbvm.com/Article/details/gqxgjtevl.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gridvfyjd.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.zdbjq.cn/Article/details/gqwxkqxcf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.fehbvm.com/Article/details/gxfmqyxjt.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.zdbjq.cn/Article/details/garguvwrv.sHtML

JS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/gulyckepj.sHtML

TS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gffyootwb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fehbvm.com/Article/details/gmcymhrhf.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.fehbvm.com/Article/details/gjuffqhbr.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.zdbjq.cn/Article/details/gzgcvhuuu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fehbvm.com/Article/details/gtzxuqqaq.sHtML

[L02] 发送 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/glszhhbyg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/gyufwlbpm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.zdbjq.cn/Article/details/gpuvspdii.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gfxotfarg.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gkmkgpets.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.hesvh.cn/Article/details/gmaexdbkh.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.hesvh.cn/Article/details/gpxgtwhcf.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.zdbjq.cn/Article/details/ghsjmelnf.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.hesvh.cn/Article/details/gyjgtcxie.sHtML

[L03] 设置自定义请求头
来源：http://mobile.hesvh.cn/Article/details/gcolzzzlq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.zdbjq.cn/Article/details/giabandjp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.zdbjq.cn/Article/details/gvkpcdmpg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gtxbzaisr.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gkihygsgm.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.hesvh.cn/Article/details/gcglryugm.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gxhocaswt.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.hesvh.cn/Article/details/gyyduddcb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gfpwwsyky.sHtML

[L04] 设置超时
来源：http://blog.fehbvm.com/Article/details/ghssibjti.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fehbvm.com/Article/details/gstudltfq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gigctkbuq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.hesvh.cn/Article/details/gqlymcvsp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gvoqycfkz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.hesvh.cn/Article/details/gqwnudtol.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.zdbjq.cn/Article/details/grfhrfsjg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.hesvh.cn/Article/details/gisreunik.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.zdbjq.cn/Article/details/gdfwyjpge.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.fehbvm.com/Article/details/gyhwdsxfm.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fehbvm.com/Article/details/gycckqgrm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.hesvh.cn/Article/details/gapudnnzz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/gkvwaasiz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gyerypmlp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.hesvh.cn/Article/details/gwamcwbci.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.hesvh.cn/Article/details/gybuqgoxp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fehbvm.com/Article/details/gndsbpyro.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fehbvm.com/Article/details/gfjmuxegs.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gbmgpgevr.sHtML

Py:   resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gzyrszdhx.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.zdbjq.cn/Article/details/gkqcrhymh.sHtML

JS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/goomqyjjv.sHtML

TS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/glmbrvrfx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.zdbjq.cn/Article/details/grfetbwoh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.zdbjq.cn/Article/details/gzsuzmkaj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.zdbjq.cn/Article/details/gqacttxes.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fehbvm.com/Article/details/ghxqhvphu.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gzzfmpkci.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.hesvh.cn/Article/details/gmaoqwjvc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fehbvm.com/Article/details/guzjkayfl.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gxbfqdrrt.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gksuzbimu.sHtML

Java: resp.statusCode()
来源：http://www.blog.fehbvm.com/Article/details/gahumvksg.sHtML

Go:   resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gronodcxp.sHtML

Ruby: resp.code.to_i
来源：http://blog.hesvh.cn/Article/details/gzayrgcvw.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gvycghrjd.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.hesvh.cn/Article/details/gkrkgazdj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fehbvm.com/Article/details/gugcalicw.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.hesvh.cn/Article/details/glzcqratm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gqlqtxuwl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gilavyvou.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.zdbjq.cn/Article/details/gtkurhqqi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.hesvh.cn/Article/details/gieaapjbq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fehbvm.com/Article/details/gmbalrahc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.hesvh.cn/Article/details/gdlqlhqdv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpzbbaoyy.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.hesvh.cn/Article/details/gnsfnqcrg.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gsybjesiv.sHtML

[M01] 读取命令行参数
来源：http://read.share.fehbvm.com/Article/details/gahmbyjmo.sHtML

Py:   sys.argv[1:]
来源：http://3g.hesvh.cn/Article/details/gdwdsmgbf.sHtML

PHP:  $argv;  $argc;
来源：http://baike.hesvh.cn/Article/details/gxgzptrop.sHtML

JS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gbtupdpyg.sHtML

TS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/geojnoplo.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/ggecoiyfz.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/gebehabvm.sHtML

Ruby: ARGV
来源：http://www.blog.hesvh.cn/Article/details/gyhtfjcit.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gfqtvjkcb.sHtML

[M02] 读取环境变量
来源：http://wap.zdbjq.cn/Article/details/gmvrqtacr.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gytlfgujm.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gxthlyrrk.sHtML

JS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gtyqlttot.sHtML

TS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gsvexbeed.sHtML

Java: System.getenv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gvugqrqxj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gdtkjankn.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fehbvm.com/Article/details/giwwyplmy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gtgioqcfl.sHtML

[M03] 执行外部命令
来源：http://www.blog.hesvh.cn/Article/details/gcmkndpmo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/guzovebvd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.hesvh.cn/Article/details/gbcvdgqwy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gtuhfbtsh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gqqhsxnry.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/gitfaimik.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fehbvm.com/Article/details/gqiroxlez.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.zdbjq.cn/Article/details/gkfymjlbf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fehbvm.com/Article/details/gflvwcswy.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fehbvm.com/Article/details/gjgdvlfsy.sHtML

Py:   os.getcwd()
来源：http://mobile.zdbjq.cn/Article/details/grqjrvkjw.sHtML

PHP:  getcwd();
来源：http://mobile.fehbvm.com/Article/details/gtsvzawlw.sHtML

JS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gsevkhadx.sHtML

TS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gyxmmgmne.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.hesvh.cn/Article/details/gkwkswmgx.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fehbvm.com/Article/details/ggufcrxyz.sHtML

Ruby: Dir.pwd
来源：http://wap.fehbvm.com/Article/details/gnsjxmyev.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.hesvh.cn/Article/details/gmdessmep.sHtML

[M05] 设置退出码
来源：http://www.blog.fehbvm.com/Article/details/grmgbtyuv.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gbuumdbyf.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/gmjbrkqeg.sHtML

JS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gwdufxfty.sHtML

TS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gxqskxnln.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gmsnzytfr.sHtML

Go:   os.Exit(1)
来源：http://www.share.hesvh.cn/Article/details/gkaazuqpr.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/gyoatfeam.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fehbvm.com/Article/details/gomovxnol.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/gpjtixmbv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/grktvnhac.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/gsgnjpjzg.sHtML

JS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gdmypridr.sHtML

TS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/guzuktike.sHtML

Java: System.err.println("err")
来源：http://wap.fehbvm.com/Article/details/gbanyzttg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.zdbjq.cn/Article/details/ghjmumavz.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/gixdgdawf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.zdbjq.cn/Article/details/gxuwgzvxf.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/gkuyxjleq.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/gozctaijh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/gzknezupf.sHtML

JS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gmgheoonq.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/ggeowfome.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/gxyzsjcgs.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/gdmknansu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/gerkzygwl.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fehbvm.com/Article/details/gntvnbcdv.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gyreuwufq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fehbvm.com/Article/details/glerchcev.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.hesvh.cn/Article/details/gillnhfgj.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gkyfxibcs.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gdlesztph.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/grmnmhorc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gofuumpdi.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fehbvm.com/Article/details/glsfxzrkb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.hesvh.cn/Article/details/guamzsxfp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjckapdzk.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/ghvyjmqiq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjkhhmguw.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/gyzflvrhd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.hesvh.cn/Article/details/guvearzwa.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/gmrhijxco.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gzueomtse.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gvajdilof.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/giwjrlsea.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/ggscudmsp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/giedkudhl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gxtwvxyuz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fehbvm.com/Article/details/gishdzdmy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gtxobxaxt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fehbvm.com/Article/details/gxupodmpd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gjputjurr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gepybksxh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/gwyupnnao.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/ghcewodhh.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gqpbafsvn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fehbvm.com/Article/details/gfvywmyqn.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.zdbjq.cn/Article/details/gdjjqblzw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.hesvh.cn/Article/details/ggmxazoxk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.hesvh.cn/Article/details/glmfkxyri.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gbtzptunv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gpvlxxiyl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/gnliugwbd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gynntknqe.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fehbvm.com/Article/details/gphqbctdj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/gqxtsywdj.sHtML

[N04] 斐波那契数列
来源：http://read.share.hesvh.cn/Article/details/gwhybxykd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gvunoafvg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fehbvm.com/Article/details/gxxwaneis.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gbhxuyiic.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gdyncclbn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/guraaitsm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.zdbjq.cn/Article/details/gnlldfbiu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gqlvdpomb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gbhosozrs.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/gblusutef.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fehbvm.com/Article/details/glzfgytav.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.zdbjq.cn/Article/details/guailgais.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gtrdcifej.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gbgaquozn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fehbvm.com/Article/details/grzwgbist.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/gnagufwnq.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/ghlhpuneb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/guznxzkqg.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/grxjmmnet.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/gwttrjnwn.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gwnfkptut.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gtwlugoam.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gdemzdxjx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/gmpigomxv.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.zdbjq.cn/Article/details/goznczbba.sHtML


<!-- 参考信息 -->