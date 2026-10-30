代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.fehbvm.com/Article/details/gtwtdmhyz.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.hesvh.cn/Article/details/gygkwlpti.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.zdbjq.cn/Article/details/gpndubnjd.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.fehbvm.com/Article/details/gvwgqeoym.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.zdbjq.cn/Article/details/gitvtprhy.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.zdbjq.cn/Article/details/gnnxdqool.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.fehbvm.com/Article/details/gcbfxbtco.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.hesvh.cn/Article/details/gwimvjave.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.fehbvm.com/Article/details/goxaiqwbm.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.hesvh.cn/Article/details/gmawknbbd.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.hesvh.cn/Article/details/gtinruavl.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.zdbjq.cn/Article/details/gtittmkqk.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.zdbjq.cn/Article/details/gwajtcboo.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.zdbjq.cn/Article/details/gagaakxur.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.hesvh.cn/Article/details/gcbtvpaqg.sHtML

[J06] 计算两时间之差
来源：http://www.blog.fehbvm.com/Article/details/gfbepovvx.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.zdbjq.cn/Article/details/gukaivlzh.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.fehbvm.com/Article/details/gufmlgiac.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.fehbvm.com/Article/details/gxefzdlft.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.fehbvm.com/Article/details/gmvskunhv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.hesvh.cn/Article/details/gxftoydoi.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.hesvh.cn/Article/details/gdgcgxjto.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.zdbjq.cn/Article/details/gamdpiyib.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.hesvh.cn/Article/details/ggifjgxnt.sHtML

[J07] 比较两个日期
来源：http://www.m.share.fehbvm.com/Article/details/gqfbeqyzk.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/ghhdgzkni.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.zdbjq.cn/Article/details/gjqsiedjx.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.hesvh.cn/Article/details/ghufhgrzz.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.hesvh.cn/Article/details/gzssexudc.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.hesvh.cn/Article/details/gfjhdwkwd.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.fehbvm.com/Article/details/gvsakzhsr.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/gcspxhxre.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.fehbvm.com/Article/details/grqofcchc.sHtML

[J08] 提取年月日与星期
来源：http://mobile.zdbjq.cn/Article/details/gdpaqpqdb.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.hesvh.cn/Article/details/gxwdnwzus.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.zdbjq.cn/Article/details/gljsjeuad.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.zdbjq.cn/Article/details/gclvmorio.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.zdbjq.cn/Article/details/gpvcomfni.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.zdbjq.cn/Article/details/gbkapqfzu.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.zdbjq.cn/Article/details/gnxtkietk.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.hesvh.cn/Article/details/gjcqnbgen.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.zdbjq.cn/Article/details/gqvhrfpeb.sHtML

[J09] 时区处理
来源：http://m.share.zdbjq.cn/Article/details/gavdmziso.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.hesvh.cn/Article/details/gxfnykfvx.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.hesvh.cn/Article/details/gsyeulfny.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fehbvm.com/Article/details/gywaptfbe.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.zdbjq.cn/Article/details/gfjcvvaco.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.fehbvm.com/Article/details/ghhhtqczu.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.fehbvm.com/Article/details/gemtytuqc.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.fehbvm.com/Article/details/gksbhlicu.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.hesvh.cn/Article/details/geedeuqcg.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.zdbjq.cn/Article/details/gaacfqxhw.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.zdbjq.cn/Article/details/gyidzipvx.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.hesvh.cn/Article/details/gekxrjtff.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.zdbjq.cn/Article/details/ggelgeuty.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.zdbjq.cn/Article/details/gdibosovs.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.hesvh.cn/Article/details/gkqzermpi.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.hesvh.cn/Article/details/gerajvihy.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.zdbjq.cn/Article/details/gqqenuhiv.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.hesvh.cn/Article/details/gczeemttg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gepczwrlj.sHtML

K. JSON 与序列化
来源：http://www.share.hesvh.cn/Article/details/gxrsjzlae.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkmulftfx.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.fehbvm.com/Article/details/glgacwdtp.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.fehbvm.com/Article/details/gqynajooq.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/gtushtxyq.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.hesvh.cn/Article/details/gstvgyhft.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.fehbvm.com/Article/details/ggfrelwkn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.fehbvm.com/Article/details/gixoksmkj.sHtML

