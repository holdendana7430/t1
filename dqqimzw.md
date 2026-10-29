代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.zdbjq.cn/Article/details/gjfzklzqu.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.hesvh.cn/Article/details/glxxxkhiw.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.fehbvm.com/Article/details/gjiebwdfl.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.zdbjq.cn/Article/details/geepirqpo.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.hesvh.cn/Article/details/gppndpcyk.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.hesvh.cn/Article/details/gsfuzcsws.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.zdbjq.cn/Article/details/gableqzzd.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.zdbjq.cn/Article/details/gcmivxhys.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.fehbvm.com/Article/details/gipodtouc.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.hesvh.cn/Article/details/gexusatyh.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.zdbjq.cn/Article/details/gkusxqizx.sHtML

[J06] 计算两时间之差
来源：http://baike.zdbjq.cn/Article/details/gmzrxdtvn.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.fehbvm.com/Article/details/geuivfoyl.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.fehbvm.com/Article/details/gvruyckpm.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.hesvh.cn/Article/details/gcyzdlfgu.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.fehbvm.com/Article/details/gvokueddb.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.zdbjq.cn/Article/details/gplmbbdep.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.hesvh.cn/Article/details/gmspdmzrn.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.zdbjq.cn/Article/details/gaoiahwtq.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.fehbvm.com/Article/details/gfnywzrdg.sHtML

[J07] 比较两个日期
来源：http://m.share.hesvh.cn/Article/details/gexpaagom.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/gemmpdbbg.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.fehbvm.com/Article/details/ghckkyllb.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.hesvh.cn/Article/details/ghexwqbai.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.hesvh.cn/Article/details/gxkccwxjm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.hesvh.cn/Article/details/gebhyettr.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.zdbjq.cn/Article/details/gzbsgjlar.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/ghkfeobvg.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.hesvh.cn/Article/details/gamhwvkit.sHtML

[J08] 提取年月日与星期
来源：http://3g.hesvh.cn/Article/details/gludbxgcg.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.zdbjq.cn/Article/details/gsmebwbuk.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.zdbjq.cn/Article/details/gbuaqaxcy.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.fehbvm.com/Article/details/gduulxxwh.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.zdbjq.cn/Article/details/gdvqrfnlk.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.hesvh.cn/Article/details/gknvyriba.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.hesvh.cn/Article/details/ggcxubsle.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.zdbjq.cn/Article/details/gfqrdqsmi.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.hesvh.cn/Article/details/gajgsjcnu.sHtML

[J09] 时区处理
来源：http://read.share.hesvh.cn/Article/details/guqbhqoyc.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.zdbjq.cn/Article/details/gunuqtinu.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.zdbjq.cn/Article/details/gakgggqdc.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fehbvm.com/Article/details/ggqdsoljl.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.zdbjq.cn/Article/details/gkqdrvmhv.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.hesvh.cn/Article/details/glphfjpbf.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.hesvh.cn/Article/details/gdcstrktk.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.hesvh.cn/Article/details/gyfwwjrvr.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.zdbjq.cn/Article/details/gseggamae.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.zdbjq.cn/Article/details/goihrugza.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.fehbvm.com/Article/details/gbcjftuet.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.zdbjq.cn/Article/details/gclolcomb.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.hesvh.cn/Article/details/gasqwyccz.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.hesvh.cn/Article/details/gfhvdclol.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gregfeqhg.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.zdbjq.cn/Article/details/gociqqrkl.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.hesvh.cn/Article/details/gugakrrrc.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.hesvh.cn/Article/details/gshnhxfeu.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjcqhdnuv.sHtML

K. JSON 与序列化
来源：http://wap.hesvh.cn/Article/details/guzmktvbg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gohcydlhc.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.hesvh.cn/Article/details/glqtikczv.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.zdbjq.cn/Article/details/gayaedhao.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/gdjzewujt.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.fehbvm.com/Article/details/gdiszgmns.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.zdbjq.cn/Article/details/gaxqyxliv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.fehbvm.com/Article/details/gxbkptnst.sHtML

