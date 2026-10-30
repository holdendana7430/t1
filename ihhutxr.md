代发 wailian999

Py:   (end - start).total_seconds()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpabnfgu.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwhwxebu.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvitnqgt.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhepmcwl.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpenhlyk.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.fanxiaobao.xyz/Article/details/guykiireb.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbecdtbu.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.fanxiaobao.xyz/Article/details/gnomvfxdi.sHtML

[J07] 比较两个日期
来源：http://3g.fanxiaobao.xyz/Article/details/ggnisoaun.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtszhmzq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.fanxiaobao.xyz/Article/details/gpvvbeobl.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.fanxiaobao.xyz/Article/details/gjgtckxnj.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.fanxiaobao.xyz/Article/details/ghoewydla.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswfnhqbq.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.fanxiaobao.xyz/Article/details/glpkennow.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.fanxiaobao.xyz/Article/details/gunqykfbg.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.fanxiaobao.xyz/Article/details/gpnfalryi.sHtML

[J08] 提取年月日与星期
来源：http://blog.fanxiaobao.xyz/Article/details/gsmfxchoi.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.fanxiaobao.xyz/Article/details/gruxpkvuy.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.fanxiaobao.xyz/Article/details/glfbngyly.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.fanxiaobao.xyz/Article/details/geglkszgi.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.fanxiaobao.xyz/Article/details/gljpjtvls.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.fanxiaobao.xyz/Article/details/gyxayqaij.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpbyagza.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.fanxiaobao.xyz/Article/details/gspeeizlb.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmqximcp.sHtML

[J09] 时区处理
来源：http://blog.fanxiaobao.xyz/Article/details/gpfrkopqn.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.fanxiaobao.xyz/Article/details/grttafceb.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.fanxiaobao.xyz/Article/details/goxhoaltr.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fanxiaobao.xyz/Article/details/gwrxofhrd.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqgywica.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.fanxiaobao.xyz/Article/details/gwklcgkeh.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.fanxiaobao.xyz/Article/details/gwamjrltx.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.fanxiaobao.xyz/Article/details/gdyuddtsf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.fanxiaobao.xyz/Article/details/grxhfxles.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.fanxiaobao.xyz/Article/details/gyukybbph.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowoijfcy.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.fanxiaobao.xyz/Article/details/gukminjzn.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guyrwwnkj.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/gplrqfrun.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.fanxiaobao.xyz/Article/details/ghcjhbaeg.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.fanxiaobao.xyz/Article/details/ghksgkdow.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.fanxiaobao.xyz/Article/details/gsmfxcpop.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/goqieonhx.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gaileyrgg.sHtML

K. JSON 与序列化
来源：http://baike.fanxiaobao.xyz/Article/details/glokxlrqn.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqwnefum.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.fanxiaobao.xyz/Article/details/glzhxtelg.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.fanxiaobao.xyz/Article/details/gmyhaxjbs.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbarmaner.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokkpeibv.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxxbslrl.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.fanxiaobao.xyz/Article/details/ggftzpzif.sHtML

