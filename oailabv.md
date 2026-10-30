代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://baike.fehbvm.com/Article/details/gxdfcxzdi.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.fehbvm.com/Article/details/gubvesovq.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.fehbvm.com/Article/details/gwvnbfemz.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.hesvh.cn/Article/details/guqsbjfim.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.fehbvm.com/Article/details/gzxvpcmln.sHtML

[J08] 提取年月日与星期
来源：http://m.share.hesvh.cn/Article/details/gmbnbzjgf.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.hesvh.cn/Article/details/gieqlzwca.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.hesvh.cn/Article/details/gsidhhnri.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.hesvh.cn/Article/details/gclrircmh.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.zdbjq.cn/Article/details/gpddyfpfd.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.zdbjq.cn/Article/details/gusctzeng.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.hesvh.cn/Article/details/gbwvofbbl.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.zdbjq.cn/Article/details/gcihclfet.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.hesvh.cn/Article/details/ggpeexksx.sHtML

[J09] 时区处理
来源：http://wap.fehbvm.com/Article/details/gnrutbget.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.fehbvm.com/Article/details/gbspxwalz.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.fehbvm.com/Article/details/ghingphzy.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fehbvm.com/Article/details/gobzarhgp.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fehbvm.com/Article/details/gfmjnfmey.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.fehbvm.com/Article/details/gwqltnvle.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.hesvh.cn/Article/details/gxptrddoj.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.zdbjq.cn/Article/details/gbdodyosz.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.zdbjq.cn/Article/details/gxeeajgkg.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.hesvh.cn/Article/details/gfdzofwva.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.hesvh.cn/Article/details/gliuwnjqq.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.hesvh.cn/Article/details/gfyycldwe.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.hesvh.cn/Article/details/gginbwyvt.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.hesvh.cn/Article/details/gqhtijwkt.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.hesvh.cn/Article/details/garqsruko.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.zdbjq.cn/Article/details/gbbilrdaz.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.hesvh.cn/Article/details/gbsavhhrw.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.fehbvm.com/Article/details/glqzyeyog.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcnrhyssy.sHtML

K. JSON 与序列化
来源：http://blog.fehbvm.com/Article/details/gexgbwvnu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gtcqahotr.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.zdbjq.cn/Article/details/ghbknguql.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.hesvh.cn/Article/details/gkcconbtw.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/gegztazcf.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.hesvh.cn/Article/details/gkkgombqk.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.hesvh.cn/Article/details/geraxrryg.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.hesvh.cn/Article/details/gpwtmztob.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.hesvh.cn/Article/details/gmsalfipc.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.fehbvm.com/Article/details/gsjiryvhb.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.hesvh.cn/Article/details/gjpvgdksz.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.zdbjq.cn/Article/details/guvauwqlo.sHtML

Py:   json.loads(s)
来源：http://3g.zdbjq.cn/Article/details/gmneonjah.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.zdbjq.cn/Article/details/ghjugyyts.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/ghbaidvcd.sHtML

TS:   JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/ghcznfrvt.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.hesvh.cn/Article/details/gddmycbla.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/gtnimrrnv.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/goledgshg.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.fehbvm.com/Article/details/gjvdlhkwu.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.zdbjq.cn/Article/details/gnkcibrye.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.fehbvm.com/Article/details/gsbsbhruw.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.fehbvm.com/Article/details/gkhibthbt.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/gymxtghjw.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/gyenbcqfg.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.hesvh.cn/Article/details/gtiuandnz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.zdbjq.cn/Article/details/glhdaeufh.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gereykfxg.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.fehbvm.com/Article/details/ggjvaitka.sHtML

