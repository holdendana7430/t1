代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.fehbvm.com/Article/details/ghvcypmqp.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.zdbjq.cn/Article/details/gqnnfoshs.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fehbvm.com/Article/details/gxnippboj.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.zdbjq.cn/Article/details/gsgqwnmsc.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.zdbjq.cn/Article/details/gbjhdvhcf.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.hesvh.cn/Article/details/giavipblw.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.fehbvm.com/Article/details/gvrqtuajs.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gdijwxxlb.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gtntsawxf.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gvvhhndhy.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gofaeazaj.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/ggxlxwbqg.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.hesvh.cn/Article/details/ghifhprct.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.fehbvm.com/Article/details/gkuhczoca.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.hesvh.cn/Article/details/gogxewmpa.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.zdbjq.cn/Article/details/gikzpxjtp.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.zdbjq.cn/Article/details/gaminvauo.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.zdbjq.cn/Article/details/gtrmatang.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.fehbvm.com/Article/details/gpbcoozou.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.zdbjq.cn/Article/details/ghhfsybze.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.zdbjq.cn/Article/details/gbhyfgogo.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.fehbvm.com/Article/details/gskxeluli.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.hesvh.cn/Article/details/gvmtwztwd.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.zdbjq.cn/Article/details/ghyitdssb.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.fehbvm.com/Article/details/gimuzczca.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fehbvm.com/Article/details/gzofalvrz.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.hesvh.cn/Article/details/gdgmmogso.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.fehbvm.com/Article/details/geyvmgjol.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.fehbvm.com/Article/details/ghdyiplai.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.zdbjq.cn/Article/details/gcjjmwtah.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.fehbvm.com/Article/details/gtnmtgvsc.sHtML

[J06] 计算两时间之差
来源：http://blog.fehbvm.com/Article/details/gpoxqoiag.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.hesvh.cn/Article/details/goyuwluzi.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.hesvh.cn/Article/details/ghharorcn.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.hesvh.cn/Article/details/gmfkguhzh.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.fehbvm.com/Article/details/ghliyjume.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.hesvh.cn/Article/details/gfxhxgpvj.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.hesvh.cn/Article/details/gwkhbhbzr.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.zdbjq.cn/Article/details/gvjkbxwpj.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.zdbjq.cn/Article/details/gvyobeesx.sHtML

[J07] 比较两个日期
来源：http://m.share.fehbvm.com/Article/details/ghyjuazer.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/gkgclbfdr.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.fehbvm.com/Article/details/gwnfwjypi.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.hesvh.cn/Article/details/gppcggrnt.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.hesvh.cn/Article/details/gxiqmgkvf.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.fehbvm.com/Article/details/gavblynir.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.zdbjq.cn/Article/details/gbunrzndj.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/gvcrskvab.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.zdbjq.cn/Article/details/gkxcpqtad.sHtML

[J08] 提取年月日与星期
来源：http://m.share.hesvh.cn/Article/details/glybsqdyf.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.fehbvm.com/Article/details/gromzykbl.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.zdbjq.cn/Article/details/gjwmiygbb.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.fehbvm.com/Article/details/gvsvpaxhk.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.zdbjq.cn/Article/details/gzoahckct.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.hesvh.cn/Article/details/gtmsjbspd.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.fehbvm.com/Article/details/glxhpgkyj.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.fehbvm.com/Article/details/gsngsacjn.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.hesvh.cn/Article/details/gwoedmfpp.sHtML

[J09] 时区处理
来源：http://mobile.zdbjq.cn/Article/details/gmahaokbu.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.hesvh.cn/Article/details/gkjzzxvfj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.fehbvm.com/Article/details/grhngyrfi.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fehbvm.com/Article/details/ghcdaqvzo.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.hesvh.cn/Article/details/gjicndygo.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.zdbjq.cn/Article/details/ggbkqauvm.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.zdbjq.cn/Article/details/grobwxglh.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.zdbjq.cn/Article/details/gqgumwpos.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.zdbjq.cn/Article/details/gmhtvhptc.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.hesvh.cn/Article/details/gzeasppio.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.hesvh.cn/Article/details/gnlfxhdxs.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.zdbjq.cn/Article/details/ggcmxugpr.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.fehbvm.com/Article/details/ggegqqglg.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.fehbvm.com/Article/details/gqufbefbs.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.zdbjq.cn/Article/details/gtlgxwtid.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.fehbvm.com/Article/details/gfsguntwg.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.zdbjq.cn/Article/details/gpzbcjnpa.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.fehbvm.com/Article/details/gauyivmny.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggytiydns.sHtML