Go:   json.Marshal(obj)
来源：http://wap.zdbjq.cn/Article/details/ggbnyavqd.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.hesvh.cn/Article/details/gjgtrpscy.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.zdbjq.cn/Article/details/gpjrglhfy.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.hesvh.cn/Article/details/gamogozgf.sHtML

Py:   json.loads(s)
来源：http://www.m.share.hesvh.cn/Article/details/gnvxifdsn.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.zdbjq.cn/Article/details/gnukvhgtj.sHtML

JS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gsxnipoky.sHtML

TS:   JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/gmisbchpn.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.hesvh.cn/Article/details/gzgyzvgmu.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.fehbvm.com/Article/details/gdxlxeiud.sHtML

Ruby: JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gcrgzbjgy.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.zdbjq.cn/Article/details/gytdhroei.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.fehbvm.com/Article/details/gppvxpxzf.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gdnqdmwya.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.zdbjq.cn/Article/details/grkhqtrnq.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.hesvh.cn/Article/details/glaolwjcl.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.hesvh.cn/Article/details/gwtprmfcp.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.fehbvm.com/Article/details/gvqrsyamf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.hesvh.cn/Article/details/gxgcjtbft.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.hesvh.cn/Article/details/guebuynal.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.hesvh.cn/Article/details/gjsaiwcls.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.fehbvm.com/Article/details/gyafkebbx.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.hesvh.cn/Article/details/ghqjnqscf.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.zdbjq.cn/Article/details/gugcujeap.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/goeityhdk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/gxocfizzl.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gxmcvzxrf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/gsxzteler.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.fehbvm.com/Article/details/gboxpehcx.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.fehbvm.com/Article/details/grydbtuvq.sHtML

[K05] 深拷贝对象
来源：http://read.share.hesvh.cn/Article/details/gtxtkmldj.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.hesvh.cn/Article/details/glnnkcqkh.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.fehbvm.com/Article/details/gihticskr.sHtML

JS:   structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gpqmsvgbx.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gzbjilsqo.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.hesvh.cn/Article/details/grcpfwxkd.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.hesvh.cn/Article/details/gkfmaqacy.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/ghcuwnxdn.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.zdbjq.cn/Article/details/gjmxnmmbf.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.hesvh.cn/Article/details/gkladzbkq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gnewcqaax.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.zdbjq.cn/Article/details/gxhoseheo.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/gkngheskt.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/geuxyindb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.fehbvm.com/Article/details/glbbpdqwc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gnfsjxblg.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gnqdntqfw.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gyvfhozaq.sHtML

[K07] 进制转换
来源：http://mobile.fehbvm.com/Article/details/ghizqdosr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gjhkpnlem.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.hesvh.cn/Article/details/gjepjqrgi.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gjvpzasxd.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gcyhoolfy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gxxntzezi.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.fehbvm.com/Article/details/gxvfsogzl.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.zdbjq.cn/Article/details/gatvhyhsq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gahfjlran.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.zdbjq.cn/Article/details/gnhpiyfma.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.fehbvm.com/Article/details/gphvqugyu.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.zdbjq.cn/Article/details/gbazgmhum.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/ggsmaatak.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/ghwxazwys.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.zdbjq.cn/Article/details/gkcbzlgpw.sHtML

Go:   encoding/gob
来源：http://m.share.hesvh.cn/Article/details/gjpczscrw.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.zdbjq.cn/Article/details/grtmcossl.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gxceznsur.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/goumqnzey.sHtML

L. 网络请求
来源：http://3g.hesvh.cn/Article/details/gpocogpro.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gerzjliib.sHtML

[L01] 发送 GET 请求
来源：http://www.share.fehbvm.com/Article/details/geynorgss.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fehbvm.com/Article/details/gxlevahjk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.hesvh.cn/Article/details/gqsmhgoeh.sHtML

JS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/goeuzvwov.sHtML