Go:   json.Marshal(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gfqpgllfn.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.fanxiaobao.xyz/Article/details/gspjcnrhn.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gidozfaez.sHtML

[K02] JSON 字符串转对象
来源：http://3g.fanxiaobao.xyz/Article/details/gsksaszqy.sHtML

Py:   json.loads(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbwfryld.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.fanxiaobao.xyz/Article/details/gvdbyneuj.sHtML

JS:   JSON.parse(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrkisxqa.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjymjjvv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.fanxiaobao.xyz/Article/details/geqqefltb.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.fanxiaobao.xyz/Article/details/gdkpesnlq.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjussdiki.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmdrnopd.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.fanxiaobao.xyz/Article/details/grtznitez.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.fanxiaobao.xyz/Article/details/gmdevbglc.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.fanxiaobao.xyz/Article/details/goausdzxr.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gstyrxwbt.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnktlkdi.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsbrtifk.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.fanxiaobao.xyz/Article/details/goeyqnsok.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkbafkpj.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsdzdxxz.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmkjectt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.fanxiaobao.xyz/Article/details/gubsiexus.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.fanxiaobao.xyz/Article/details/grekaruvw.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fanxiaobao.xyz/Article/details/ggcrbmwbu.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fanxiaobao.xyz/Article/details/gnlzeyxej.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.fanxiaobao.xyz/Article/details/gswtzixgz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhnmmodz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtwywdwe.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gphdbrdbd.sHtML

[K05] 深拷贝对象
来源：http://mobile.fanxiaobao.xyz/Article/details/gpymuejuq.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqmbtmjr.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.fanxiaobao.xyz/Article/details/gntkoyjqx.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebvrivun.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrrpvntb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfulflwy.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyubsabe.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntcnqpic.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqckquuzz.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.fanxiaobao.xyz/Article/details/gokokcjzb.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmprdxzwk.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnpxirln.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdpcdbmt.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fanxiaobao.xyz/Article/details/gykmlrczm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywpyfqjz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.fanxiaobao.xyz/Article/details/geveojnpt.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.fanxiaobao.xyz/Article/details/giofvnxui.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.fanxiaobao.xyz/Article/details/gexwkqadk.sHtML

[K07] 进制转换
来源：http://baike.fanxiaobao.xyz/Article/details/gfxakhimo.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyfygvzn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.fanxiaobao.xyz/Article/details/gvuorefak.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmatwodjt.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvyqhekz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.fanxiaobao.xyz/Article/details/givgeolcw.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqtlbsvs.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifyiymcg.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbppznos.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.fanxiaobao.xyz/Article/details/gzoxklply.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gehedrxwa.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/geianzone.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.fanxiaobao.xyz/Article/details/gidjjwexf.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fanxiaobao.xyz/Article/details/gojxdktlv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fanxiaobao.xyz/Article/details/ggsodkisw.sHtML

Go:   encoding/gob
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchiztrub.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gtxxaiqhz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.fanxiaobao.xyz/Article/details/ggqrkkbtn.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvdcrjzw.sHtML

L. 网络请求
来源：http://3g.fanxiaobao.xyz/Article/details/gxdkiixjt.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gqltoogrg.sHtML

[L01] 发送 GET 请求
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvzmmyqg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fanxiaobao.xyz/Article/details/gnfvelfiq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.fanxiaobao.xyz/Article/details/guzrnoitq.sHtML

JS:   await fetch(url)
来源：http://wap.fanxiaobao.xyz/Article/details/gbujgpmgj.sHtML

TS:   await fetch(url)
来源：http://wap.fanxiaobao.xyz/Article/details/grkfvpnmb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrwzfowl.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.fanxiaobao.xyz/Article/details/gjwcufmxg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.fanxiaobao.xyz/Article/details/gvubhehwt.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghexicmxc.sHtML

[L02] 发送 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gshhpoggt.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fanxiaobao.xyz/Article/details/giofeewdy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwfsdlfb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcvgmxer.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fanxiaobao.xyz/Article/details/giotnobgn.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fanxiaobao.xyz/Article/details/gtakjfztc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fanxiaobao.xyz/Article/details/gswowthav.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzriaegl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fanxiaobao.xyz/Article/details/gzdgjfqdp.sHtML

[L03] 设置自定义请求头
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvbxghec.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.fanxiaobao.xyz/Article/details/gueqgrapq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkihwmgzm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fanxiaobao.xyz/Article/details/gaytkvske.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejgisgop.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwmpsgac.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fanxiaobao.xyz/Article/details/gkqaigwus.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbuejnwke.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fanxiaobao.xyz/Article/details/gskawczbr.sHtML

[L04] 设置超时
来源：http://wap.fanxiaobao.xyz/Article/details/gvehmgymz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.fanxiaobao.xyz/Article/details/gshsiadyu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.fanxiaobao.xyz/Article/details/gjmeraykc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklhmqbft.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fanxiaobao.xyz/Article/details/gyuqrhtlw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fanxiaobao.xyz/Article/details/gnhipidyo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.fanxiaobao.xyz/Article/details/gonfmcofz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fanxiaobao.xyz/Article/details/gkjglqwuf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gyrzdiqjj.sHtML

[L05] 上传文件（multipart）
来源：http://3g.fanxiaobao.xyz/Article/details/guoaeqhvn.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fanxiaobao.xyz/Article/details/gbprbagye.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gguskeojx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrcoesgv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fanxiaobao.xyz/Article/details/gfmtyqwmq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.fanxiaobao.xyz/Article/details/gjseeigdb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekjlqifw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fanxiaobao.xyz/Article/details/gurzgrkqi.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gculcijrb.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gfdvwquvw.sHtML

Py:   resp.json()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezirbybg.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fanxiaobao.xyz/Article/details/gtdiwtiux.sHtML

JS:   await resp.json()
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxwsjvzl.sHtML

TS:   await resp.json()
来源：http://www.share.fanxiaobao.xyz/Article/details/gyskcoepj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpwlvyfo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fanxiaobao.xyz/Article/details/gybraxuig.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnedbjzfo.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fanxiaobao.xyz/Article/details/gwsnodigp.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/guyevping.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fanxiaobao.xyz/Article/details/gifueedcu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.fanxiaobao.xyz/Article/details/gphektcnq.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fanxiaobao.xyz/Article/details/gkntdappk.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fanxiaobao.xyz/Article/details/gebyppojw.sHtML

Java: resp.statusCode()
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcwmpqni.sHtML

Go:   resp.StatusCode
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcijtman.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fanxiaobao.xyz/Article/details/gygvyqjah.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fanxiaobao.xyz/Article/details/guplwdntn.sHtML

[L08] 并发请求多个地址
来源：http://baike.fanxiaobao.xyz/Article/details/gshqcxeor.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fanxiaobao.xyz/Article/details/gctraxska.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fanxiaobao.xyz/Article/details/gdpwjcicd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fanxiaobao.xyz/Article/details/gnipwuxlr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fanxiaobao.xyz/Article/details/gkhwrxlps.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fanxiaobao.xyz/Article/details/gpqlnftan.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fanxiaobao.xyz/Article/details/gkygdlzag.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqiyqysg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/gazobqeaw.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbdaewnk.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fanxiaobao.xyz/Article/details/gofukihbd.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gigzsjtbw.sHtML

[M01] 读取命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjeldivv.sHtML

Py:   sys.argv[1:]
来源：http://baike.fanxiaobao.xyz/Article/details/gomjavysr.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glapxakqj.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyupembug.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fanxiaobao.xyz/Article/details/grlfulaja.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjfifjon.sHtML

Go:   os.Args[1:]
来源：http://blog.fanxiaobao.xyz/Article/details/glhbnttbl.sHtML

Ruby: ARGV
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcunwdzk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.fanxiaobao.xyz/Article/details/glqqvntiq.sHtML

[M02] 读取环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/goewsesbd.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjvxrxes.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxdgaleh.sHtML

JS:   process.env.HOME
来源：http://wap.fanxiaobao.xyz/Article/details/gqifnekni.sHtML

TS:   process.env.HOME
来源：http://read.share.fanxiaobao.xyz/Article/details/gammbpvww.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpdcspcr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fanxiaobao.xyz/Article/details/gszhhtwip.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikwtlskk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrvqooau.sHtML

[M03] 执行外部命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gevwdhnnz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gstowxsvf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fanxiaobao.xyz/Article/details/ggefomcfu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgxxznxn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fanxiaobao.xyz/Article/details/geufztcuc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcfubfzi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fanxiaobao.xyz/Article/details/glzrawcks.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfqouczf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyxrsilz.sHtML

[M04] 获取当前工作目录
来源：http://3g.fanxiaobao.xyz/Article/details/gmjoqxkzr.sHtML

Py:   os.getcwd()
来源：http://blog.fanxiaobao.xyz/Article/details/gwhimnkej.sHtML

PHP:  getcwd();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmghkxhlk.sHtML

JS:   process.cwd()
来源：http://3g.fanxiaobao.xyz/Article/details/grqdgriod.sHtML

TS:   process.cwd()
来源：http://wap.fanxiaobao.xyz/Article/details/gyqaesfcf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fanxiaobao.xyz/Article/details/giiryfhde.sHtML

Go:   os.Getwd()
来源：http://www.share.fanxiaobao.xyz/Article/details/gicpdjmrd.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fanxiaobao.xyz/Article/details/geomjrjgq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkcfgalb.sHtML

[M05] 设置退出码
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqnhmoie.sHtML

Py:   sys.exit(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdptotefm.sHtML

PHP:  exit(1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkssxuyz.sHtML

JS:   process.exit(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gdbjqasfx.sHtML

TS:   process.exit(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjwpaijm.sHtML

Java: System.exit(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gichnayaa.sHtML

Go:   os.Exit(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gtqxdukok.sHtML

Ruby: exit 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gykcbrsvk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkcorwuz.sHtML

[M06] 向标准错误输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gabqsamzj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gosgnkmmc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxtcljym.sHtML

JS:   console.error("err")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgfbjplo.sHtML

TS:   console.error("err")
来源：http://m.share.fanxiaobao.xyz/Article/details/gnplamjhk.sHtML

Java: System.err.println("err")
来源：http://blog.fanxiaobao.xyz/Article/details/gltixzuwv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fanxiaobao.xyz/Article/details/gobquohfc.sHtML

Ruby: warn "err"
来源：http://m.share.fanxiaobao.xyz/Article/details/gcyivofbl.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fanxiaobao.xyz/Article/details/gslkwsbom.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrhlzmyc.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fanxiaobao.xyz/Article/details/gynlhxjhw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fanxiaobao.xyz/Article/details/gsujtjqja.sHtML

JS:   require.main === module
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuekdbcz.sHtML

TS:   require.main === module
来源：http://mobile.fanxiaobao.xyz/Article/details/gerbclxbw.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhdsrqzg.sHtML

Go:   func main()
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjtibddl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpuzlmiuy.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwqozmba.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.fanxiaobao.xyz/Article/details/ghizffscc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fanxiaobao.xyz/Article/details/galehdyaq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gervkbrkm.sHtML

JS:   process.platform;  process.version
来源：http://wap.fanxiaobao.xyz/Article/details/gxtohrhao.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvviyfsjw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskhcusax.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fanxiaobao.xyz/Article/details/gjvrjufne.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fanxiaobao.xyz/Article/details/gzvnpqvua.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfnrgxpx.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/giuetfwkm.sHtML

N. 数据结构与算法
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkslaegz.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbigwrrh.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fanxiaobao.xyz/Article/details/gmvwwkbtv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fanxiaobao.xyz/Article/details/gxnnghqrk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghemotblv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fanxiaobao.xyz/Article/details/gvbpwptoc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpagsquth.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbugvvqlz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxaauvrmt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fanxiaobao.xyz/Article/details/grqcldrlw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdrjhejh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fanxiaobao.xyz/Article/details/gbfvvdkld.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fanxiaobao.xyz/Article/details/gadavxpwc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvhrwdvl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fanxiaobao.xyz/Article/details/giltnxqjn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fanxiaobao.xyz/Article/details/gafzmluwf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fanxiaobao.xyz/Article/details/gascthvmz.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwzlslaa.sHtML

Ruby: arr.sort
来源：http://wap.fanxiaobao.xyz/Article/details/gmfozqtpg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fanxiaobao.xyz/Article/details/gqqpbciks.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fanxiaobao.xyz/Article/details/gshkcjsse.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbjylucy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fanxiaobao.xyz/Article/details/grmkepepe.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkzxtuwd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fanxiaobao.xyz/Article/details/gxsdnolxh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fanxiaobao.xyz/Article/details/garocjnto.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fanxiaobao.xyz/Article/details/gncfezzhe.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fanxiaobao.xyz/Article/details/gykddtgux.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gechvqfnx.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvytdqzjw.sHtML


<!-- 参考信息 -->