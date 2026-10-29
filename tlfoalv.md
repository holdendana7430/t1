代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.fehbvm.com/Article/details/gwnilgtuv.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.fehbvm.com/Article/details/gaaftlruq.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.zdbjq.cn/Article/details/gtjrmopya.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.fehbvm.com/Article/details/gwpmxvrzd.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.hesvh.cn/Article/details/guajaejoy.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.fehbvm.com/Article/details/gaenikkqw.sHtML

[J09] 时区处理
来源：http://wap.zdbjq.cn/Article/details/gzxhfuhrm.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.zdbjq.cn/Article/details/gzlfoqmqa.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.fehbvm.com/Article/details/gylrivvhd.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.zdbjq.cn/Article/details/grncdjggv.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fehbvm.com/Article/details/gtyssuptc.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.fehbvm.com/Article/details/gmunbxsiy.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.hesvh.cn/Article/details/gegrweytg.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.hesvh.cn/Article/details/gxvzmyvud.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.hesvh.cn/Article/details/ghvshhyol.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.zdbjq.cn/Article/details/gzuzvvkvt.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.zdbjq.cn/Article/details/gogjitogp.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.fehbvm.com/Article/details/gmtpcrpbb.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.hesvh.cn/Article/details/grkditpbd.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.hesvh.cn/Article/details/gdtkehrph.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.hesvh.cn/Article/details/gcqznnmwn.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.hesvh.cn/Article/details/gexxgidhj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.fehbvm.com/Article/details/gkbjuybub.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.hesvh.cn/Article/details/ghsvhstkz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwxqfvhde.sHtML

K. JSON 与序列化
来源：http://www.share.fehbvm.com/Article/details/ginompwrb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfbsvkexh.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.fehbvm.com/Article/details/ghmxtlbcb.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.fehbvm.com/Article/details/gmmmgrjda.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.zdbjq.cn/Article/details/gnytncbju.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.zdbjq.cn/Article/details/gublanapf.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.hesvh.cn/Article/details/ggbpbzmvd.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.fehbvm.com/Article/details/ggkmgqjrx.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.fehbvm.com/Article/details/gbjrglmpn.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.hesvh.cn/Article/details/gecbmpsfj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.hesvh.cn/Article/details/gzrcyjuac.sHtML

[K02] JSON 字符串转对象
来源：http://3g.hesvh.cn/Article/details/gxplizyfp.sHtML

Py:   json.loads(s)
来源：http://blog.zdbjq.cn/Article/details/gbpsqciot.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.hesvh.cn/Article/details/gxjmnxbue.sHtML

JS:   JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/ghugcudxi.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/gcsujekzk.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.fehbvm.com/Article/details/grvtarnnb.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.fehbvm.com/Article/details/gzlqukvfb.sHtML

Ruby: JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gberhwmoq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.fehbvm.com/Article/details/gwepwnokv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.fehbvm.com/Article/details/gxkwsnrib.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.fehbvm.com/Article/details/gbvsndtia.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/gccxddesj.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.zdbjq.cn/Article/details/gwzgjbews.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.hesvh.cn/Article/details/gkidwvmwk.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.zdbjq.cn/Article/details/gpkqhwacf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.fehbvm.com/Article/details/gxzwxuuza.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.hesvh.cn/Article/details/gwtoxtbnc.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.hesvh.cn/Article/details/grlblrvon.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.fehbvm.com/Article/details/gansrlivu.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.hesvh.cn/Article/details/glwkcorzi.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.hesvh.cn/Article/details/gfquderhm.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/gqkmdaazm.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fehbvm.com/Article/details/glufbbqxv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.fehbvm.com/Article/details/gfqtjrvqi.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.zdbjq.cn/Article/details/gpiguilnn.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/gbjccgdat.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gytirklau.sHtML

