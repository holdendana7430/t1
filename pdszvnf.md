代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.zdbjq.cn/Article/details/gahexpihx.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fehbvm.com/Article/details/getxetqdt.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.hesvh.cn/Article/details/gmnkfmlbb.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.fehbvm.com/Article/details/gkgjdpngz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.fehbvm.com/Article/details/gfzyczgxl.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.zdbjq.cn/Article/details/garhfcckf.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.hesvh.cn/Article/details/gbuzvquzw.sHtML

[J06] 计算两时间之差
来源：http://3g.zdbjq.cn/Article/details/ginbddtzi.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.hesvh.cn/Article/details/gifekqmor.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.fehbvm.com/Article/details/ghlmrkwxj.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.zdbjq.cn/Article/details/gavmuovvn.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.hesvh.cn/Article/details/gleuzewux.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.fehbvm.com/Article/details/gypwidgez.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.hesvh.cn/Article/details/gktadsljt.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.fehbvm.com/Article/details/ggczhqiby.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.fehbvm.com/Article/details/gxmxqzlul.sHtML

[J07] 比较两个日期
来源：http://mobile.fehbvm.com/Article/details/gkfonhvcl.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.hesvh.cn/Article/details/gcsglnync.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.fehbvm.com/Article/details/gxpdyiyua.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.hesvh.cn/Article/details/gexblalxe.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.fehbvm.com/Article/details/gifydxkym.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.hesvh.cn/Article/details/gnoorllcj.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.hesvh.cn/Article/details/gxbbkhrug.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.hesvh.cn/Article/details/gdxfetxgi.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.zdbjq.cn/Article/details/glznhubdu.sHtML

[J08] 提取年月日与星期
来源：http://3g.fehbvm.com/Article/details/griwrqqan.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.hesvh.cn/Article/details/gqgabpgzt.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.zdbjq.cn/Article/details/ghnatpanm.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.hesvh.cn/Article/details/ggdvpfocq.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.fehbvm.com/Article/details/gifajhekq.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.hesvh.cn/Article/details/gbbyapmdj.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.zdbjq.cn/Article/details/gkdmtjnrp.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.zdbjq.cn/Article/details/gwimeuonn.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.fehbvm.com/Article/details/gkmvnhnkp.sHtML

[J09] 时区处理
来源：http://www.share.fehbvm.com/Article/details/gmenhchqv.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.zdbjq.cn/Article/details/gzkmpqada.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.hesvh.cn/Article/details/gwgxftzyr.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.zdbjq.cn/Article/details/gfjuizdfu.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fehbvm.com/Article/details/gecaazmjc.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.zdbjq.cn/Article/details/gflnoirko.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.hesvh.cn/Article/details/ggnlbacaa.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.fehbvm.com/Article/details/gdteawrpt.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.fehbvm.com/Article/details/gaxbnbjcz.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.zdbjq.cn/Article/details/gyonwgckj.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.hesvh.cn/Article/details/gvrrbrdad.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.zdbjq.cn/Article/details/gzvsipbor.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.zdbjq.cn/Article/details/gheiibkai.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.hesvh.cn/Article/details/gprhpvnse.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.zdbjq.cn/Article/details/gnohzarwm.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.fehbvm.com/Article/details/gvutjbkkk.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.zdbjq.cn/Article/details/gqpzkynaz.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.zdbjq.cn/Article/details/grvynjnar.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gsbmpirtc.sHtML

K. JSON 与序列化
来源：http://3g.hesvh.cn/Article/details/gfzhxbqkt.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/guldxkqdn.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.fehbvm.com/Article/details/ghsewhwrk.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.zdbjq.cn/Article/details/gvskxvlnl.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/gsvrgizkq.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.fehbvm.com/Article/details/gutohkibh.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.hesvh.cn/Article/details/gidiouvfx.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.zdbjq.cn/Article/details/gmkgunlvp.sHtML

Go:   json.Marshal(obj)
来源：http://blog.fehbvm.com/Article/details/gldydqmuk.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.hesvh.cn/Article/details/glvgzrzim.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.fehbvm.com/Article/details/gwyvrjznk.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.zdbjq.cn/Article/details/ghauvvewe.sHtML