[K04] 读取 JSON 文件
来源：http://baike.fehbvm.com/Article/details/gfjqjlylq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.zdbjq.cn/Article/details/gxhwjflch.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.zdbjq.cn/Article/details/gijekkmbw.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gdkrbqdfl.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fehbvm.com/Article/details/glympyhuo.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gjtdglkrj.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/gshnotktp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.zdbjq.cn/Article/details/ghnxjgaaq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.hesvh.cn/Article/details/gsonluxjm.sHtML

[K05] 深拷贝对象
来源：http://baike.zdbjq.cn/Article/details/ghopfmgah.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fehbvm.com/Article/details/gifykkzbg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.zdbjq.cn/Article/details/gzidvkdqk.sHtML

JS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gjvpvnhgo.sHtML

TS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gezbfbzbo.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.hesvh.cn/Article/details/gjyuycmvi.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.zdbjq.cn/Article/details/gemggzhng.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.hesvh.cn/Article/details/gvqgljchz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.zdbjq.cn/Article/details/gjozwbknk.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.zdbjq.cn/Article/details/gfsajqmvg.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.hesvh.cn/Article/details/gtjuehlck.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.hesvh.cn/Article/details/gaznmvbvs.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/ghxuhmxdm.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.zdbjq.cn/Article/details/gkszhhkrq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.hesvh.cn/Article/details/gprfedgam.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gvclajesl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gmivwwgew.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/glclawghv.sHtML

[K07] 进制转换
来源：http://baike.fehbvm.com/Article/details/gabhdjqpd.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gcmqazcqx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.hesvh.cn/Article/details/gkzxerpyg.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gzqwelrve.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gcpuwtsay.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/glqtbncxy.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.fehbvm.com/Article/details/gnkwhhyht.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.hesvh.cn/Article/details/geqlxdgzo.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/ggqlzrniw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.zdbjq.cn/Article/details/givzrmxbn.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fehbvm.com/Article/details/gnvbhpxwm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.fehbvm.com/Article/details/gbgtvnnun.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/gqbwhzccu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/gmjoclvok.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.hesvh.cn/Article/details/gywxbeuti.sHtML

Go:   encoding/gob
来源：http://www.share.hesvh.cn/Article/details/gzvybvvns.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.hesvh.cn/Article/details/gifnnyjvc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gcdurahel.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkphlwigh.sHtML

L. 网络请求
来源：http://read.share.fehbvm.com/Article/details/gvcozdqsd.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvospxljs.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.hesvh.cn/Article/details/gelgecgow.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.fehbvm.com/Article/details/giprgiabg.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fehbvm.com/Article/details/garrjkvvp.sHtML

JS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/ghvocsxce.sHtML

TS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/gnoodfoqj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.fehbvm.com/Article/details/gaxyxtmza.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.zdbjq.cn/Article/details/giiilmoty.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.hesvh.cn/Article/details/gvbcsdlkt.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.zdbjq.cn/Article/details/gxcempyni.sHtML

[L02] 发送 POST JSON
来源：http://blog.fehbvm.com/Article/details/gunzbfhdg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.zdbjq.cn/Article/details/gvcpjxmli.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.zdbjq.cn/Article/details/glbhgkazz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gsiytvgod.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gzcuqansz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.zdbjq.cn/Article/details/goyivjzey.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fehbvm.com/Article/details/gndxgkhyc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.hesvh.cn/Article/details/gbbyrmygo.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.hesvh.cn/Article/details/gsexzqpzo.sHtML

[L03] 设置自定义请求头
来源：http://blog.fehbvm.com/Article/details/gtxaexkrg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.zdbjq.cn/Article/details/giveaptnp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.zdbjq.cn/Article/details/gvempacjx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/ghvfobamy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gpqdhmzhx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.fehbvm.com/Article/details/gamxwzbtd.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/gqkkgwpek.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.zdbjq.cn/Article/details/gmkgukhla.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/gapfmzbwg.sHtML