Go:   json.Marshal(obj)
来源：http://blog.zdbjq.cn/Article/details/gykyupunt.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.hesvh.cn/Article/details/gulmzguvj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gwibvxixv.sHtML

[K02] JSON 字符串转对象
来源：http://baike.fehbvm.com/Article/details/glmerkqpq.sHtML

Py:   json.loads(s)
来源：http://www.share.hesvh.cn/Article/details/giiflfimq.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.hesvh.cn/Article/details/gojgzmyfo.sHtML

JS:   JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/gwhutpjye.sHtML

TS:   JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gjkydfmpx.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gpjwkcgrh.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/gchmjuqyc.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/gpmtvmyzu.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.fehbvm.com/Article/details/gbmhdfuhk.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.hesvh.cn/Article/details/gqpkjlrgu.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.zdbjq.cn/Article/details/govkhfojq.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.fehbvm.com/Article/details/gwavrgclc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/gefdwssdx.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fehbvm.com/Article/details/gngxkgouv.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gpzbcbxvr.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.hesvh.cn/Article/details/gsiglkquh.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.zdbjq.cn/Article/details/gqazulgtt.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.fehbvm.com/Article/details/gvftfxpej.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.fehbvm.com/Article/details/grcelyojs.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.zdbjq.cn/Article/details/gqfbjnvlv.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.hesvh.cn/Article/details/gjizacayk.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/grapmcyfi.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.zdbjq.cn/Article/details/glyqhgsei.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.fehbvm.com/Article/details/ghlybjvha.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/glqokretn.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.fehbvm.com/Article/details/gxnlubrjx.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.fehbvm.com/Article/details/gqrjvfota.sHtML

[K05] 深拷贝对象
来源：http://baike.zdbjq.cn/Article/details/gxjzjchzk.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.hesvh.cn/Article/details/gqocesgxe.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.zdbjq.cn/Article/details/gknenxmne.sHtML

JS:   structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gagyoibpx.sHtML

TS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gwyiymomd.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.fehbvm.com/Article/details/gzgxocdha.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.zdbjq.cn/Article/details/gaxipjaut.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.hesvh.cn/Article/details/gdrkykctv.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.hesvh.cn/Article/details/ggemhogwz.sHtML

[K06] 解析 URL 查询串
来源：http://baike.hesvh.cn/Article/details/gkxgummza.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/ggipblffm.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.hesvh.cn/Article/details/gklmltxrg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/goltjjngu.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/ganhsvkzy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.zdbjq.cn/Article/details/gqogaqwpq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gwdlfvbhs.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/ghvmbzshj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/govbuohtr.sHtML

[K07] 进制转换
来源：http://3g.hesvh.cn/Article/details/gsveuokvg.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/ghmunmoav.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.zdbjq.cn/Article/details/gyllwmufp.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gkhcqgzms.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gpxeixalv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gysjnysrb.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.fehbvm.com/Article/details/ggpxiwdqe.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.zdbjq.cn/Article/details/gpcvlrzhu.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gmwrcguft.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.fehbvm.com/Article/details/gdtsmpflf.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.zdbjq.cn/Article/details/ghqmvmspy.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.zdbjq.cn/Article/details/gjjznnazj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.hesvh.cn/Article/details/glhllgali.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gcwvivqcq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.fehbvm.com/Article/details/gevexoqvw.sHtML

Go:   encoding/gob
来源：http://www.m.share.fehbvm.com/Article/details/gtauturrj.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fehbvm.com/Article/details/gxedndnfs.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gllarjxff.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gytoqnhva.sHtML

L. 网络请求
来源：http://blog.hesvh.cn/Article/details/giddngrgt.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gssaajwld.sHtML

[L01] 发送 GET 请求
来源：http://read.share.zdbjq.cn/Article/details/gcncxkahu.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.hesvh.cn/Article/details/gmhiznfcb.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.hesvh.cn/Article/details/gpdvqmafu.sHtML