Py:   json.loads(s)
来源：http://baike.zdbjq.cn/Article/details/gfrduxtqz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.fehbvm.com/Article/details/gckisdmvg.sHtML

JS:   JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/gpncfozhr.sHtML

TS:   JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gjbqwdfal.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gqtavihtw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.zdbjq.cn/Article/details/glpqrsxro.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/gdcojgggg.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.hesvh.cn/Article/details/gnehieqzb.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.hesvh.cn/Article/details/gysvwsvoz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.fehbvm.com/Article/details/gcklmczao.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/gdunknnzs.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gcqrqwpqy.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/gtylubwop.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.fehbvm.com/Article/details/gydmgbnev.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.zdbjq.cn/Article/details/gbuvkclsd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gcckxnkef.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.hesvh.cn/Article/details/gucineiaa.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.zdbjq.cn/Article/details/glxoiscid.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.zdbjq.cn/Article/details/gmncmpcif.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.hesvh.cn/Article/details/gmfqsebmh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.hesvh.cn/Article/details/gkkwakokk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/geeyqrrvd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.fehbvm.com/Article/details/grjoeeila.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/ghfwscusm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/gjcyefysp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.fehbvm.com/Article/details/gygjnpghd.sHtML

[K05] 深拷贝对象
来源：http://www.blog.fehbvm.com/Article/details/gtknvahmg.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.zdbjq.cn/Article/details/ghfeftngu.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.fehbvm.com/Article/details/ghfatmrex.sHtML

JS:   structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gaqyanvwn.sHtML

TS:   structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gnspkesvu.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fehbvm.com/Article/details/gibxukkfl.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.zdbjq.cn/Article/details/gbpailezb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.hesvh.cn/Article/details/grkwmoreu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.hesvh.cn/Article/details/gdiakuvrb.sHtML

[K06] 解析 URL 查询串
来源：http://wap.zdbjq.cn/Article/details/gscozhdyf.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/gcvukbfog.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.zdbjq.cn/Article/details/gpxxdxlka.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fehbvm.com/Article/details/genpjsynn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/ggttxkygb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.fehbvm.com/Article/details/goteyxtpi.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/gkkbpmfwb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gfjpstlvx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gxikvdalq.sHtML

[K07] 进制转换
来源：http://baike.hesvh.cn/Article/details/gcisrzsgo.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/ghehlseln.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.zdbjq.cn/Article/details/grgbtgclh.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gkpwxhqyi.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/grrjootxm.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gbouigxbp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.hesvh.cn/Article/details/gzffmryzu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.hesvh.cn/Article/details/gxxilawhw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gxebgedmr.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.zdbjq.cn/Article/details/gcelkwzbb.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.zdbjq.cn/Article/details/gwlaajzas.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fehbvm.com/Article/details/gtnmmoano.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/gcbvxtvcs.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/gpulbucfb.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.zdbjq.cn/Article/details/gqzmxemgv.sHtML

Go:   encoding/gob
来源：http://m.share.fehbvm.com/Article/details/gkrmnlvbt.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.hesvh.cn/Article/details/gzcikogdp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gqmgabnvz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxjraslwh.sHtML

L. 网络请求
来源：http://wap.fehbvm.com/Article/details/gocvwvcty.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtkjnuaff.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.zdbjq.cn/Article/details/gmqwosfuc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.fehbvm.com/Article/details/gicwfngfx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.fehbvm.com/Article/details/gwyybaond.sHtML

JS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gxhgwhtif.sHtML

TS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gzwokhyew.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.hesvh.cn/Article/details/gzaympmlv.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.zdbjq.cn/Article/details/gsuttbtkk.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.hesvh.cn/Article/details/gcuwzflpn.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.hesvh.cn/Article/details/gqsmhwozm.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gtzrtszfg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.fehbvm.com/Article/details/gpwrtwybb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.hesvh.cn/Article/details/ghxuoxvmo.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/gqmelfrou.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/gkjtmjunl.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.fehbvm.com/Article/details/gdpuspgqm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.hesvh.cn/Article/details/gtaxizktp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.fehbvm.com/Article/details/gmjokileh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.zdbjq.cn/Article/details/gyvidxfag.sHtML