[L04] 设置超时
来源：http://www.share.fehbvm.com/Article/details/gklaneowh.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.zdbjq.cn/Article/details/gvstoaoqi.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.fehbvm.com/Article/details/gxhpshgff.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gxkmgttwg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gybigedbx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fehbvm.com/Article/details/ghtprmecy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.zdbjq.cn/Article/details/gyymiknrk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fehbvm.com/Article/details/gagxeyibq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.hesvh.cn/Article/details/giodtndyg.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.zdbjq.cn/Article/details/gelbvaqid.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.zdbjq.cn/Article/details/gfhcwfiwm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.zdbjq.cn/Article/details/gkiabuzjq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gnhotshcy.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/ghyjjewbb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.hesvh.cn/Article/details/gqwbdvhus.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.zdbjq.cn/Article/details/gqokitnft.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.hesvh.cn/Article/details/gsmikpbzz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.hesvh.cn/Article/details/gsosvjlrt.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fehbvm.com/Article/details/guljhqtet.sHtML

Py:   resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gynclmjhi.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fehbvm.com/Article/details/gwmavgyhn.sHtML

JS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gsjbffkss.sHtML

TS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/gktmlwuqs.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fehbvm.com/Article/details/glevjsbeb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.hesvh.cn/Article/details/geanefgsa.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fehbvm.com/Article/details/gdywigkaf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gargcwmhu.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gvtddacfj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fehbvm.com/Article/details/gzwveakjr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fehbvm.com/Article/details/gcczgeuzx.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gxobwbmvt.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gegzbrztp.sHtML

Java: resp.statusCode()
来源：http://m.share.zdbjq.cn/Article/details/gfwyhacfl.sHtML

Go:   resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gtmoyikko.sHtML

Ruby: resp.code.to_i
来源：http://wap.hesvh.cn/Article/details/gmhmjmhcd.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gixzmsafw.sHtML

[L08] 并发请求多个地址
来源：http://baike.hesvh.cn/Article/details/gbmtncqdb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.fehbvm.com/Article/details/gcyrzwrie.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.hesvh.cn/Article/details/gbmyyskvz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gxdzghwjk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gdmazjtsz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.zdbjq.cn/Article/details/gmoyimhkw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.zdbjq.cn/Article/details/giiihtqok.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gqhxpqiir.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gjzycbmwc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfhiswphu.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.hesvh.cn/Article/details/gkafwwoqg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gerqxgcml.sHtML

[M01] 读取命令行参数
来源：http://www.share.hesvh.cn/Article/details/gmzparxjk.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fehbvm.com/Article/details/gslvozfvk.sHtML

PHP:  $argv;  $argc;
来源：http://3g.zdbjq.cn/Article/details/gayhxropb.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gxcxckprt.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gutmspkcj.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gnblurgzc.sHtML

Go:   os.Args[1:]
来源：http://blog.hesvh.cn/Article/details/gatqxlvtd.sHtML

Ruby: ARGV
来源：http://mobile.fehbvm.com/Article/details/gbyiphuzl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gaebcjqaw.sHtML

[M02] 读取环境变量
来源：http://baike.fehbvm.com/Article/details/gjovdrtut.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gnxrrmvcp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/ggbgvbzaj.sHtML

JS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gqpcwqudz.sHtML

TS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gbcwrnejw.sHtML

Java: System.getenv("HOME")
来源：http://read.share.hesvh.cn/Article/details/glnrzyjtx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/ggnhcboey.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/gsgtapazu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.hesvh.cn/Article/details/gdadnppxa.sHtML

[M03] 执行外部命令
来源：http://www.blog.zdbjq.cn/Article/details/gubsqnqbq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.hesvh.cn/Article/details/gaxipfsfv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.hesvh.cn/Article/details/ggtiaqrjh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gcjftpftv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gkldkxltt.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fehbvm.com/Article/details/glekcvrsr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/ggwvtxatj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fehbvm.com/Article/details/gzpwurqmv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.zdbjq.cn/Article/details/goladobgu.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/geakdnxdv.sHtML