TS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/giirtubmb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.fehbvm.com/Article/details/glwrdppls.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fehbvm.com/Article/details/gzplegkhp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.hesvh.cn/Article/details/gsybtgmdg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.hesvh.cn/Article/details/godaqgbii.sHtML

[L02] 发送 POST JSON
来源：http://baike.zdbjq.cn/Article/details/giunxqlvo.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gqmhdndxr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.hesvh.cn/Article/details/gxffdyvne.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/gmdvumkdq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/ggwrjnwwe.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fehbvm.com/Article/details/gjmphjyjd.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.hesvh.cn/Article/details/gvrtbjblt.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.zdbjq.cn/Article/details/grmcjgdyh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.fehbvm.com/Article/details/gkcewtxjp.sHtML

[L03] 设置自定义请求头
来源：http://mobile.zdbjq.cn/Article/details/gyujfdwnp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.hesvh.cn/Article/details/gvrctoaky.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.hesvh.cn/Article/details/gywgrqxdd.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gnblfnfow.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/ghgefzhan.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.hesvh.cn/Article/details/gqiqjgbsh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gbtxtpqic.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.hesvh.cn/Article/details/gsuxxdnvk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gggzowcpx.sHtML

[L04] 设置超时
来源：http://mobile.zdbjq.cn/Article/details/gjlijmqrz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.hesvh.cn/Article/details/gzgavckqw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.zdbjq.cn/Article/details/gjootfyhf.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/goemqzpvo.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gggumzsqe.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.hesvh.cn/Article/details/geizkwybg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.zdbjq.cn/Article/details/gqngncpfv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.hesvh.cn/Article/details/gbjfsrccg.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fehbvm.com/Article/details/gmnqfmojt.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.hesvh.cn/Article/details/ggnjrqesi.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fehbvm.com/Article/details/gpsrzelhc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.hesvh.cn/Article/details/gezfgwsuf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gjeyifznb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gnlgbqyzi.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.hesvh.cn/Article/details/gcenihiaj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.hesvh.cn/Article/details/geqspesby.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fehbvm.com/Article/details/gvnigovct.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.zdbjq.cn/Article/details/guxiqurmb.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gxsswihny.sHtML

Py:   resp.json()
来源：http://m.share.zdbjq.cn/Article/details/giwsrvaik.sHtML

PHP:  json_decode($body, true);
来源：http://3g.zdbjq.cn/Article/details/gonkqqfij.sHtML

JS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/ghmndhzel.sHtML

TS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gnblecpqj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gdoccfngt.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.zdbjq.cn/Article/details/ggtitrrsg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.zdbjq.cn/Article/details/glnnjsyzt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fehbvm.com/Article/details/gcrxyrowu.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gtdxwhqtk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.hesvh.cn/Article/details/gsljjrlte.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.zdbjq.cn/Article/details/gxchvpqum.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gzxloqavw.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gsbxeadku.sHtML

Java: resp.statusCode()
来源：http://3g.zdbjq.cn/Article/details/giwdqywii.sHtML

Go:   resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gqwhshtbm.sHtML

Ruby: resp.code.to_i
来源：http://blog.fehbvm.com/Article/details/gpsitjqgk.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gkyuxpkhq.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fehbvm.com/Article/details/gijcjzoam.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fehbvm.com/Article/details/gsirtohsv.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.zdbjq.cn/Article/details/gppszyebf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/goxvrrmhr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/guzcuktvm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.zdbjq.cn/Article/details/gsozaupka.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.hesvh.cn/Article/details/gnalcwvea.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.hesvh.cn/Article/details/gkuitvvof.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/geqotqsuy.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gedvklbai.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.hesvh.cn/Article/details/gtewmeagu.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/giovmbxba.sHtML

[M01] 读取命令行参数
来源：http://baike.fehbvm.com/Article/details/gcapromri.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.hesvh.cn/Article/details/gopqmgfcg.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fehbvm.com/Article/details/gqetacuvn.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gkuywrrli.sHtML

TS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gpdkglhnl.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/glciwezqs.sHtML

