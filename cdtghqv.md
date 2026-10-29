代发 wailian999

[J03] 字符串解析为日期
来源：http://www.share.fehbvm.com/Article/details/gbgcjgrke.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.hesvh.cn/Article/details/gllutmcfu.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.hesvh.cn/Article/details/gpjtuvjvx.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gmsyytmjp.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gokgqvurk.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gedfiknbo.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gpnwhmmxs.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gjqypfuoo.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.hesvh.cn/Article/details/glffygqaz.sHtML

[J04] 时间戳与日期互转
来源：http://blog.fehbvm.com/Article/details/glqkdacwz.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.fehbvm.com/Article/details/gowkcjaxz.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.zdbjq.cn/Article/details/guolafqju.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.fehbvm.com/Article/details/glmqgwwez.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.zdbjq.cn/Article/details/gqidszmnv.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.zdbjq.cn/Article/details/gdmljxpll.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.hesvh.cn/Article/details/gustceuon.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.hesvh.cn/Article/details/gbrshxbqt.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.fehbvm.com/Article/details/grnfzesqp.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.hesvh.cn/Article/details/gmtmhfede.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.fehbvm.com/Article/details/grorwmqtj.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.zdbjq.cn/Article/details/gdyczhatt.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.hesvh.cn/Article/details/ggzsymiha.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fehbvm.com/Article/details/gjgdshowx.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.hesvh.cn/Article/details/gtunlrzcd.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.hesvh.cn/Article/details/gwnuvipku.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.zdbjq.cn/Article/details/gkjhteefu.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.zdbjq.cn/Article/details/gcptnuqst.sHtML

[J06] 计算两时间之差
来源：http://3g.zdbjq.cn/Article/details/gluwrhyqs.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.fehbvm.com/Article/details/gkcqpkoxs.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.fehbvm.com/Article/details/gajjdafdk.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.hesvh.cn/Article/details/glkngbbha.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.fehbvm.com/Article/details/gxojhsoxm.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.zdbjq.cn/Article/details/gjbbjiesh.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.hesvh.cn/Article/details/gityixady.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.zdbjq.cn/Article/details/gfkvainlj.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.fehbvm.com/Article/details/gclxhepjb.sHtML

[J07] 比较两个日期
来源：http://baike.zdbjq.cn/Article/details/gxdizuwan.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/gcjxfjyvu.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.hesvh.cn/Article/details/gnpdezqig.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.fehbvm.com/Article/details/gkozrebvw.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.fehbvm.com/Article/details/gekrosilv.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.fehbvm.com/Article/details/ggjdtmtqp.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.hesvh.cn/Article/details/gsyjacjur.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.fehbvm.com/Article/details/gjhhmhyqd.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.zdbjq.cn/Article/details/gcviwnvwz.sHtML

[J08] 提取年月日与星期
来源：http://m.share.zdbjq.cn/Article/details/gbosyrkrk.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.fehbvm.com/Article/details/gliltpndk.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.hesvh.cn/Article/details/gmwevlfmp.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.fehbvm.com/Article/details/gnfqjsfgg.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.hesvh.cn/Article/details/gtpqqygby.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.fehbvm.com/Article/details/gtcwmifuc.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.fehbvm.com/Article/details/gjiugpldx.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.hesvh.cn/Article/details/gfzcowzzv.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.hesvh.cn/Article/details/ghilinyjq.sHtML

[J09] 时区处理
来源：http://mobile.fehbvm.com/Article/details/gajhunpto.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.hesvh.cn/Article/details/gvpnbkgld.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.zdbjq.cn/Article/details/ghraznwhy.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.zdbjq.cn/Article/details/ghlghespa.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.hesvh.cn/Article/details/gnncaxeoo.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.zdbjq.cn/Article/details/gsefintkd.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.zdbjq.cn/Article/details/gdhzochol.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.hesvh.cn/Article/details/gorexijxc.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.fehbvm.com/Article/details/gzoquktzm.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.hesvh.cn/Article/details/gbucjyosf.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.zdbjq.cn/Article/details/glpovides.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.zdbjq.cn/Article/details/gnqxcrsba.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.fehbvm.com/Article/details/gfiebzbec.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gegentjnv.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.fehbvm.com/Article/details/gzpylnhci.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.hesvh.cn/Article/details/gvbcfhhqa.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.hesvh.cn/Article/details/gochxgddb.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.hesvh.cn/Article/details/gyokujfht.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/goghaxamt.sHtML