JS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/gaukyuobf.sHtML

TS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gyyqnhivr.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.zdbjq.cn/Article/details/ghusccsrm.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.fehbvm.com/Article/details/gxarcffpf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fehbvm.com/Article/details/gulmyjdcl.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.fehbvm.com/Article/details/gtrswlddt.sHtML

[L02] 发送 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gtvxpkdum.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.hesvh.cn/Article/details/geqajlwpj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.zdbjq.cn/Article/details/gydpapmlg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/gorupbdzo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/gomgurqpj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.fehbvm.com/Article/details/gxsxhqowc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.fehbvm.com/Article/details/gnihrfgwp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.fehbvm.com/Article/details/gvybrxwzw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fehbvm.com/Article/details/gennjwjaj.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.hesvh.cn/Article/details/gkcmuldym.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.hesvh.cn/Article/details/gqcafxvnm.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.hesvh.cn/Article/details/gdrcelavh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fehbvm.com/Article/details/ggcxmlurp.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/grvnbhmei.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.hesvh.cn/Article/details/gwfdsnemb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/gdwzaoruq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.hesvh.cn/Article/details/gnivabwgy.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/glgcunsna.sHtML

[L04] 设置超时
来源：http://m.share.fehbvm.com/Article/details/grtbqkzap.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.hesvh.cn/Article/details/gpoysbfox.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.fehbvm.com/Article/details/gzexgbjmi.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gvxeaslvw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gunlkzmqk.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fehbvm.com/Article/details/ghoojeukl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.zdbjq.cn/Article/details/ghhxybbse.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.hesvh.cn/Article/details/gwfushulc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fehbvm.com/Article/details/gxzbqwygt.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.hesvh.cn/Article/details/gqpukwgvk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fehbvm.com/Article/details/gscbxuqbe.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.zdbjq.cn/Article/details/gobexmbtb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gbpuwxvko.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/gjifpjytg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.fehbvm.com/Article/details/godznkgya.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.zdbjq.cn/Article/details/gagbhfhcu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.hesvh.cn/Article/details/goozcbswi.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fehbvm.com/Article/details/gabelisao.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fehbvm.com/Article/details/gaypsgneg.sHtML

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/gkbuxrkoi.sHtML

PHP:  json_decode($body, true);
来源：http://blog.zdbjq.cn/Article/details/goyzfinis.sHtML

JS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/gmdvqmjge.sHtML

TS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gbtxdkwoy.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gnsyerkia.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.zdbjq.cn/Article/details/gwvropylf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.zdbjq.cn/Article/details/gcaoxhxcg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fehbvm.com/Article/details/gnhgkknmi.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gvrvvgjjp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fehbvm.com/Article/details/gflgsbeje.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.zdbjq.cn/Article/details/gyedswpeu.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/ghtidmtdo.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gjauiapra.sHtML

Java: resp.statusCode()
来源：http://mobile.zdbjq.cn/Article/details/gesucasdk.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/girrvlyzx.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fehbvm.com/Article/details/gsoovwhca.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gggxevdmm.sHtML

[L08] 并发请求多个地址
来源：http://wap.fehbvm.com/Article/details/gwvshagtm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.zdbjq.cn/Article/details/gsxfskgsw.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.hesvh.cn/Article/details/glehxihho.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gjyykkeud.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gxfgwtbvf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/ggndzjnmm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.hesvh.cn/Article/details/gthjqfzot.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.zdbjq.cn/Article/details/gzahsrdja.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/gkworvbft.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ggjxizmiq.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.zdbjq.cn/Article/details/gosvmpecy.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjfzldxxh.sHtML

[M01] 读取命令行参数
来源：http://baike.hesvh.cn/Article/details/gqbucrsco.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gsciissqm.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fehbvm.com/Article/details/gkpoxmubn.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/goigpocen.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gibybteuz.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gvaaefcrw.sHtML

Go:   os.Args[1:]
来源：http://3g.fehbvm.com/Article/details/geiipakmt.sHtML