Go:   os.Args[1:]
来源：http://wap.zdbjq.cn/Article/details/gkrqqbdku.sHtML

Ruby: ARGV
来源：http://m.share.fehbvm.com/Article/details/gzqdxhxip.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gimoantdx.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/gfakmecbl.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gfkgzjavc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gespjuymh.sHtML

JS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gimzhbmqt.sHtML

TS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gjwrrecjn.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gjcencmbo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gfclnwcnn.sHtML

Ruby: ENV["HOME"]
来源：http://wap.hesvh.cn/Article/details/ghnbdvaul.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gjinwhepa.sHtML

[M03] 执行外部命令
来源：http://www.blog.zdbjq.cn/Article/details/gkfebpwem.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.hesvh.cn/Article/details/gldnzjlnx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.hesvh.cn/Article/details/gfpqegsfx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gngifrkfd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gbauqflpa.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.fehbvm.com/Article/details/gavetoejb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/ganaoamnw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fehbvm.com/Article/details/ghdywdehv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.zdbjq.cn/Article/details/gyvvyfnmi.sHtML

[M04] 获取当前工作目录
来源：http://3g.zdbjq.cn/Article/details/gfdmuxbdi.sHtML

Py:   os.getcwd()
来源：http://m.share.zdbjq.cn/Article/details/gddrjtbmj.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gvfuzqzro.sHtML

JS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gkaybdfsn.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gjhdhrchu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fehbvm.com/Article/details/gafxtnycl.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/gnnpdkxti.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/ggcfhwxgy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/gsrjltgit.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/gcunekcfz.sHtML

Py:   sys.exit(1)
来源：http://3g.fehbvm.com/Article/details/geuhjmxub.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/gkgkwqdfq.sHtML

JS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gzxeulads.sHtML

TS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gpgbdyhow.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gcqkjtihm.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/ggemdzskk.sHtML

Ruby: exit 1
来源：http://www.blog.fehbvm.com/Article/details/gjvvaxhzj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.hesvh.cn/Article/details/ghxknexzv.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fehbvm.com/Article/details/gzwhkgrqj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gkrvezavw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gyfebojsk.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gzjoyuhec.sHtML

TS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gkhzswekr.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/gpccigghl.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/ghepkuflu.sHtML

Ruby: warn "err"
来源：http://read.share.fehbvm.com/Article/details/gwijtpjrq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/gdxkiuoxp.sHtML

[M07] 判断是否为主入口
来源：http://3g.fehbvm.com/Article/details/gasdyedkt.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/gnnivcvpj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fehbvm.com/Article/details/gzadrimzu.sHtML

JS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gvfhvkblj.sHtML

TS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gjiumgame.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.hesvh.cn/Article/details/gbkskhlxm.sHtML

Go:   func main()
来源：http://m.share.fehbvm.com/Article/details/goqmswwfp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gkcndxcdh.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.zdbjq.cn/Article/details/guconcvvl.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/gasklgqiv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/gjqetlanp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.hesvh.cn/Article/details/gpuzfpwjg.sHtML

JS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/geupndnwi.sHtML

TS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/ghujxddoi.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.hesvh.cn/Article/details/glxjfgjkz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.zdbjq.cn/Article/details/gurpxojwo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/gawrccsvv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fehbvm.com/Article/details/grxspqtiy.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdnowidvw.sHtML

N. 数据结构与算法
来源：http://www.blog.hesvh.cn/Article/details/gwyfrvuwx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqcofftau.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.zdbjq.cn/Article/details/gjptdfymz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gkiypuxhd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.hesvh.cn/Article/details/gaaltkynu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gnvehtybu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gajgjhtqr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gpzlylggn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gmzrbwkql.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/gkhxkmcot.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gvrouokfy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.zdbjq.cn/Article/details/gcflfujwz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/ggfaccsbk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/grayyuuat.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gatrflyri.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gtduepddj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/gqoijexnn.sHtML

Go:   slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gdpjpvxxm.sHtML


<!-- 参考信息 -->