[L03] 设置自定义请求头
来源：http://baike.hesvh.cn/Article/details/ghsttgzfv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.zdbjq.cn/Article/details/gmdjzhmro.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.fehbvm.com/Article/details/grkcdbuea.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gtfzdjedx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gwydygvsb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.zdbjq.cn/Article/details/gnxebmhgc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gsknkputj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.zdbjq.cn/Article/details/gcipflivd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gpkgpbgjg.sHtML

[L04] 设置超时
来源：http://m.share.hesvh.cn/Article/details/gyjeuumnx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.zdbjq.cn/Article/details/gixaibzfr.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gmxivhbze.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gvskbhlql.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gizlarmyh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.hesvh.cn/Article/details/geuhdhmab.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.hesvh.cn/Article/details/gixzmyouf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.hesvh.cn/Article/details/gpxxavuwy.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fehbvm.com/Article/details/grbnrteqa.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.zdbjq.cn/Article/details/grmckrzkz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.hesvh.cn/Article/details/gizvfncyn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.zdbjq.cn/Article/details/gsfmbqact.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gfpuymeou.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/grthppjig.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/gacjgiohs.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.zdbjq.cn/Article/details/guwibuidq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.hesvh.cn/Article/details/gtnpdwnro.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fehbvm.com/Article/details/goibewskw.sHtML

[L06] 解析响应为 JSON
来源：http://blog.zdbjq.cn/Article/details/gtfdrztgg.sHtML

Py:   resp.json()
来源：http://mobile.hesvh.cn/Article/details/grpevaapi.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.zdbjq.cn/Article/details/gomwpilir.sHtML

JS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gninclsez.sHtML

TS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gfsmmfdcp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gequotckj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.zdbjq.cn/Article/details/gvptettlk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.zdbjq.cn/Article/details/gzqrghpds.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.zdbjq.cn/Article/details/gzozkkidh.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/grbdnqnhm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.hesvh.cn/Article/details/gmqgoampc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.hesvh.cn/Article/details/gcvvhconx.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gogpclymc.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gazgshsps.sHtML

Java: resp.statusCode()
来源：http://mobile.fehbvm.com/Article/details/gbcoqlhfy.sHtML

Go:   resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/guyxixhgq.sHtML

Ruby: resp.code.to_i
来源：http://blog.hesvh.cn/Article/details/gvokdviad.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gpkrefpel.sHtML

[L08] 并发请求多个地址
来源：http://read.share.hesvh.cn/Article/details/gcgjdhqir.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.hesvh.cn/Article/details/glsjxigxj.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.hesvh.cn/Article/details/gewvcmijw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gfncgbdpz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gibhlkoku.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.hesvh.cn/Article/details/gpzerrmif.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.zdbjq.cn/Article/details/gdrsgpxdk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.zdbjq.cn/Article/details/grhrnsurx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fehbvm.com/Article/details/gljohybjb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gkjzvhtmo.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.hesvh.cn/Article/details/ghmxuwpgy.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ganxytlok.sHtML

[M01] 读取命令行参数
来源：http://www.share.fehbvm.com/Article/details/gjjzzvoze.sHtML

Py:   sys.argv[1:]
来源：http://blog.hesvh.cn/Article/details/gaelaitbn.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.hesvh.cn/Article/details/gfrrctfej.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/glslzpoyb.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/giozfimzq.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gytspsxdw.sHtML

Go:   os.Args[1:]
来源：http://m.share.zdbjq.cn/Article/details/gejqxyfgv.sHtML

Ruby: ARGV
来源：http://read.share.hesvh.cn/Article/details/gbjmjgpdc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gmuzsdpnq.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gewtayrok.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.hesvh.cn/Article/details/gpnzewvoq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gmoyvlheb.sHtML

JS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gxklnnxib.sHtML

TS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/glirpwkti.sHtML

Java: System.getenv("HOME")
来源：http://mobile.hesvh.cn/Article/details/glyeuoxxs.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fehbvm.com/Article/details/gjavxkbws.sHtML

