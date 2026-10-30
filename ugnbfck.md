代发 wailian999

[J03] 字符串解析为日期
来源：http://m.share.fanxiaobao.xyz/Article/details/gdcdctsik.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfqvwehk.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.fanxiaobao.xyz/Article/details/gewxrtxdq.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxepbrgxq.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.fanxiaobao.xyz/Article/details/gzhdhcxap.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.fanxiaobao.xyz/Article/details/gydshoxpe.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.fanxiaobao.xyz/Article/details/gonsdelqt.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.fanxiaobao.xyz/Article/details/gadacpvtd.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghaeqrjhz.sHtML

[J04] 时间戳与日期互转
来源：http://blog.fanxiaobao.xyz/Article/details/gaanuueey.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.fanxiaobao.xyz/Article/details/gqytqvfdz.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.fanxiaobao.xyz/Article/details/gylbgqdfk.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjgvuhlp.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.fanxiaobao.xyz/Article/details/gcvxeswdd.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyrqeaym.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhcvvyqq.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.fanxiaobao.xyz/Article/details/ghhebjazn.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.fanxiaobao.xyz/Article/details/gllitfmrc.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxhjigjb.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.fanxiaobao.xyz/Article/details/gqdzxkzpe.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstmhmszh.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fanxiaobao.xyz/Article/details/grmhszqug.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxmyuben.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfexgehy.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtqwoddg.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmqerqsz.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.fanxiaobao.xyz/Article/details/gllckyduv.sHtML

[J06] 计算两时间之差
来源：http://baike.fanxiaobao.xyz/Article/details/gwyytrqvc.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.fanxiaobao.xyz/Article/details/gttuqnkct.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.fanxiaobao.xyz/Article/details/gooqhkdzv.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.fanxiaobao.xyz/Article/details/gtjoewbsa.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtudfihac.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdipcbxq.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnctpfdz.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.fanxiaobao.xyz/Article/details/gaianqaaf.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.fanxiaobao.xyz/Article/details/golfoixfc.sHtML

[J07] 比较两个日期
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbyguepa.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlfgddln.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.fanxiaobao.xyz/Article/details/grnzivcip.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.fanxiaobao.xyz/Article/details/gulaxgopd.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqkgaaag.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdmswppm.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlyopqos.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.fanxiaobao.xyz/Article/details/gdnfdhgzj.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.fanxiaobao.xyz/Article/details/gqspwjsqr.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydwomptl.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbzsywht.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.fanxiaobao.xyz/Article/details/gairotzaw.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmvnuwmc.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfwutkbn.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.fanxiaobao.xyz/Article/details/gjjtqdflj.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwqvrogr.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbqaqiig.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.fanxiaobao.xyz/Article/details/ghytpshcf.sHtML

[J09] 时区处理
来源：http://baike.fanxiaobao.xyz/Article/details/gfnujibnk.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.fanxiaobao.xyz/Article/details/gptjrwatc.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvqkzubb.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fanxiaobao.xyz/Article/details/gdzayqcjc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gouzxaavq.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.fanxiaobao.xyz/Article/details/gmmiedizf.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzidiyeq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhxlvejf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.fanxiaobao.xyz/Article/details/grhknlkld.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.fanxiaobao.xyz/Article/details/gevhnssrn.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.fanxiaobao.xyz/Article/details/gntvxjexl.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.fanxiaobao.xyz/Article/details/grlihyrtx.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/glukgmnfh.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/gsnebbkim.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghieavene.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.fanxiaobao.xyz/Article/details/gwjdzqoub.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnhaqceh.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxosinleu.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gaawzrart.sHtML

K. JSON 与序列化
来源：http://wap.fanxiaobao.xyz/Article/details/ggahgevsp.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gwuqagpgd.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gguclceyn.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.fanxiaobao.xyz/Article/details/gupfyzpsr.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzayhrakq.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/giurcmspp.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glilpdaus.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmgundde.sHtML

