代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.fehbvm.com/Article/details/gebksnmbq.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.hesvh.cn/Article/details/gvllpcuvl.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.fehbvm.com/Article/details/gylfofbmv.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.fehbvm.com/Article/details/glanvxmwq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.hesvh.cn/Article/details/gmbahlwyb.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.zdbjq.cn/Article/details/gklexpdgc.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.zdbjq.cn/Article/details/grtjpzpnq.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.hesvh.cn/Article/details/gnssjlnxr.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.zdbjq.cn/Article/details/goizhfpam.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.fehbvm.com/Article/details/gewemacof.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.fehbvm.com/Article/details/gmylitatv.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.zdbjq.cn/Article/details/gwpqetwvz.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.zdbjq.cn/Article/details/gujshjgnl.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fehbvm.com/Article/details/glddjldjk.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.hesvh.cn/Article/details/gkurnrope.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.zdbjq.cn/Article/details/gokhujtri.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.hesvh.cn/Article/details/gugdrewqq.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.zdbjq.cn/Article/details/gmiarxxtk.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.zdbjq.cn/Article/details/ggcwbbsla.sHtML

[J06] 计算两时间之差
来源：http://baike.hesvh.cn/Article/details/gtvavnwld.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.zdbjq.cn/Article/details/glkfsfkux.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.fehbvm.com/Article/details/gfqtwgghz.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.hesvh.cn/Article/details/grljaabna.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.zdbjq.cn/Article/details/gfbkudege.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.hesvh.cn/Article/details/gjpsscweg.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.hesvh.cn/Article/details/geejlotal.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.fehbvm.com/Article/details/gazhypxrm.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.hesvh.cn/Article/details/gkxawddss.sHtML

[J07] 比较两个日期
来源：http://www.m.share.hesvh.cn/Article/details/gnwkkxnhx.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.hesvh.cn/Article/details/ggayddjmr.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.hesvh.cn/Article/details/gtxslarjq.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.zdbjq.cn/Article/details/gvgjalrjn.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.hesvh.cn/Article/details/gcpfvbesv.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.fehbvm.com/Article/details/gfbytqmxt.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.hesvh.cn/Article/details/gtkncoihx.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.hesvh.cn/Article/details/gbgqzsbkz.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/gqojqfchz.sHtML

[J08] 提取年月日与星期
来源：http://wap.zdbjq.cn/Article/details/giplxsdty.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.zdbjq.cn/Article/details/gmdvndpkj.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.zdbjq.cn/Article/details/gehzfzpwb.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.fehbvm.com/Article/details/gbexucjdq.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.hesvh.cn/Article/details/gqyzmppwo.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.fehbvm.com/Article/details/gtjxcoxmw.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.zdbjq.cn/Article/details/gyedcocvf.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.hesvh.cn/Article/details/gflvtnncw.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.fehbvm.com/Article/details/gidvntnio.sHtML

[J09] 时区处理
来源：http://m.share.zdbjq.cn/Article/details/gcmsnvqsw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.zdbjq.cn/Article/details/giloyvgpb.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.fehbvm.com/Article/details/gyrltimua.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fehbvm.com/Article/details/gneztetir.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.hesvh.cn/Article/details/gcwlhpati.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.zdbjq.cn/Article/details/gmaqfcjrm.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.hesvh.cn/Article/details/gdngbzbwj.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.fehbvm.com/Article/details/gdjdkvqqv.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.fehbvm.com/Article/details/gzsurigtt.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.fehbvm.com/Article/details/gavhfegpv.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.zdbjq.cn/Article/details/ghjtespcd.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.zdbjq.cn/Article/details/gclgqytwe.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.zdbjq.cn/Article/details/gusxtenrm.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.hesvh.cn/Article/details/gbkehkgcd.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.zdbjq.cn/Article/details/gphfwovrt.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.fehbvm.com/Article/details/gfdpooaph.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.fehbvm.com/Article/details/gnxiprmsd.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.fehbvm.com/Article/details/ggeppnykg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghconljqn.sHtML