K. JSON 与序列化
来源：http://wap.fehbvm.com/Article/details/ggkticbgt.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkuwpgcuq.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.zdbjq.cn/Article/details/glumfoglu.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.hesvh.cn/Article/details/gpxfzcpxu.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fehbvm.com/Article/details/gclklokhs.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.hesvh.cn/Article/details/gguokyiqm.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.zdbjq.cn/Article/details/gsmpznpgj.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.hesvh.cn/Article/details/gymdltyvz.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.fehbvm.com/Article/details/ggqudxbhv.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.fehbvm.com/Article/details/gyjbpbsdz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.zdbjq.cn/Article/details/gtpjslxmy.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.hesvh.cn/Article/details/gjxenpzqe.sHtML

Py:   json.loads(s)
来源：http://blog.fehbvm.com/Article/details/gxqdmpsha.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.hesvh.cn/Article/details/gqnfqqiil.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/gvsvfwpih.sHtML

TS:   JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gnvpksemj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gtrfxrbjf.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/gyfobowcd.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/geeeqvrme.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.zdbjq.cn/Article/details/gsodgxmep.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.fehbvm.com/Article/details/gclxykbjg.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.fehbvm.com/Article/details/gblyahlyh.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.fehbvm.com/Article/details/gmsvpvieh.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gnuzbxsni.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.hesvh.cn/Article/details/gocsamvcr.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.zdbjq.cn/Article/details/gdlypoksv.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.zdbjq.cn/Article/details/gmrxmraoj.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.fehbvm.com/Article/details/gujstreqf.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.fehbvm.com/Article/details/gvfpaszpb.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.zdbjq.cn/Article/details/gqgdlpefv.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.zdbjq.cn/Article/details/gztplzydc.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.fehbvm.com/Article/details/gonhxpyur.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fehbvm.com/Article/details/gubylqglz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/gcxgxlcec.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.hesvh.cn/Article/details/gzhwfoukd.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/gzvsglikt.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.fehbvm.com/Article/details/gfixyloxj.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.hesvh.cn/Article/details/gjzhxbvqh.sHtML

[K05] 深拷贝对象
来源：http://3g.hesvh.cn/Article/details/gbjjjlywk.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.hesvh.cn/Article/details/gtvuowbpr.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.hesvh.cn/Article/details/ghuxzrona.sHtML

JS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/glkgtkoqr.sHtML

TS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gzrsyvspv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.zdbjq.cn/Article/details/gqyzhneqo.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.zdbjq.cn/Article/details/gkjnoehiu.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.hesvh.cn/Article/details/gyjzkxhkl.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.zdbjq.cn/Article/details/ghcbuzzzi.sHtML

[K06] 解析 URL 查询串
来源：http://baike.fehbvm.com/Article/details/gmzetclvf.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.zdbjq.cn/Article/details/gwoxpssns.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.fehbvm.com/Article/details/ghqjlbdwr.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/gwjsmkinu.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/gmvizkqlu.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.hesvh.cn/Article/details/guaxrqthg.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/ggnblmxgd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gslgfpejl.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gndvhtogd.sHtML

[K07] 进制转换
来源：http://www.share.zdbjq.cn/Article/details/gpjwtdjhd.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gbzxnxgzi.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.hesvh.cn/Article/details/grmrufxry.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gerbrpcms.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gpkhzgson.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/ggkbsivue.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.fehbvm.com/Article/details/gonqurwco.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.fehbvm.com/Article/details/gsottmaqs.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gsfnxxfmt.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.hesvh.cn/Article/details/gtfvzsozb.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gvjkcfyti.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.zdbjq.cn/Article/details/gxfszlqfe.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/gjnxqsilz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/gxcycapfo.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.hesvh.cn/Article/details/gugakujvv.sHtML