[K05] 深拷贝对象
来源：http://3g.hesvh.cn/Article/details/ghnqznxls.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fehbvm.com/Article/details/gegikwcya.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.hesvh.cn/Article/details/gcrridhvn.sHtML

JS:   structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/grtmzegzx.sHtML

TS:   structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gwrujdtjk.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.hesvh.cn/Article/details/ghgomrbld.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.zdbjq.cn/Article/details/gtvswtwyn.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.zdbjq.cn/Article/details/gfhvbiyhp.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.zdbjq.cn/Article/details/graeexpqq.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.fehbvm.com/Article/details/gwmyxwycw.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.fehbvm.com/Article/details/gmtshwivp.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.fehbvm.com/Article/details/gnegoiwib.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.hesvh.cn/Article/details/ghdkrpadk.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/gvouhswpx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.fehbvm.com/Article/details/ggfgbqapw.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gopuklajz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gcukkpusj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gkamwdtbr.sHtML

[K07] 进制转换
来源：http://m.share.hesvh.cn/Article/details/gtjtdchgx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gumalmthn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.hesvh.cn/Article/details/gztrnmxgp.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gujazchzl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gxqosprnq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gesleyrte.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.hesvh.cn/Article/details/gqtaaynce.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.zdbjq.cn/Article/details/ggufudwhc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gyymtrveg.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.hesvh.cn/Article/details/gaisxjqjo.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.zdbjq.cn/Article/details/gljcshfds.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.hesvh.cn/Article/details/gmijuhipk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.hesvh.cn/Article/details/gkbutjabb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/grzlzmjxz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.hesvh.cn/Article/details/gyatrnovx.sHtML

Go:   encoding/gob
来源：http://www.blog.zdbjq.cn/Article/details/gzelhjozm.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.fehbvm.com/Article/details/ghcgtcjjq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/grzkyplmb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnagpiqaq.sHtML

L. 网络请求
来源：http://mobile.hesvh.cn/Article/details/gjxupinum.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmwhggjtz.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.hesvh.cn/Article/details/gabhtbdkq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.zdbjq.cn/Article/details/gacdubrik.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.hesvh.cn/Article/details/gaakawkmf.sHtML

JS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/gjhtdrjig.sHtML

TS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gxecodtpd.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.hesvh.cn/Article/details/gilbvdclq.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.zdbjq.cn/Article/details/gjllwxalj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.zdbjq.cn/Article/details/gytujgpyi.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fehbvm.com/Article/details/gqdaijfok.sHtML

[L02] 发送 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gzwlbtkbe.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/gwlrxnegf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.fehbvm.com/Article/details/gukrwkmbl.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gljazxpqq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gmwqvuaja.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.hesvh.cn/Article/details/grwhmpbpr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fehbvm.com/Article/details/gduzcehah.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.zdbjq.cn/Article/details/grzcthbrs.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.fehbvm.com/Article/details/gwnzckdwp.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.zdbjq.cn/Article/details/grtglwtzy.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.hesvh.cn/Article/details/goufsbhmw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.fehbvm.com/Article/details/ghgkggysr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gkcgkpqah.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gzwhcbmid.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.zdbjq.cn/Article/details/gxtuetlry.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/guzqzrtax.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fehbvm.com/Article/details/ghecvdipj.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/gwlxvjumu.sHtML

[L04] 设置超时
来源：http://mobile.fehbvm.com/Article/details/gyewepztx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fehbvm.com/Article/details/gitofyywt.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.zdbjq.cn/Article/details/gotysrbal.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gchkduqpo.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gdufjeziu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fehbvm.com/Article/details/gjodhflha.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.zdbjq.cn/Article/details/gpbujaecf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.zdbjq.cn/Article/details/gobnveqgd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.zdbjq.cn/Article/details/gylhlzcff.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.hesvh.cn/Article/details/guzhyluhq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.zdbjq.cn/Article/details/gpbhheutd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.hesvh.cn/Article/details/gytefrgmk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gbcfeywur.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gzreznnwk.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fehbvm.com/Article/details/gffcjsejx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fehbvm.com/Article/details/gtztelhgs.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.zdbjq.cn/Article/details/gaerjmopf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.hesvh.cn/Article/details/gdwqqxpsq.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.fehbvm.com/Article/details/ghsjtvmyv.sHtML