Ruby: ENV["HOME"]
来源：http://wap.hesvh.cn/Article/details/gyvknodui.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fehbvm.com/Article/details/gxgahvqjx.sHtML

[M03] 执行外部命令
来源：http://blog.fehbvm.com/Article/details/gbsglicqe.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fehbvm.com/Article/details/gbxxnmgfj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.hesvh.cn/Article/details/gkuobzidg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/goripttga.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/guewqalqg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.hesvh.cn/Article/details/gzyqbqavr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.hesvh.cn/Article/details/guhzrxkqd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fehbvm.com/Article/details/gpnzfjfuq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.zdbjq.cn/Article/details/gfnsuzrro.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/gxnqshxqt.sHtML

Py:   os.getcwd()
来源：http://mobile.hesvh.cn/Article/details/gkmloczjq.sHtML

PHP:  getcwd();
来源：http://read.share.zdbjq.cn/Article/details/gpfjnggtw.sHtML

JS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gqnrjjmbn.sHtML

TS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gsjexqxcw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/gkrvvaztk.sHtML

Go:   os.Getwd()
来源：http://baike.hesvh.cn/Article/details/gkfqujifk.sHtML

Ruby: Dir.pwd
来源：http://wap.hesvh.cn/Article/details/guphmrsru.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/gqqwdsvmp.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/gfvuvkljj.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gmcaqfmse.sHtML

PHP:  exit(1);
来源：http://www.share.fehbvm.com/Article/details/gbzjoiatv.sHtML

JS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gdywzluce.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gnewkglym.sHtML

Java: System.exit(1)
来源：http://wap.hesvh.cn/Article/details/geromqujq.sHtML

Go:   os.Exit(1)
来源：http://mobile.fehbvm.com/Article/details/gyaiified.sHtML

Ruby: exit 1
来源：http://www.m.share.zdbjq.cn/Article/details/gbxbghirg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.hesvh.cn/Article/details/gwohyhdsb.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/gexhyovni.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gbemjnqqs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.zdbjq.cn/Article/details/gsscoywtg.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/grnuvcwfu.sHtML

TS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/glklphgke.sHtML

Java: System.err.println("err")
来源：http://www.share.hesvh.cn/Article/details/gqeskokzp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.hesvh.cn/Article/details/glsfswlbj.sHtML

Ruby: warn "err"
来源：http://m.share.hesvh.cn/Article/details/gxodpuftp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fehbvm.com/Article/details/gzxegvumi.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/ghesqhbva.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.zdbjq.cn/Article/details/gwqyqfbno.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/golucuycy.sHtML

JS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gmrqgqhyo.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/grqxgdgnh.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/gptukxpvr.sHtML

Go:   func main()
来源：http://m.share.zdbjq.cn/Article/details/gnjaafjac.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fehbvm.com/Article/details/gjthfslph.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.hesvh.cn/Article/details/gyknwneue.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fehbvm.com/Article/details/gwzfmdiii.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fehbvm.com/Article/details/gswcfqodh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/gztajxkes.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gqmaovvbu.sHtML

TS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gtmtwphiv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.zdbjq.cn/Article/details/gemotkbru.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/gmevenluk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.zdbjq.cn/Article/details/ghxhjojbo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/gqfvpazwz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gipwxzvse.sHtML

N. 数据结构与算法
来源：http://wap.zdbjq.cn/Article/details/gggcseair.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gikkdhugp.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fehbvm.com/Article/details/ghfhjwfxf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gfpriqjpn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/gmrdiblha.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/giszqwecg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gmjcrbuuu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gfhzkvein.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gyqmrhkvo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/gpxjsnddb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gpahnmydp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/gizbtdhgb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gisirntkt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fehbvm.com/Article/details/gigfgzvju.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gwhzxxryf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gwsynavoq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/gzapnotkk.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gblkdnyfr.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gvgqasuzr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/glmjrftek.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fehbvm.com/Article/details/gtylzufav.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.zdbjq.cn/Article/details/gentpmakk.sHtML


<!-- 参考信息 -->