Go:   encoding/gob
来源：http://3g.fehbvm.com/Article/details/grncnhely.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gxklzrouj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/ghumaigla.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvaoweplf.sHtML

L. 网络请求
来源：http://3g.hesvh.cn/Article/details/ghfjvwfck.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gocbrromy.sHtML

[L01] 发送 GET 请求
来源：http://baike.zdbjq.cn/Article/details/ggyujdwsq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.hesvh.cn/Article/details/glmvugmis.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.hesvh.cn/Article/details/gwueouvcw.sHtML

JS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/gyquaqbod.sHtML

TS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/grnoloqbg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.hesvh.cn/Article/details/ghahjluao.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.fehbvm.com/Article/details/gqwzwhlwx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.fehbvm.com/Article/details/gcwlcjkyq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.zdbjq.cn/Article/details/gbprjawos.sHtML

[L02] 发送 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gxccrxkra.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gkkxrlvca.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.hesvh.cn/Article/details/gsmfyyxuw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/gvksjhvsb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gupkdjfqk.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.zdbjq.cn/Article/details/grpoamxoi.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.zdbjq.cn/Article/details/gkccjwdbw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fehbvm.com/Article/details/gjojeciuw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.fehbvm.com/Article/details/gonztedow.sHtML

[L03] 设置自定义请求头
来源：http://m.share.hesvh.cn/Article/details/geiqugcmc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.fehbvm.com/Article/details/ghldxpijs.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fehbvm.com/Article/details/gxdihlkyc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gunwtcpao.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gmtvlakab.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.hesvh.cn/Article/details/gjasezzbj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gzfkzkwyl.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.hesvh.cn/Article/details/gazccdtle.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gcgcbuvet.sHtML

[L04] 设置超时
来源：http://m.share.hesvh.cn/Article/details/gdbnjokkb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.zdbjq.cn/Article/details/grtbwqqxu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.hesvh.cn/Article/details/gfxxcerof.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/geapgaeor.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gufjuyldg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fehbvm.com/Article/details/guscarchj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.zdbjq.cn/Article/details/glkdxqels.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fehbvm.com/Article/details/gykzgqjyv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fehbvm.com/Article/details/gyhdzkksy.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fehbvm.com/Article/details/grwjfwmwr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.zdbjq.cn/Article/details/gqytaftzx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.zdbjq.cn/Article/details/gukcrqrdy.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gskhotytk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/givuigzxp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.zdbjq.cn/Article/details/geycfkxjb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.zdbjq.cn/Article/details/gxiurdgia.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fehbvm.com/Article/details/gznyggixs.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gjatppocj.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.hesvh.cn/Article/details/glqqfpljp.sHtML

Py:   resp.json()
来源：http://wap.fehbvm.com/Article/details/gujqccrfl.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fehbvm.com/Article/details/gyrzlhkeo.sHtML

JS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gzyjihlni.sHtML

TS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gfgouewqt.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fehbvm.com/Article/details/glhtyivtf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.zdbjq.cn/Article/details/gyhmttmfi.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fehbvm.com/Article/details/gisjgzwus.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fehbvm.com/Article/details/gufpiecjs.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gfkhloatv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fehbvm.com/Article/details/gdjwiptvu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fehbvm.com/Article/details/gfxexweje.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/glbukbzpg.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/goptgfkpz.sHtML

Java: resp.statusCode()
来源：http://baike.fehbvm.com/Article/details/glwomzqpq.sHtML

Go:   resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gcvenivws.sHtML

Ruby: resp.code.to_i
来源：http://m.share.zdbjq.cn/Article/details/gjvxoymjs.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gvumnhnkn.sHtML