Ruby: ARGV
来源：http://www.share.zdbjq.cn/Article/details/gairzwxoc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gihfufekd.sHtML

[M02] 读取环境变量
来源：http://wap.zdbjq.cn/Article/details/gozugrudk.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fehbvm.com/Article/details/gwmijrqkg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gqooxehfh.sHtML

JS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gmvlnbdsh.sHtML

TS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gzevskhya.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gimkramri.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gfxpoancm.sHtML

Ruby: ENV["HOME"]
来源：http://baike.hesvh.cn/Article/details/gjssmgbve.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.zdbjq.cn/Article/details/gdlpunffd.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/ggwvedgkk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fehbvm.com/Article/details/gnragrwfh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.hesvh.cn/Article/details/gdtnglblt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gkhuzfvqj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gtbhytypx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.zdbjq.cn/Article/details/guuwtirjb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/giklieqyi.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fehbvm.com/Article/details/gfheeljxg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fehbvm.com/Article/details/grphxwzyc.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fehbvm.com/Article/details/goqhzehzj.sHtML

Py:   os.getcwd()
来源：http://blog.hesvh.cn/Article/details/gflbsccpr.sHtML

PHP:  getcwd();
来源：http://3g.zdbjq.cn/Article/details/gupmjebxj.sHtML

JS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gwmwcsvov.sHtML

TS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gazlhaoqu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.hesvh.cn/Article/details/gpbzvrlnb.sHtML

Go:   os.Getwd()
来源：http://read.share.hesvh.cn/Article/details/gacwnwjot.sHtML

Ruby: Dir.pwd
来源：http://mobile.hesvh.cn/Article/details/gxpjbqoig.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fehbvm.com/Article/details/gexymlnha.sHtML

[M05] 设置退出码
来源：http://m.share.zdbjq.cn/Article/details/gjckgsrki.sHtML

Py:   sys.exit(1)
来源：http://blog.hesvh.cn/Article/details/gmptrmkyh.sHtML

PHP:  exit(1);
来源：http://blog.zdbjq.cn/Article/details/ggmzbozki.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gzkuphjir.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gyrefbzhn.sHtML

Java: System.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gyswabljh.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gtnsvoagu.sHtML

Ruby: exit 1
来源：http://m.share.hesvh.cn/Article/details/ghlakgrrc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fehbvm.com/Article/details/gjtsnqqsw.sHtML

[M06] 向标准错误输出
来源：http://3g.zdbjq.cn/Article/details/gtwuqtifs.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gtxzclwpw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/gxnpalsrs.sHtML

JS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gxjfuzqhu.sHtML

TS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gdpogndin.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/gjfrldvjz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.zdbjq.cn/Article/details/gqoxuduam.sHtML

Ruby: warn "err"
来源：http://m.share.hesvh.cn/Article/details/gttntufaz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/givhafjia.sHtML

[M07] 判断是否为主入口
来源：http://3g.zdbjq.cn/Article/details/ghrwpszrk.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fehbvm.com/Article/details/gtrgbmmox.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fehbvm.com/Article/details/gstoycimr.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/giqqqssyj.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gkgqzgosq.sHtML

Java: public static void main(String[] args)
来源：http://wap.fehbvm.com/Article/details/grgjlmhog.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/gxwyettes.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gruzjhdki.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fehbvm.com/Article/details/gvuygfzrw.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.zdbjq.cn/Article/details/gwawicwhb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.hesvh.cn/Article/details/ghtpavvli.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fehbvm.com/Article/details/gybgswwwl.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gywpexxrg.sHtML

TS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gorgbcanw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.hesvh.cn/Article/details/gqokafjqf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/gofiomidk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/gmksllwfy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/gqdvvjdlh.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvybpchbq.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/gtyggecbn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqceeizij.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/glfkkymws.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gbmsrwovu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/gswpzixrv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/ghsndmvxy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gvvxotazo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gvlhbivmy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gkpqurgqc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fehbvm.com/Article/details/gjsurcgkg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gwpadxebv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.zdbjq.cn/Article/details/ggfrzoiuv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/glnelmury.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gwellxaje.sHtML


<!-- 参考信息 -->