K. JSON 与序列化
来源：http://wap.fehbvm.com/Article/details/gymtovezt.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxqqlzamz.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.zdbjq.cn/Article/details/gdnnvugsk.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.fehbvm.com/Article/details/gbfrigqrp.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.zdbjq.cn/Article/details/gdgbjthuv.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.fehbvm.com/Article/details/gayklgkix.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gidzmowna.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.zdbjq.cn/Article/details/gtzznvrtk.sHtML

Go:   json.Marshal(obj)
来源：http://baike.fehbvm.com/Article/details/grndaooew.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.hesvh.cn/Article/details/grzgmvrzh.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.zdbjq.cn/Article/details/gokijxstu.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.hesvh.cn/Article/details/gbrdzwoyc.sHtML

Py:   json.loads(s)
来源：http://wap.zdbjq.cn/Article/details/gogfdwnxh.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.zdbjq.cn/Article/details/gfbirtvgb.sHtML

JS:   JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/gtsjdccjg.sHtML

TS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gwpgnmhek.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.hesvh.cn/Article/details/gknbugzet.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.fehbvm.com/Article/details/gztfqnict.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/glcnkgxkl.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.hesvh.cn/Article/details/guqqcxjmg.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.zdbjq.cn/Article/details/givhqfyza.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.zdbjq.cn/Article/details/ggfluoaam.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.hesvh.cn/Article/details/giosfloob.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.fehbvm.com/Article/details/gzwttbfqi.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/giujjkpdy.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.fehbvm.com/Article/details/gtwhhkdzu.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fehbvm.com/Article/details/gkfwmjfiw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.zdbjq.cn/Article/details/gndfvcifl.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.zdbjq.cn/Article/details/gxgrbmrkj.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.zdbjq.cn/Article/details/gjuxhpieu.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.hesvh.cn/Article/details/gyufcnsmo.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.hesvh.cn/Article/details/gfiypuksz.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fehbvm.com/Article/details/gfusrgjvj.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.hesvh.cn/Article/details/gnxbguvnm.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/giwyqmtez.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.zdbjq.cn/Article/details/gzgvbtodp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.hesvh.cn/Article/details/gezfesuar.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.hesvh.cn/Article/details/ghrwhkpqq.sHtML

[K05] 深拷贝对象
来源：http://mobile.zdbjq.cn/Article/details/gcleersfa.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.hesvh.cn/Article/details/gxoyegeht.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.fehbvm.com/Article/details/gqqwfimfa.sHtML

JS:   structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gkfghquay.sHtML

TS:   structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gpyigtcbu.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.zdbjq.cn/Article/details/gfartxakw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.hesvh.cn/Article/details/gddgxmhin.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.zdbjq.cn/Article/details/goyhqoggd.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.zdbjq.cn/Article/details/gsossagwd.sHtML

[K06] 解析 URL 查询串
来源：http://3g.fehbvm.com/Article/details/giapxzpkp.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/gbhzltwzx.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.fehbvm.com/Article/details/gdeowafms.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.zdbjq.cn/Article/details/gdqjbwjah.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/gzujnoiop.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.fehbvm.com/Article/details/gqzxzvset.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gllrommfu.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gmpygpecj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gjcclqwgm.sHtML

[K07] 进制转换
来源：http://m.share.zdbjq.cn/Article/details/grddorbbz.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gdcmielin.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.hesvh.cn/Article/details/ggyilpbxh.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gqzxgcsxw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gyflrtqca.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gxpiykjmj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.hesvh.cn/Article/details/gtduhsjkp.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fehbvm.com/Article/details/grqpdvieb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gtjxzmrjs.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.hesvh.cn/Article/details/gzvcnemen.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.zdbjq.cn/Article/details/ggclpymaf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.hesvh.cn/Article/details/gksruejup.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gnluxfjpj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/gbflofzij.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.zdbjq.cn/Article/details/gjseshtdc.sHtML

Go:   encoding/gob
来源：http://m.share.zdbjq.cn/Article/details/gbzkrznni.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.zdbjq.cn/Article/details/gftuptsow.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gljtbsgkj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gaskxleuo.sHtML

L. 网络请求
来源：http://read.share.fehbvm.com/Article/details/gekrripfa.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyptkfnjh.sHtML