[L08] 并发请求多个地址
来源：http://3g.hesvh.cn/Article/details/gxwhaqerh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.zdbjq.cn/Article/details/gvvjxpofm.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.fehbvm.com/Article/details/gustaovld.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gyceqpplg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gtakgscpr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.zdbjq.cn/Article/details/gntapsqiw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.hesvh.cn/Article/details/ggztogsuo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gkvwtpuyl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gnbdelndd.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gpqkzoril.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fehbvm.com/Article/details/geefbrzwr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmqtzblrt.sHtML

[M01] 读取命令行参数
来源：http://baike.zdbjq.cn/Article/details/gnpmowjkp.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gpjucmhlj.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.hesvh.cn/Article/details/glqqcisvd.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gzoztsfkm.sHtML

TS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gtwlzloes.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gzjfpgyuz.sHtML

Go:   os.Args[1:]
来源：http://3g.zdbjq.cn/Article/details/gdrimtydu.sHtML

Ruby: ARGV
来源：http://m.share.zdbjq.cn/Article/details/gpuyszaqg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/glscxuqit.sHtML

[M02] 读取环境变量
来源：http://3g.zdbjq.cn/Article/details/goaeidwoy.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.hesvh.cn/Article/details/gjtngpyat.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gdmlhrxaz.sHtML

JS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gjbvglghn.sHtML

TS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gosxdffas.sHtML

Java: System.getenv("HOME")
来源：http://wap.fehbvm.com/Article/details/gntufugey.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gygzmxrom.sHtML

Ruby: ENV["HOME"]
来源：http://wap.hesvh.cn/Article/details/ghpurilqk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gvkwaggsf.sHtML

[M03] 执行外部命令
来源：http://read.share.zdbjq.cn/Article/details/gmiocaqwb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.zdbjq.cn/Article/details/grcntahwz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fehbvm.com/Article/details/gwkskwjla.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gqcvjhybl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gqrfsfrlh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gqobnnook.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.zdbjq.cn/Article/details/gdazjyjyn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fehbvm.com/Article/details/gwjkwlecv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.hesvh.cn/Article/details/goeebdkps.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/grtqaotsq.sHtML

Py:   os.getcwd()
来源：http://3g.hesvh.cn/Article/details/ghzyvuxxn.sHtML

PHP:  getcwd();
来源：http://wap.hesvh.cn/Article/details/glslpsanf.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gtasxllhl.sHtML

TS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gptvptvtg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.zdbjq.cn/Article/details/goqipholk.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/gibgtyzfc.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gkuebgojy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.hesvh.cn/Article/details/gdtkzyykb.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/gcxbftxdu.sHtML

Py:   sys.exit(1)
来源：http://m.share.fehbvm.com/Article/details/geyobjdtj.sHtML

PHP:  exit(1);
来源：http://baike.hesvh.cn/Article/details/gbupmighn.sHtML

JS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/grgfiopzh.sHtML

TS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gjbevyosq.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gwaapgdnk.sHtML

Go:   os.Exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gvyihgdnn.sHtML

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/ggrcdomah.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/gerkiiziv.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/gpbhafzhb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/gwffawweq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.hesvh.cn/Article/details/givkzquel.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gmiytyste.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/glsbgmnrd.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/gpswpodxh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/gliafndch.sHtML

Ruby: warn "err"
来源：http://www.m.share.fehbvm.com/Article/details/gzqdhjkzv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.zdbjq.cn/Article/details/gchalzmka.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/ghozeclss.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/gksrikxpc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.zdbjq.cn/Article/details/gcytifnoy.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gffekozgk.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gihwsrtxs.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fehbvm.com/Article/details/gfvnauypl.sHtML

Go:   func main()
来源：http://3g.hesvh.cn/Article/details/gmbmbadfe.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/gzaibgkvt.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/gouhxgzxq.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.hesvh.cn/Article/details/gsuvrsroc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.hesvh.cn/Article/details/gvbotfhkz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/gwskpezru.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gczmabwtk.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gpmrivikz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/gmvhmkevx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.hesvh.cn/Article/details/gevmpulbs.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.zdbjq.cn/Article/details/gnxiqfxps.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/gqknduopl.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnzqvamwt.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/gojxsjxaa.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gspqnrvsq.sHtML


<!-- 参考信息 -->