Go:   json.Marshal(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gcwdyoujk.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.fanxiaobao.xyz/Article/details/gayzorzui.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gsfqpjium.sHtML

[K02] JSON 字符串转对象
来源：http://blog.fanxiaobao.xyz/Article/details/gaaetbnfn.sHtML

Py:   json.loads(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmdlwath.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.fanxiaobao.xyz/Article/details/gcfjutwnh.sHtML

JS:   JSON.parse(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnmowcva.sHtML

TS:   JSON.parse(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gnzreerxb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjzpbpck.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.fanxiaobao.xyz/Article/details/gowiibbdf.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfuszeccw.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gaeyprvvb.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.fanxiaobao.xyz/Article/details/gucdhzalt.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgwtxswc.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevioznnb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlrcjwof.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gzojtjkhg.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijxpqfeq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftciesbm.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gescwytuh.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvtvrbcd.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswloicue.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.fanxiaobao.xyz/Article/details/gztzolhuo.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjrzyhzf.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnadjybh.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fanxiaobao.xyz/Article/details/gshigmzog.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmgjvnip.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxfulmrj.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzexzahr.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflcoqmwa.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnfgnbmm.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/ggkjnjrvt.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzycpzwdv.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkpvzvao.sHtML

TS:   structuredClone(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqslyjlj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.fanxiaobao.xyz/Article/details/gnytkahuf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.fanxiaobao.xyz/Article/details/grsqdukbv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqadnaht.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpldnjps.sHtML

[K06] 解析 URL 查询串
来源：http://blog.fanxiaobao.xyz/Article/details/gvupcmvtc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghruaqyhb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.fanxiaobao.xyz/Article/details/gcwgotleb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fanxiaobao.xyz/Article/details/gyasmsqih.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fanxiaobao.xyz/Article/details/gmeemanim.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtkggozx.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqyimmcn.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.fanxiaobao.xyz/Article/details/gninroehv.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhipobdt.sHtML

[K07] 进制转换
来源：http://baike.fanxiaobao.xyz/Article/details/gbeimapcn.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gazlgpbcv.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyxzsmll.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.fanxiaobao.xyz/Article/details/gfwsugytp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlbeknzc.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvrbmrrn.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzretzkul.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fanxiaobao.xyz/Article/details/gxucfglnt.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fanxiaobao.xyz/Article/details/gdjsfylyh.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.fanxiaobao.xyz/Article/details/gspveqzry.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gugdyqipj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfpmeplo.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.fanxiaobao.xyz/Article/details/gjobstsfc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.fanxiaobao.xyz/Article/details/gamostlsg.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjqdgjsz.sHtML

Go:   encoding/gob
来源：http://baike.fanxiaobao.xyz/Article/details/gwruarbxu.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonoriqfc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwzeynqx.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gjoulutvm.sHtML

L. 网络请求
来源：http://m.share.fanxiaobao.xyz/Article/details/gegogoems.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikgpgxzo.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhaiwbsc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.fanxiaobao.xyz/Article/details/glaucbduc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpaklwjk.sHtML

JS:   await fetch(url)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbyorkcl.sHtML

TS:   await fetch(url)
来源：http://wap.fanxiaobao.xyz/Article/details/gptpevoxq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fanxiaobao.xyz/Article/details/gkllxtlec.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnvcwtfa.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmjkpbcy.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvffrcubb.sHtML

[L02] 发送 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvbzpljm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.fanxiaobao.xyz/Article/details/gtxekbusj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.fanxiaobao.xyz/Article/details/glyedlbdl.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fanxiaobao.xyz/Article/details/gmivleadj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fanxiaobao.xyz/Article/details/gznyyzhuk.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.fanxiaobao.xyz/Article/details/gpilwvyxh.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqqbnici.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.fanxiaobao.xyz/Article/details/gdveqymuv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkmniypd.sHtML

[L03] 设置自定义请求头
来源：http://blog.fanxiaobao.xyz/Article/details/gjjbycwps.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fanxiaobao.xyz/Article/details/gyzlijzgm.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogjaqgzd.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhigkoqq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnoshzkc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fanxiaobao.xyz/Article/details/gyuznwahn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fanxiaobao.xyz/Article/details/gxywnxkoh.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgeilxxq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grihpclrj.sHtML

[L04] 设置超时
来源：http://wap.fanxiaobao.xyz/Article/details/gwemsvtim.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmlcbrvj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fanxiaobao.xyz/Article/details/gwhehvyes.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fanxiaobao.xyz/Article/details/gbbixclyk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fanxiaobao.xyz/Article/details/gztcpbplg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcehyoei.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fanxiaobao.xyz/Article/details/gemuldzhk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzocvjvw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgmjlqdg.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.fanxiaobao.xyz/Article/details/gzixqacoj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbrtmudz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemyreffz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fanxiaobao.xyz/Article/details/gltcapxql.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glsyxfmxu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fanxiaobao.xyz/Article/details/gwtzlsefm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fanxiaobao.xyz/Article/details/garflvbfd.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fanxiaobao.xyz/Article/details/gfhgsnvjo.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gscxzrbnl.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/glyonolew.sHtML

Py:   resp.json()
来源：http://read.share.fanxiaobao.xyz/Article/details/gynuuorqf.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsxfvahk.sHtML

JS:   await resp.json()
来源：http://read.share.fanxiaobao.xyz/Article/details/giqkpfotp.sHtML

TS:   await resp.json()
来源：http://baike.fanxiaobao.xyz/Article/details/gxpnvqqfv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqseiajul.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fanxiaobao.xyz/Article/details/gqusikabr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fanxiaobao.xyz/Article/details/gpfsietpn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fanxiaobao.xyz/Article/details/gvdoxcfxt.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gekoooebf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlipfzab.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqemtlytr.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fanxiaobao.xyz/Article/details/gtphpegdc.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fanxiaobao.xyz/Article/details/govrxkris.sHtML

Java: resp.statusCode()
来源：http://baike.fanxiaobao.xyz/Article/details/gbjzhgjza.sHtML

Go:   resp.StatusCode
来源：http://3g.fanxiaobao.xyz/Article/details/gkenvrmuq.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fanxiaobao.xyz/Article/details/gapntkhcn.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fanxiaobao.xyz/Article/details/gtmknrulh.sHtML

[L08] 并发请求多个地址
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqybmmxp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fanxiaobao.xyz/Article/details/gekrubzrn.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fanxiaobao.xyz/Article/details/gqhvvlith.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fanxiaobao.xyz/Article/details/goeabjvyu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfilcfbim.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fanxiaobao.xyz/Article/details/gycewiaon.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fanxiaobao.xyz/Article/details/gxchdxwih.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fanxiaobao.xyz/Article/details/gppvnfjdr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvnffmew.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/grlcpusqw.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fanxiaobao.xyz/Article/details/gbmkgcjly.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gnckmvvlh.sHtML

[M01] 读取命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkpbjfku.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fanxiaobao.xyz/Article/details/gpewdwjip.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fanxiaobao.xyz/Article/details/gznxakqvz.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjgmlnvk.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fanxiaobao.xyz/Article/details/gypcsjfgb.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxkeiagj.sHtML

Go:   os.Args[1:]
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjefcobc.sHtML

Ruby: ARGV
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkyabelit.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.fanxiaobao.xyz/Article/details/gzerdhbyl.sHtML

[M02] 读取环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrxqyfub.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fanxiaobao.xyz/Article/details/gwpzwrmik.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjtmoybt.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlutyswn.sHtML

TS:   process.env.HOME
来源：http://baike.fanxiaobao.xyz/Article/details/gguyxbirk.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fanxiaobao.xyz/Article/details/grzlpcdeu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fanxiaobao.xyz/Article/details/gsbrenavb.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fanxiaobao.xyz/Article/details/gdyjyawwm.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fanxiaobao.xyz/Article/details/gssqczgdd.sHtML

[M03] 执行外部命令
来源：http://blog.fanxiaobao.xyz/Article/details/ggzysnubw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gxzuarhag.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fanxiaobao.xyz/Article/details/gkohtxuok.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkomqbsw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fanxiaobao.xyz/Article/details/gokkhgnca.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtfmihzi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fanxiaobao.xyz/Article/details/gsuoilytx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmycamskr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fanxiaobao.xyz/Article/details/gdfhytgsa.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzhrhkki.sHtML

Py:   os.getcwd()
来源：http://m.share.fanxiaobao.xyz/Article/details/gddsmbeut.sHtML

PHP:  getcwd();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grijldzzq.sHtML

JS:   process.cwd()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysetrvrm.sHtML

TS:   process.cwd()
来源：http://3g.fanxiaobao.xyz/Article/details/gdnsvqoru.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtefmakjc.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyozsacnj.sHtML

Ruby: Dir.pwd
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyonffts.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fanxiaobao.xyz/Article/details/gyjjghnaj.sHtML

[M05] 设置退出码
来源：http://wap.fanxiaobao.xyz/Article/details/gcmrkszbx.sHtML

Py:   sys.exit(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gtdueepdf.sHtML

PHP:  exit(1);
来源：http://baike.fanxiaobao.xyz/Article/details/gljaxusnw.sHtML

JS:   process.exit(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkrijlfz.sHtML

TS:   process.exit(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gddvtajtc.sHtML

Java: System.exit(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/guepooraq.sHtML

Go:   os.Exit(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gijpheodc.sHtML

Ruby: exit 1
来源：http://3g.fanxiaobao.xyz/Article/details/gsaqmvohg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fanxiaobao.xyz/Article/details/ghogxcjzh.sHtML

[M06] 向标准错误输出
来源：http://m.share.fanxiaobao.xyz/Article/details/giambtaen.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fanxiaobao.xyz/Article/details/gpqivgxce.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fanxiaobao.xyz/Article/details/golqipupg.sHtML

JS:   console.error("err")
来源：http://3g.fanxiaobao.xyz/Article/details/gmtipmdqd.sHtML

TS:   console.error("err")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjtvgyka.sHtML

Java: System.err.println("err")
来源：http://wap.fanxiaobao.xyz/Article/details/galmsawov.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdgkoerp.sHtML

Ruby: warn "err"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtpxlxnm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjgioglp.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgkewtmz.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifpnaeol.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fanxiaobao.xyz/Article/details/gvledowbw.sHtML

JS:   require.main === module
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqogtlkc.sHtML

TS:   require.main === module
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwbmnook.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fanxiaobao.xyz/Article/details/giyleeacq.sHtML

Go:   func main()
来源：http://baike.fanxiaobao.xyz/Article/details/gunijsdxh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fanxiaobao.xyz/Article/details/gpusfnljk.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fanxiaobao.xyz/Article/details/gpapbqank.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fanxiaobao.xyz/Article/details/gmphygcim.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fanxiaobao.xyz/Article/details/gcomevcpb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fanxiaobao.xyz/Article/details/ghmdedyhk.sHtML

JS:   process.platform;  process.version
来源：http://blog.fanxiaobao.xyz/Article/details/gvvdanrbv.sHtML

TS:   process.platform;  process.version
来源：http://3g.fanxiaobao.xyz/Article/details/gckbzdwow.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fanxiaobao.xyz/Article/details/gqmuxfvpm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fanxiaobao.xyz/Article/details/gukotybzu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fanxiaobao.xyz/Article/details/gwrundqls.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fanxiaobao.xyz/Article/details/goipptmlu.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gzehuaeno.sHtML

N. 数据结构与算法
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmbxnwhb.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gmywofpgh.sHtML


<!-- 参考信息 -->