[L01] 发送 GET 请求
来源：http://read.share.hesvh.cn/Article/details/gzkycckia.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.zdbjq.cn/Article/details/gymdriyoe.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.hesvh.cn/Article/details/gubeqlwfk.sHtML

JS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gfueqzhew.sHtML

TS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/ggfyxrytn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.hesvh.cn/Article/details/gqepktsvt.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.hesvh.cn/Article/details/gdtlivcjy.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.zdbjq.cn/Article/details/gqnebuvzm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.hesvh.cn/Article/details/gjkwgffhz.sHtML

[L02] 发送 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gxntqsiqa.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/gfgekptih.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.fehbvm.com/Article/details/gqpdhtiwc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gxzunlxke.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/gqyvgdnmi.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.hesvh.cn/Article/details/gcvrelavi.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.hesvh.cn/Article/details/gqkyeljok.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.hesvh.cn/Article/details/gptvtjcfg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.zdbjq.cn/Article/details/gfixpieuu.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/gyaormgup.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fehbvm.com/Article/details/gvrggzezk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.fehbvm.com/Article/details/gywuwwldf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gdxfbdetz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/getygderu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.hesvh.cn/Article/details/ggsvtgdfl.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gutsxlxnz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fehbvm.com/Article/details/gfugothpr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gxqiidlab.sHtML

[L04] 设置超时
来源：http://www.share.fehbvm.com/Article/details/glwtextwo.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.fehbvm.com/Article/details/gnjjmhycz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.hesvh.cn/Article/details/gwvzpiljn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.hesvh.cn/Article/details/gyhimkwip.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gzssbaboo.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.zdbjq.cn/Article/details/gvzxleeig.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.hesvh.cn/Article/details/ghiwswvdf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.zdbjq.cn/Article/details/glfkbyyrs.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.hesvh.cn/Article/details/gpjmptxxx.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.fehbvm.com/Article/details/gyoutrwjp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.zdbjq.cn/Article/details/gmplpgywb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fehbvm.com/Article/details/gmufpmhot.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gyzuscges.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gshpzacma.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.hesvh.cn/Article/details/gsfaacqhi.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fehbvm.com/Article/details/gprjlsuko.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.hesvh.cn/Article/details/gbhdivwhe.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.zdbjq.cn/Article/details/gcsknpjat.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.fehbvm.com/Article/details/gkbwevyby.sHtML

Py:   resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/goyxqligl.sHtML

PHP:  json_decode($body, true);
来源：http://3g.hesvh.cn/Article/details/gxdduduql.sHtML

JS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/greobniwu.sHtML

TS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gbbgrtmwk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fehbvm.com/Article/details/ggdzohjuh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.zdbjq.cn/Article/details/guagdgytf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.zdbjq.cn/Article/details/gydsgfjoq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.hesvh.cn/Article/details/gfpllgbjd.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gjxydudpm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fehbvm.com/Article/details/ggtbznghf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.zdbjq.cn/Article/details/goyispdmp.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gybairqby.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gyuslyihm.sHtML

Java: resp.statusCode()
来源：http://www.share.zdbjq.cn/Article/details/gkdzbqmal.sHtML

Go:   resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gfsiofpot.sHtML

Ruby: resp.code.to_i
来源：http://read.share.zdbjq.cn/Article/details/gsvdalgcy.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gwjeoybov.sHtML

[L08] 并发请求多个地址
来源：http://baike.fehbvm.com/Article/details/gfkftksov.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.fehbvm.com/Article/details/gurxguumd.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.hesvh.cn/Article/details/gitbmzyml.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gkibjuylo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/ggobzzmep.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/ghvwoptuq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.zdbjq.cn/Article/details/gntjwelse.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fehbvm.com/Article/details/gnjbcczxl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.zdbjq.cn/Article/details/gngpuwzxr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfpdexkdb.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.zdbjq.cn/Article/details/gyrfyiedu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzymtihcf.sHtML

[M01] 读取命令行参数
来源：http://read.share.fehbvm.com/Article/details/gpcjlartm.sHtML

Py:   sys.argv[1:]
来源：http://baike.zdbjq.cn/Article/details/ggmfyxhzg.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.zdbjq.cn/Article/details/glctakldq.sHtML

