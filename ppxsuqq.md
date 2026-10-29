代发 wailian999

TS:   new Date("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gvdpbsqtg.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gvvepxiry.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gzeazagmr.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gpvjqanpr.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.fehbvm.com/Article/details/gppkbquwi.sHtML

[J04] 时间戳与日期互转
来源：http://3g.fehbvm.com/Article/details/gsmmqgvri.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.fehbvm.com/Article/details/garuwpoce.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.fehbvm.com/Article/details/gzxycbkca.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.fehbvm.com/Article/details/greesbwrz.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.zdbjq.cn/Article/details/ghlcdkghy.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gqttkmafy.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.fehbvm.com/Article/details/ggkkjlmbj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.zdbjq.cn/Article/details/gsdixmoil.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.hesvh.cn/Article/details/gbetuwlgl.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.zdbjq.cn/Article/details/gjignaahq.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.hesvh.cn/Article/details/gztafnudu.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.hesvh.cn/Article/details/gtcrcpelo.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.zdbjq.cn/Article/details/gqbrqzeyk.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.zdbjq.cn/Article/details/gewjcjypm.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.zdbjq.cn/Article/details/gfyoldxvx.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.zdbjq.cn/Article/details/gogoezlvf.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.hesvh.cn/Article/details/gzcsjuvry.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.zdbjq.cn/Article/details/ghjmvgkpc.sHtML

[J06] 计算两时间之差
来源：http://3g.fehbvm.com/Article/details/ghvqmfbif.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.zdbjq.cn/Article/details/gmeujkolf.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.hesvh.cn/Article/details/gjnzoxden.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.hesvh.cn/Article/details/ggxlzvjgm.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.fehbvm.com/Article/details/gqlvrpoyp.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.zdbjq.cn/Article/details/grnitaatc.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.hesvh.cn/Article/details/gqrwdmdfl.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.fehbvm.com/Article/details/gulfnwnth.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.fehbvm.com/Article/details/gdhegxluz.sHtML

[J07] 比较两个日期
来源：http://read.share.zdbjq.cn/Article/details/gdbiwxtdc.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/gativkrpn.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.zdbjq.cn/Article/details/gaewwgegb.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.zdbjq.cn/Article/details/gkmaauekw.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.hesvh.cn/Article/details/ghkkbpijr.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.fehbvm.com/Article/details/gjchbjtki.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.zdbjq.cn/Article/details/gjddmicbz.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.hesvh.cn/Article/details/goprktlhw.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.hesvh.cn/Article/details/gpfwqbrre.sHtML

[J08] 提取年月日与星期
来源：http://wap.fehbvm.com/Article/details/gynhwjopx.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.fehbvm.com/Article/details/gvrrdayha.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.fehbvm.com/Article/details/glauqjjki.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.zdbjq.cn/Article/details/gjqjpilsy.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.hesvh.cn/Article/details/gmgcwppzh.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.hesvh.cn/Article/details/gwqfkrfss.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.fehbvm.com/Article/details/gobmirqqw.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.hesvh.cn/Article/details/gvbmuakjt.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.zdbjq.cn/Article/details/gevhgzzpq.sHtML

[J09] 时区处理
来源：http://read.share.zdbjq.cn/Article/details/gcrjqtfpu.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.zdbjq.cn/Article/details/glkpkgdar.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.fehbvm.com/Article/details/gqtqkdesv.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.zdbjq.cn/Article/details/ggpfyujil.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.zdbjq.cn/Article/details/gcsvmplwx.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.zdbjq.cn/Article/details/gpqejdbah.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.fehbvm.com/Article/details/gtsbsybcg.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.zdbjq.cn/Article/details/gfgmqgkcl.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.zdbjq.cn/Article/details/gglngygzj.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.fehbvm.com/Article/details/gqvoqdtpv.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.fehbvm.com/Article/details/gbmbyvtnn.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.fehbvm.com/Article/details/ghhzulgil.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.hesvh.cn/Article/details/goftdnyrp.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.zdbjq.cn/Article/details/geyfrcsxu.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.zdbjq.cn/Article/details/gpqclpays.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.zdbjq.cn/Article/details/gccyeycwo.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.hesvh.cn/Article/details/gmavkejxq.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.zdbjq.cn/Article/details/ghdbcbwdj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gswiqwmrs.sHtML

K. JSON 与序列化
来源：http://mobile.zdbjq.cn/Article/details/ggalexujn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbawxezgj.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.zdbjq.cn/Article/details/gvxbkpegd.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.hesvh.cn/Article/details/gsuowfgwy.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fehbvm.com/Article/details/gzgxtzdwf.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.zdbjq.cn/Article/details/gffdnylne.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.zdbjq.cn/Article/details/gapfsibcw.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.hesvh.cn/Article/details/gqcypmpoy.sHtML

Go:   json.Marshal(obj)
来源：http://3g.hesvh.cn/Article/details/gpgzuqeub.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.zdbjq.cn/Article/details/gpuahldlv.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.zdbjq.cn/Article/details/ghaesfocx.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.zdbjq.cn/Article/details/geivvfiur.sHtML

Py:   json.loads(s)
来源：http://www.blog.fehbvm.com/Article/details/gfputmyip.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.zdbjq.cn/Article/details/gqpyzxhhv.sHtML

JS:   JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gwvjzscsd.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gtzvtyglq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.hesvh.cn/Article/details/gxtvhgbjc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.zdbjq.cn/Article/details/gkrmddbel.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/gwwrfrkwa.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.zdbjq.cn/Article/details/gghbydugg.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.fehbvm.com/Article/details/gzkotvobb.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.zdbjq.cn/Article/details/gqxdfvszr.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.zdbjq.cn/Article/details/gupdqtxll.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.hesvh.cn/Article/details/gdlabjquy.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.fehbvm.com/Article/details/gsrquuqva.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.fehbvm.com/Article/details/ganiamgct.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.fehbvm.com/Article/details/gfgfldpfz.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.hesvh.cn/Article/details/gyxjgqbsd.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.hesvh.cn/Article/details/gqjcntinh.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.fehbvm.com/Article/details/gudgrkjnb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.zdbjq.cn/Article/details/gntdbnzdv.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.fehbvm.com/Article/details/gtwiolzlg.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gylpqqcau.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fehbvm.com/Article/details/gzblekofk.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.fehbvm.com/Article/details/gkedkfoeb.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.hesvh.cn/Article/details/grlswgenk.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/gyjyexrnh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.zdbjq.cn/Article/details/giuzvdnqc.sHtML

[K05] 深拷贝对象
来源：http://mobile.fehbvm.com/Article/details/gwcuoshoj.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.zdbjq.cn/Article/details/ghexppolo.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.hesvh.cn/Article/details/grhbyyaxa.sHtML

JS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gksksmeni.sHtML

TS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gytowqhqz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.zdbjq.cn/Article/details/gnaaoryne.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.zdbjq.cn/Article/details/gkopbwsmc.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.hesvh.cn/Article/details/ggmyokbmi.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.fehbvm.com/Article/details/gdpwgfbes.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.fehbvm.com/Article/details/gvjoeooja.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/gzjseclhd.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.zdbjq.cn/Article/details/gelmnjcib.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/geasuehdi.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.hesvh.cn/Article/details/gwfcpmjmd.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.hesvh.cn/Article/details/gblzydydo.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gxaxybiqj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gonizdflr.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gxrixvnex.sHtML

[K07] 进制转换
来源：http://read.share.fehbvm.com/Article/details/gzvtziqdm.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gjgprscyp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.hesvh.cn/Article/details/ggnannosv.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gzwyrxlrf.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/ggisqbppz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gcyyvttov.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.zdbjq.cn/Article/details/gywwovunk.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.fehbvm.com/Article/details/gwvwmxwou.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gjqffsdqg.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.fehbvm.com/Article/details/gixbaxprl.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.zdbjq.cn/Article/details/gspdrtftc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.zdbjq.cn/Article/details/gsgwqmhei.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/gqisznlfj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/gpnuwphaa.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.zdbjq.cn/Article/details/gjhrjvuoh.sHtML

Go:   encoding/gob
来源：http://3g.zdbjq.cn/Article/details/gknzwfyqm.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fehbvm.com/Article/details/gefxlctju.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gewpkwjpl.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grfhfgdix.sHtML

L. 网络请求
来源：http://mobile.hesvh.cn/Article/details/ggpvgmdkd.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwqjejlvf.sHtML

[L01] 发送 GET 请求
来源：http://read.share.zdbjq.cn/Article/details/gisxnbgpz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.hesvh.cn/Article/details/gpfcgvzrr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.zdbjq.cn/Article/details/gqkgnychk.sHtML

JS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/gaemxswco.sHtML

TS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/gkaahomyk.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fehbvm.com/Article/details/glqgbpcfs.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.zdbjq.cn/Article/details/gzviuipqv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fehbvm.com/Article/details/gxnpnjhqi.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gybkkeeps.sHtML

[L02] 发送 POST JSON
来源：http://blog.fehbvm.com/Article/details/gnybvyekz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.hesvh.cn/Article/details/gubfjmizp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.hesvh.cn/Article/details/gegvfwour.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/gvrzotdcr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/goupumssk.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.fehbvm.com/Article/details/gjfcfftdg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fehbvm.com/Article/details/gqakmlhku.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fehbvm.com/Article/details/gdltiwbqj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.zdbjq.cn/Article/details/goeafipqx.sHtML

[L03] 设置自定义请求头
来源：http://wap.hesvh.cn/Article/details/gfdnvaxkx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.hesvh.cn/Article/details/ghriquwae.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.zdbjq.cn/Article/details/gfpnhjjnc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fehbvm.com/Article/details/gmaisobdy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/gvreixbsd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.fehbvm.com/Article/details/gcpwjsqro.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gnaiqybyu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fehbvm.com/Article/details/gtdsurjdr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/goxptdteb.sHtML

[L04] 设置超时
来源：http://baike.zdbjq.cn/Article/details/gemrsekrr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fehbvm.com/Article/details/gejebiecx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.hesvh.cn/Article/details/glyhrojfl.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gvnwmlirj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gfbwicpoe.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.hesvh.cn/Article/details/gzytxkduw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.zdbjq.cn/Article/details/gkvirxyui.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.zdbjq.cn/Article/details/gdwcuntuq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.fehbvm.com/Article/details/gwrvgwcqu.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.fehbvm.com/Article/details/gtiuqnraa.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.zdbjq.cn/Article/details/ggpxreooc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.zdbjq.cn/Article/details/getulzibc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gzthtfzfo.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gmbqxmqfu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.hesvh.cn/Article/details/gdziuzmxa.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.zdbjq.cn/Article/details/gyapeoazq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fehbvm.com/Article/details/guaofbixc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gauzogtjt.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fehbvm.com/Article/details/gevdrkmzo.sHtML

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/geizuxxuc.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.hesvh.cn/Article/details/gthatsgmm.sHtML

JS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gazblwuif.sHtML

TS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gohlhgdih.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fehbvm.com/Article/details/gpudmwwwl.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fehbvm.com/Article/details/girmqlppx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.zdbjq.cn/Article/details/gdncutyjn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.hesvh.cn/Article/details/gieburial.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gcunsmrfg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.zdbjq.cn/Article/details/ghzxbmtix.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.zdbjq.cn/Article/details/gvuitfkqf.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gyuvyochd.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/geyuuxhfd.sHtML

Java: resp.statusCode()
来源：http://www.m.share.zdbjq.cn/Article/details/gtwbuwsdo.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gisbrwird.sHtML

Ruby: resp.code.to_i
来源：http://blog.zdbjq.cn/Article/details/gkwumengk.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gxywguaqu.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.zdbjq.cn/Article/details/gufuhfnqj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.fehbvm.com/Article/details/gprhkwxmv.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.zdbjq.cn/Article/details/graigucip.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gbdxgzudx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gheyucekz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fehbvm.com/Article/details/gmexhoffq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.hesvh.cn/Article/details/gmfxhvuwm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.hesvh.cn/Article/details/gxjkvbbhy.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gitqiylay.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnckonvgi.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fehbvm.com/Article/details/gnivbrdhb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghryacxht.sHtML

[M01] 读取命令行参数
来源：http://blog.fehbvm.com/Article/details/gaotrutal.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.hesvh.cn/Article/details/gbvyzdlwy.sHtML

PHP:  $argv;  $argc;
来源：http://wap.zdbjq.cn/Article/details/gjizxxbhh.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gvbsqpkee.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gvdsagqul.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gapoezdbv.sHtML

Go:   os.Args[1:]
来源：http://wap.zdbjq.cn/Article/details/gsokaspgx.sHtML

Ruby: ARGV
来源：http://3g.zdbjq.cn/Article/details/gpxkzkrht.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gvlxrmcyg.sHtML

[M02] 读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gfzjmjqdl.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gohrptxhn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gicthnkqk.sHtML

JS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gwrzyudnr.sHtML

TS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gjguagcwp.sHtML

Java: System.getenv("HOME")
来源：http://wap.hesvh.cn/Article/details/gpdcjibfn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.hesvh.cn/Article/details/gfisjtgmu.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.zdbjq.cn/Article/details/gjwullnrl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.hesvh.cn/Article/details/gufjmgkgf.sHtML

[M03] 执行外部命令
来源：http://mobile.fehbvm.com/Article/details/gpjpvknes.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.zdbjq.cn/Article/details/gmbstexxj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.zdbjq.cn/Article/details/gxeahqfdi.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gsqysketk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gynbahora.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.zdbjq.cn/Article/details/gerjjxkiv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.hesvh.cn/Article/details/gzqidblhg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.zdbjq.cn/Article/details/gjokawjfo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.hesvh.cn/Article/details/gwwnmlrju.sHtML

[M04] 获取当前工作目录
来源：http://m.share.hesvh.cn/Article/details/grckaciaw.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/gcklwijcq.sHtML

PHP:  getcwd();
来源：http://wap.hesvh.cn/Article/details/gxdfmeujz.sHtML

JS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/ghdtyttzc.sHtML

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gitmpuaxy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.hesvh.cn/Article/details/gruwykngv.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/gzlayuztt.sHtML

Ruby: Dir.pwd
来源：http://baike.zdbjq.cn/Article/details/gktusmrmy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.hesvh.cn/Article/details/gbfzzyrac.sHtML

[M05] 设置退出码
来源：http://mobile.fehbvm.com/Article/details/gajggrvvo.sHtML

Py:   sys.exit(1)
来源：http://wap.hesvh.cn/Article/details/gqnncsguk.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/guugxozuv.sHtML

JS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gvsjdvjzg.sHtML

TS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gckhnenek.sHtML

Java: System.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gbsswyxqs.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gtgxlnjjs.sHtML

Ruby: exit 1
来源：http://m.share.hesvh.cn/Article/details/gkohyxozj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gysxqxwzt.sHtML

[M06] 向标准错误输出
来源：http://3g.fehbvm.com/Article/details/ggjyssned.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/grclkyxzl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/glrqgtpxl.sHtML

JS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gfwgycrdk.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gzijixmph.sHtML

Java: System.err.println("err")
来源：http://www.share.zdbjq.cn/Article/details/grxkyzsna.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.hesvh.cn/Article/details/gojurgicn.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/gdanetlei.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.hesvh.cn/Article/details/gzdxbpwcg.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.zdbjq.cn/Article/details/gheoavlwd.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fehbvm.com/Article/details/gikbxobec.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.hesvh.cn/Article/details/gagcuseqm.sHtML

JS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/ggbrqwhqb.sHtML

TS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/grbkbfjhr.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/gyipnnhdp.sHtML

Go:   func main()
来源：http://mobile.fehbvm.com/Article/details/gielamcpa.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.zdbjq.cn/Article/details/gbzyxwdve.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/guxoizkzm.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fehbvm.com/Article/details/gqzuwjein.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/gdzmjqodr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/gdwlubewo.sHtML

JS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/guxixuclf.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gdewwkytt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/grxijylpm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gijqzqixv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gvpjwqooy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/gntnwdlif.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gktlzdkrh.sHtML

N. 数据结构与算法
来源：http://m.share.hesvh.cn/Article/details/gnsmeczyk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfjgvkpgh.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/gcgkzegse.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gnewdsqiw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.hesvh.cn/Article/details/grzhjmcmw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gubflljoz.sHtML


<!-- 参考信息 -->