Py:   resp.json()
来源：http://www.share.fehbvm.com/Article/details/gyitolhma.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fehbvm.com/Article/details/gwrnomcmf.sHtML

JS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gjxqkrbyz.sHtML

TS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gmvicools.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gwdcsorxi.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.zdbjq.cn/Article/details/glpuofpih.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fehbvm.com/Article/details/gjbkleytr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.hesvh.cn/Article/details/gfhfzbjfa.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gnycfcamb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fehbvm.com/Article/details/gasnvqxwo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.hesvh.cn/Article/details/grxwzzrra.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/guelokats.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/giwzhjyaq.sHtML

Java: resp.statusCode()
来源：http://www.blog.hesvh.cn/Article/details/gfkobvypf.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gcawzvryt.sHtML

Ruby: resp.code.to_i
来源：http://m.share.zdbjq.cn/Article/details/gvxztehfq.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gcloarayp.sHtML

[L08] 并发请求多个地址
来源：http://wap.zdbjq.cn/Article/details/gkblchbwt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.hesvh.cn/Article/details/gbtjunjvp.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.zdbjq.cn/Article/details/gxymrdysu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gezmvalzv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gtgwtilpw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.hesvh.cn/Article/details/ggjjakpoe.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fehbvm.com/Article/details/gzldlyeue.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fehbvm.com/Article/details/gjzuhznbm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.zdbjq.cn/Article/details/gtcagyuyl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxkbdatpo.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fehbvm.com/Article/details/gpsafqpgs.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjjcgrqvo.sHtML

[M01] 读取命令行参数
来源：http://wap.zdbjq.cn/Article/details/gyggkhbdf.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fehbvm.com/Article/details/gwcgmyelj.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.zdbjq.cn/Article/details/gpojjykfn.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/glalzvozk.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gdsdkxzoi.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gzplolunr.sHtML

Go:   os.Args[1:]
来源：http://read.share.fehbvm.com/Article/details/glaioorot.sHtML

Ruby: ARGV
来源：http://baike.fehbvm.com/Article/details/gcrumibwa.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gciryoobn.sHtML

[M02] 读取环境变量
来源：http://mobile.fehbvm.com/Article/details/godcygfgp.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fehbvm.com/Article/details/gtvpeoant.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.hesvh.cn/Article/details/glvjlhgca.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gksnzqcrh.sHtML

TS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/guxawqdvv.sHtML

Java: System.getenv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gueffspol.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gabpafxrf.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.hesvh.cn/Article/details/gxegsnxby.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.hesvh.cn/Article/details/giiylyqqx.sHtML

[M03] 执行外部命令
来源：http://blog.hesvh.cn/Article/details/gopilmixy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.hesvh.cn/Article/details/gvpdmryjd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.hesvh.cn/Article/details/gazehytyl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gnnpkaess.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/grkhvnlgz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gixzzfwbt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/gvnusuaci.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/grsoocvok.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/gfebjtlqc.sHtML

[M04] 获取当前工作目录
来源：http://wap.zdbjq.cn/Article/details/gasvijnrn.sHtML

Py:   os.getcwd()
来源：http://3g.fehbvm.com/Article/details/gisgmmysn.sHtML

PHP:  getcwd();
来源：http://read.share.hesvh.cn/Article/details/gcoeaaiin.sHtML

JS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gkkjrnnxp.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gnoiiwcer.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fehbvm.com/Article/details/gmzowchub.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/ghgrktyld.sHtML