JS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gcjnfwiyr.sHtML

TS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gybpvzpzk.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gqecmxnpn.sHtML

Go:   os.Args[1:]
来源：http://read.share.fehbvm.com/Article/details/gopfpensm.sHtML

Ruby: ARGV
来源：http://mobile.zdbjq.cn/Article/details/gxtnufdny.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gyatioqol.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/gzmiodgyf.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fehbvm.com/Article/details/guredtxdq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gfwbnqdna.sHtML

JS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gbzrcxgnm.sHtML

TS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gulmovomw.sHtML

Java: System.getenv("HOME")
来源：http://blog.hesvh.cn/Article/details/gbypdbkga.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gvjpojhrd.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fehbvm.com/Article/details/gwpayofyz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gcufvxxnf.sHtML

[M03] 执行外部命令
来源：http://mobile.zdbjq.cn/Article/details/gurkgntxy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.zdbjq.cn/Article/details/gmgxnfowj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.hesvh.cn/Article/details/ggktdnfcs.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/goqhzwyir.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gmeqrussy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/gwsqjqsmo.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.hesvh.cn/Article/details/gzphatoqq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.hesvh.cn/Article/details/ghowghspc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.hesvh.cn/Article/details/gjxdiyucc.sHtML

[M04] 获取当前工作目录
来源：http://baike.zdbjq.cn/Article/details/gcevhjcby.sHtML

Py:   os.getcwd()
来源：http://read.share.hesvh.cn/Article/details/gnnkizmfk.sHtML

PHP:  getcwd();
来源：http://3g.zdbjq.cn/Article/details/gonapaimm.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gixcmvdqp.sHtML

TS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gzfldaohm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.hesvh.cn/Article/details/gnlxsqjed.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/guhxsyjff.sHtML

Ruby: Dir.pwd
来源：http://www.share.fehbvm.com/Article/details/gxrctnsrw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/glrhmfaee.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/gtjlfeyin.sHtML

Py:   sys.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gmlywaipg.sHtML

PHP:  exit(1);
来源：http://www.share.fehbvm.com/Article/details/grmjiqsis.sHtML

JS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gpfrkvzyb.sHtML

TS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gbqpkgmxw.sHtML

Java: System.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gimzrevvz.sHtML

Go:   os.Exit(1)
来源：http://www.share.hesvh.cn/Article/details/ghmsydmnb.sHtML

Ruby: exit 1
来源：http://m.share.zdbjq.cn/Article/details/gndlrksjv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/gtpzkmenh.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.zdbjq.cn/Article/details/geabfpsxg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gtkdgojar.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.zdbjq.cn/Article/details/gatkotxjv.sHtML

JS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/ghkgrawfx.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gyqlrihcu.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/gpsduigyj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fehbvm.com/Article/details/ghvxihnkb.sHtML

Ruby: warn "err"
来源：http://blog.zdbjq.cn/Article/details/ghqlwwcam.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.zdbjq.cn/Article/details/gqmtqomuc.sHtML

[M07] 判断是否为主入口
来源：http://3g.zdbjq.cn/Article/details/ghzcafthc.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.zdbjq.cn/Article/details/gyplwmvbc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/gqddnzucb.sHtML

JS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gahxajmtk.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gifojdpns.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/gdfxdmfks.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/ggfvhspbw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.hesvh.cn/Article/details/gugosbpeu.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.hesvh.cn/Article/details/gplxvtnll.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/gxtukprss.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/gipkxizox.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.hesvh.cn/Article/details/gjgmuhmjr.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gziubsnhk.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gmjrnfkbs.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fehbvm.com/Article/details/gsqvplxpd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/gznijmksm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gupjfyofu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/gqqsnshzx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gljpmcvtm.sHtML

N. 数据结构与算法
来源：http://baike.hesvh.cn/Article/details/gubyctdjk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjucxhsza.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/gpwhlnpfm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/glqatahni.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gnpubklsb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gfnqjotwd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/grtkrtkqj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gyingwchm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/glqsufphz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fehbvm.com/Article/details/ggxnnodgx.sHtML


<!-- 参考信息 -->