Py:   os.getcwd()
来源：http://www.share.fehbvm.com/Article/details/gonocffjh.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/gsfpacjwb.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/ggfdlywbv.sHtML

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gusceardm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.hesvh.cn/Article/details/gpxdhotji.sHtML

Go:   os.Getwd()
来源：http://www.share.hesvh.cn/Article/details/ghpquumrn.sHtML

Ruby: Dir.pwd
来源：http://blog.hesvh.cn/Article/details/ghvqadoob.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/gjqjwgvhn.sHtML

[M05] 设置退出码
来源：http://3g.zdbjq.cn/Article/details/goljynurb.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gfbmutzbl.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/gdesvmppi.sHtML

JS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gafayjzjl.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/ggwevuqkv.sHtML

Java: System.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gieayvmra.sHtML

Go:   os.Exit(1)
来源：http://baike.fehbvm.com/Article/details/gxzhddqjs.sHtML

Ruby: exit 1
来源：http://3g.zdbjq.cn/Article/details/gjybzlgba.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fehbvm.com/Article/details/gboyobemb.sHtML

[M06] 向标准错误输出
来源：http://m.share.hesvh.cn/Article/details/gxnjfckbe.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gozdtimxi.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/gnhkcronb.sHtML

JS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gbwjwzyaa.sHtML

TS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gwridbbbq.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/gxzworlif.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fehbvm.com/Article/details/gfocodqjx.sHtML

Ruby: warn "err"
来源：http://blog.zdbjq.cn/Article/details/gmumoqnzw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.hesvh.cn/Article/details/grpacqnnz.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.hesvh.cn/Article/details/gusjbjrgh.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fehbvm.com/Article/details/gglubwyhs.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/gguxlkaft.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gqvirunud.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gojoakdlv.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fehbvm.com/Article/details/gnejexxgp.sHtML

Go:   func main()
来源：http://www.blog.zdbjq.cn/Article/details/gritlcyba.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/ghvdrebsk.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/galrjhpig.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.zdbjq.cn/Article/details/gctxmtzgx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.hesvh.cn/Article/details/gesgyuxpw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/gwaxgeltr.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gjulsujcy.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gfewahfvk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.zdbjq.cn/Article/details/gijdblkxk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/gnjmtlmim.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/gylvzxpzl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.hesvh.cn/Article/details/gvklqvpfk.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gahzcewqw.sHtML

N. 数据结构与算法
来源：http://m.share.hesvh.cn/Article/details/gepnrziwf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtbarzzmk.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/geckpujtp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gglpubvmo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.zdbjq.cn/Article/details/gogvqdzpy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gdoblcqrp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gzosynopc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gfqkkstgp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/glduscqyc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.zdbjq.cn/Article/details/gghjcomch.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gxsnpquwo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.zdbjq.cn/Article/details/ghvzstszo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gofjzzkis.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fehbvm.com/Article/details/gezwhjdqg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gtofxqigc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/ggyvfpzhh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.zdbjq.cn/Article/details/gimjvwezp.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gljcttmzv.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gwbxlsata.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/gcjbrgjbb.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.hesvh.cn/Article/details/gwvvrfsim.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.zdbjq.cn/Article/details/gzcsakkku.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.hesvh.cn/Article/details/gwvhuddmo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gjjtjyrul.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/giejisfzc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/gvzhrrhku.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/gtkfmrgkk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/gngkepkxj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.hesvh.cn/Article/details/gevferdhp.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gkivqbdou.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gcozbetmz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fehbvm.com/Article/details/gfrsvkeba.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/ggmwwminr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gkchqjduj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/glvwoqsso.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.zdbjq.cn/Article/details/grkqhtmmh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gqufbysoj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gpsgkyoul.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/gkyuomggw.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gxajrypwm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/gpqabchpx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gmpvzyuim.sHtML


<!-- 参考信息 -->