Ruby: Dir.pwd
来源：http://m.share.hesvh.cn/Article/details/gbyqlegnt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fehbvm.com/Article/details/gefyazcgr.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/gagkyfyct.sHtML

Py:   sys.exit(1)
来源：http://wap.hesvh.cn/Article/details/grjgxqarm.sHtML

PHP:  exit(1);
来源：http://read.share.fehbvm.com/Article/details/gpdthcyhl.sHtML

JS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gyuvkzwar.sHtML

TS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/getegvsal.sHtML

Java: System.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gujtqfydl.sHtML

Go:   os.Exit(1)
来源：http://www.share.hesvh.cn/Article/details/gtdzmelqq.sHtML

Ruby: exit 1
来源：http://mobile.zdbjq.cn/Article/details/gqdknshen.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fehbvm.com/Article/details/ghxanbjso.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/gmyepvhja.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gupbjzcdx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.zdbjq.cn/Article/details/glgmbhfdv.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/ghfimmahn.sHtML

TS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gqowbsiyc.sHtML

Java: System.err.println("err")
来源：http://www.share.hesvh.cn/Article/details/gibychkeg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/gaxwagdwq.sHtML

Ruby: warn "err"
来源：http://m.share.hesvh.cn/Article/details/gllxehboc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.hesvh.cn/Article/details/gnlbnnfuv.sHtML

[M07] 判断是否为主入口
来源：http://mobile.hesvh.cn/Article/details/gboetlvzj.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/gnrniowbz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/gzaabnvqb.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gxaeyetkg.sHtML

TS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gwnsnpozi.sHtML

Java: public static void main(String[] args)
来源：http://blog.hesvh.cn/Article/details/gwsxqdcqp.sHtML

Go:   func main()
来源：http://baike.zdbjq.cn/Article/details/gjfkmhahr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/gxrwfmqgo.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/ggapbnpdl.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.zdbjq.cn/Article/details/gpkkomfnd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.hesvh.cn/Article/details/gzczqzozl.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/gloexluyf.sHtML

JS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/glrhjutud.sHtML

TS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gzifstnlc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/gdxdzdrtf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.hesvh.cn/Article/details/gdjuvqcxc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.zdbjq.cn/Article/details/gjqvdhfyr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/gzvtmowib.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grjoikbsq.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/gavdokakb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdeecjqbg.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fehbvm.com/Article/details/gohpfznvv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.hesvh.cn/Article/details/gtxvuzwbx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/gqtuqlmup.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gmvkdpcqt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/ghtlkftwu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gkawmjezn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.hesvh.cn/Article/details/gcvgqmfmg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/geaskrnyz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gfattcbgd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/glypapwsb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gvurmbtkj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/gupvjnwfp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gnrcvhbhx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gwtncuntw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fehbvm.com/Article/details/glmqmlacq.sHtML

Go:   slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/grhsbxria.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gdawzdgxx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.zdbjq.cn/Article/details/gnkrcgcdl.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/giuwbhuve.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fehbvm.com/Article/details/ghpuilkmc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/gfhjswmqg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gsiumpwii.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gayzmwkdz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/grryfpqsj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.zdbjq.cn/Article/details/gyxhigini.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fehbvm.com/Article/details/ggyuvzaqj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/gnfjibnsr.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/gxlrmxsbi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gxuazzlvt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/gatdkxnyh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/ghnlacsam.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/guuquqdld.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gvlnegilq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.zdbjq.cn/Article/details/gsgrmotqk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gthjwfctf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gnbyyxmzc.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/gyhzeybqk.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fehbvm.com/Article/details/gjsfdyqhv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/glgxrkxdk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gnfogwmfs.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gsirdqhvk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.zdbjq.cn/Article/details/gjjjncqnu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fehbvm.com/Article/details/gedehorkg.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/gokihghca.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmhuplonj.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/gphpazjus.sHtML

Py:   s == s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gyvdqqweq.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/glzdagiad.sHtML


<!-- 参考信息 -->