K. JSON 与序列化
来源：http://baike.zdbjq.cn/Article/details/gbaensvsi.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/giqeagdmb.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.fehbvm.com/Article/details/gxrgamomh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gpksboyip.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.hesvh.cn/Article/details/giilgwloe.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gthxflhrh.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.fehbvm.com/Article/details/gscctjzfr.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.zdbjq.cn/Article/details/gpfewwfck.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.hesvh.cn/Article/details/gkfuqnqmf.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.zdbjq.cn/Article/details/gtohlbmwy.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.fehbvm.com/Article/details/gydycnnzj.sHtML

[K02] JSON 字符串转对象
来源：http://blog.fehbvm.com/Article/details/gopslcxxf.sHtML

Py:   json.loads(s)
来源：http://www.blog.fehbvm.com/Article/details/gswsajqpl.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.fehbvm.com/Article/details/gurzosewo.sHtML

JS:   JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gppdidwye.sHtML

TS:   JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gjgknnhbc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.hesvh.cn/Article/details/gdhtfuaat.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.fehbvm.com/Article/details/griuwyuhm.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/gdghaxyns.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.hesvh.cn/Article/details/giniwbhoa.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.fehbvm.com/Article/details/gxdzyckvq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.zdbjq.cn/Article/details/gssqitsbf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/gotuuyapn.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/gvlyvwkwf.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/glvbxdxlr.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gyabhmusq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.fehbvm.com/Article/details/gnxvobdws.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gzwtjtipw.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.zdbjq.cn/Article/details/gbjnmmiwi.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.hesvh.cn/Article/details/gzptbeypy.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.fehbvm.com/Article/details/gsgmyymzj.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.fehbvm.com/Article/details/gsxctovke.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/gnobkwmbk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fehbvm.com/Article/details/gzkiotvho.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.fehbvm.com/Article/details/gskbahcqf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fehbvm.com/Article/details/gegjujade.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.fehbvm.com/Article/details/gcgyeplhq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.hesvh.cn/Article/details/gzfageoax.sHtML

[K05] 深拷贝对象
来源：http://wap.hesvh.cn/Article/details/gstrhzcpl.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gsnvmlown.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.zdbjq.cn/Article/details/gzahynygf.sHtML

JS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gtvrwrgzl.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gswvbonng.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.hesvh.cn/Article/details/gxiqrrstp.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.fehbvm.com/Article/details/gangufima.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.zdbjq.cn/Article/details/ggajrdudr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.zdbjq.cn/Article/details/gxwupolfi.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.fehbvm.com/Article/details/gbtjkggmr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gbywhnxng.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.zdbjq.cn/Article/details/gemavykwb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/gjyjxdxld.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/giauztfty.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gepigcyqf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gkhfzkvph.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gpzxdkkul.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gncvpuxje.sHtML

[K07] 进制转换
来源：http://m.share.hesvh.cn/Article/details/gkrpucjlq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gzrtyoaab.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.hesvh.cn/Article/details/ghzscubwy.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gajdyjlts.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gjmlhaoll.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gdzjwbhwd.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fehbvm.com/Article/details/gfxmrgnxy.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.fehbvm.com/Article/details/gxfwxdaka.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gulkrjisx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.zdbjq.cn/Article/details/gxplxqhrt.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.zdbjq.cn/Article/details/gxvemcojo.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.fehbvm.com/Article/details/gfpgzkuxy.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gtzzqlsfk.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/gqkkwctbs.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.fehbvm.com/Article/details/gemqkcblj.sHtML

Go:   encoding/gob
来源：http://m.share.zdbjq.cn/Article/details/gzyljjhzz.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.hesvh.cn/Article/details/gosrryhcl.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.hesvh.cn/Article/details/gpjqvzcpn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqqqdprko.sHtML

L. 网络请求
来源：http://www.share.fehbvm.com/Article/details/gejwyhxiv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfmpcrwti.sHtML

[L01] 发送 GET 请求
来源：http://www.share.fehbvm.com/Article/details/gtrrherns.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.hesvh.cn/Article/details/gdxejnjrw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.fehbvm.com/Article/details/gcjykexmm.sHtML

JS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/gxtfabvea.sHtML

TS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/ghnoevlot.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.zdbjq.cn/Article/details/gjigyxldb.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fehbvm.com/Article/details/gpwodenfb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.zdbjq.cn/Article/details/grkxsljvl.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fehbvm.com/Article/details/gfbpqfmhp.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gvldzkxym.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gjojzodxs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.hesvh.cn/Article/details/gyptppaue.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/ghpiqwvvq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gbplhikdv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gijqcxfpi.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.fehbvm.com/Article/details/gipmlqijb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.hesvh.cn/Article/details/gwlpwdmwi.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.fehbvm.com/Article/details/guvlamaam.sHtML

[L03] 设置自定义请求头
来源：http://3g.fehbvm.com/Article/details/gukpgjraw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.hesvh.cn/Article/details/gojqdbwer.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.zdbjq.cn/Article/details/ggqyxhyim.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gbrrulskl.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gbdpxnbqi.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.zdbjq.cn/Article/details/giduflmqf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/glpgjqytc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fehbvm.com/Article/details/gmnahgjlw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/glzojhyuk.sHtML

[L04] 设置超时
来源：http://www.m.share.fehbvm.com/Article/details/glfksyphq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.fehbvm.com/Article/details/glwudhbee.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.hesvh.cn/Article/details/giutnoipd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gmfzevcja.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gaqvpigvx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fehbvm.com/Article/details/gexrhtwin.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.hesvh.cn/Article/details/gizdikjbu.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fehbvm.com/Article/details/gtpgljbcd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.fehbvm.com/Article/details/gynqzzoja.sHtML

[L05] 上传文件（multipart）
来源：http://3g.hesvh.cn/Article/details/gxgrxvemt.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fehbvm.com/Article/details/gsifubkok.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fehbvm.com/Article/details/gevmafnsc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gzbfuwvvr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gbrvphctr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fehbvm.com/Article/details/gbugjgzne.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fehbvm.com/Article/details/gdpktlwny.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.hesvh.cn/Article/details/gduqrjbvk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gussbjxir.sHtML

[L06] 解析响应为 JSON
来源：http://3g.hesvh.cn/Article/details/gwbdscnjd.sHtML

Py:   resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gyfkocssy.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fehbvm.com/Article/details/gcfelqjyw.sHtML

JS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/guuqrryuz.sHtML

TS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gqvpqwjdz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fehbvm.com/Article/details/glebxzcmz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fehbvm.com/Article/details/gofksimnw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.zdbjq.cn/Article/details/gigbeymes.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fehbvm.com/Article/details/gbxmohbnu.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gucqzlemg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.zdbjq.cn/Article/details/gokmkngvv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.fehbvm.com/Article/details/gerojcoex.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gcegaylvj.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gdsfekbjq.sHtML

Java: resp.statusCode()
来源：http://m.share.zdbjq.cn/Article/details/gaczytfqk.sHtML

Go:   resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gfontqbkx.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fehbvm.com/Article/details/glvgqmlpl.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gacvizwmt.sHtML

[L08] 并发请求多个地址
来源：http://read.share.hesvh.cn/Article/details/gxnqcaqnn.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.zdbjq.cn/Article/details/ghjwhdohc.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.zdbjq.cn/Article/details/gbcwwyjxx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gitevvqhq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gxvahutfz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.hesvh.cn/Article/details/gtkquujks.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.hesvh.cn/Article/details/gfloxbrwk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gxzbzqnou.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.hesvh.cn/Article/details/gbcldarrh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/guicfbkbn.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.hesvh.cn/Article/details/gjhnhtgtd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxngofkev.sHtML

[M01] 读取命令行参数
来源：http://wap.hesvh.cn/Article/details/gcmhhprca.sHtML

Py:   sys.argv[1:]
来源：http://3g.hesvh.cn/Article/details/gvptxsgoi.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.zdbjq.cn/Article/details/gljoxzitg.sHtML

JS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gxtotoacf.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/ggbcpdsez.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/glvzflpgz.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gfrgiptvs.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/ggjttxylm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gldwgbhuq.sHtML

[M02] 读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gkdlwomec.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.zdbjq.cn/Article/details/gukzejfat.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gfjlfdzrw.sHtML

JS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gtzyvhrts.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gorztkwxi.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/ghxmnfhhb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.hesvh.cn/Article/details/gslnidgle.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fehbvm.com/Article/details/gfjdqtlxj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.hesvh.cn/Article/details/gpiwzprna.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gaqxsgeeu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.hesvh.cn/Article/details/gqabsramc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.hesvh.cn/Article/details/gpbjiaasy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/geqvlkarg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gyuyaepxj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/gvnqijwzs.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.zdbjq.cn/Article/details/gvwllaree.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fehbvm.com/Article/details/gseizuvjo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.zdbjq.cn/Article/details/gvbdkoktg.sHtML

[M04] 获取当前工作目录
来源：http://wap.zdbjq.cn/Article/details/grgmzpjir.sHtML

Py:   os.getcwd()
来源：http://wap.fehbvm.com/Article/details/ggxjzzhth.sHtML

PHP:  getcwd();
来源：http://wap.zdbjq.cn/Article/details/gevkyvzbx.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gcfocsuak.sHtML

TS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gowxliosh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fehbvm.com/Article/details/ggfchwcqj.sHtML

Go:   os.Getwd()
来源：http://wap.hesvh.cn/Article/details/ggwolelss.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/ghneoutki.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.zdbjq.cn/Article/details/gxgojtoog.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/gkxejkyzc.sHtML

Py:   sys.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gerzxxrgf.sHtML

PHP:  exit(1);
来源：http://read.share.fehbvm.com/Article/details/gutmlkvph.sHtML

JS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gasbumfso.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gpnllevbr.sHtML

Java: System.exit(1)
来源：http://wap.hesvh.cn/Article/details/glbyoirjo.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/giwbhbprt.sHtML

Ruby: exit 1
来源：http://wap.zdbjq.cn/Article/details/gvzcqfesk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gjfpmridx.sHtML

[M06] 向标准错误输出
来源：http://www.blog.hesvh.cn/Article/details/givcxvooe.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gmhqfzafp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gkkqzqitp.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gxigzixop.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gfayhkpxv.sHtML

Java: System.err.println("err")
来源：http://mobile.fehbvm.com/Article/details/gqaluvznm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.zdbjq.cn/Article/details/gpatfuqyd.sHtML

Ruby: warn "err"
来源：http://m.share.hesvh.cn/Article/details/gathactqe.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/gvgvbggou.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/gxwtrzhwx.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.zdbjq.cn/Article/details/gmvcsipoy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.zdbjq.cn/Article/details/gsjyrivom.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gyutcpvne.sHtML

TS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gpqdrmvro.sHtML

Java: public static void main(String[] args)
来源：http://mobile.hesvh.cn/Article/details/gcfdguvbf.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/gqlntgokv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.zdbjq.cn/Article/details/gcbradlvw.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fehbvm.com/Article/details/gqvghgyaj.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/gbqriapso.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/gdclbosib.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/gxmvyvfog.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gpcazdxzt.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/ggkrgkmsi.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.hesvh.cn/Article/details/gpraocegm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.zdbjq.cn/Article/details/gubjndatf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.hesvh.cn/Article/details/ghtlqjgiz.sHtML


<!-- 参考信息 -->