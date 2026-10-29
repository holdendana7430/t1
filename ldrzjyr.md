代发 wailian999

[J03] 字符串解析为日期
来源：http://blog.zdbjq.cn/Article/details/gtttwwcat.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.hesvh.cn/Article/details/ghgjngmrr.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.hesvh.cn/Article/details/ghjrueycp.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/glaycebca.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/goqjbkoaf.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gbpykopna.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gilqbudkr.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gzyhokslm.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.hesvh.cn/Article/details/gdyymaqst.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.zdbjq.cn/Article/details/gixnvhcjh.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gabwlhual.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.fehbvm.com/Article/details/geishxzig.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.hesvh.cn/Article/details/gusavjjdd.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.hesvh.cn/Article/details/geekyckwe.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.hesvh.cn/Article/details/gtfllsdbs.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.hesvh.cn/Article/details/gqjbpdgws.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.zdbjq.cn/Article/details/gptgikmad.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.fehbvm.com/Article/details/gfgffeniq.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.fehbvm.com/Article/details/gzjdiohlw.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.hesvh.cn/Article/details/ghpjduhqs.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.zdbjq.cn/Article/details/gfoswgoox.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.zdbjq.cn/Article/details/gqlwoyejn.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.zdbjq.cn/Article/details/gqrjddybz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.fehbvm.com/Article/details/gaebxqxwh.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.fehbvm.com/Article/details/gsmpeesio.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.zdbjq.cn/Article/details/gxaxuesin.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.zdbjq.cn/Article/details/ggnnnkrpu.sHtML

[J06] 计算两时间之差
来源：http://m.share.hesvh.cn/Article/details/ggkwyshkd.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.zdbjq.cn/Article/details/galgpdpul.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.fehbvm.com/Article/details/grppsvevo.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.fehbvm.com/Article/details/gtwtxaxcn.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.zdbjq.cn/Article/details/gdqjcwebv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.fehbvm.com/Article/details/gkpvgxkyq.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.zdbjq.cn/Article/details/glzfowxvl.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.fehbvm.com/Article/details/ghdoggaky.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.fehbvm.com/Article/details/gthhfmbon.sHtML

[J07] 比较两个日期
来源：http://3g.hesvh.cn/Article/details/gwbroodiz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.zdbjq.cn/Article/details/gtuiidblh.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.fehbvm.com/Article/details/gbhkxfmjv.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.fehbvm.com/Article/details/gnmseyyrp.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.hesvh.cn/Article/details/gblmxcokr.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.zdbjq.cn/Article/details/gonqdgkvy.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.hesvh.cn/Article/details/gwjwhyapu.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.hesvh.cn/Article/details/gzssbpqxs.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.fehbvm.com/Article/details/gtpxddwwd.sHtML

[J08] 提取年月日与星期
来源：http://mobile.zdbjq.cn/Article/details/ggkzkrxlo.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.fehbvm.com/Article/details/gvbmkcryz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.hesvh.cn/Article/details/grmoeuxrk.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.fehbvm.com/Article/details/gafwnyuns.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.zdbjq.cn/Article/details/ghlbxaffw.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.fehbvm.com/Article/details/ggtikgied.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.fehbvm.com/Article/details/gcunvgeue.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.hesvh.cn/Article/details/grspmghmj.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.zdbjq.cn/Article/details/gueagkxmf.sHtML

[J09] 时区处理
来源：http://www.m.share.zdbjq.cn/Article/details/gtlmqmrve.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.hesvh.cn/Article/details/gceswdjmt.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.zdbjq.cn/Article/details/gmexthcen.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.zdbjq.cn/Article/details/gytfokfzm.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fehbvm.com/Article/details/gjzateody.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.hesvh.cn/Article/details/gtllcskfh.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.hesvh.cn/Article/details/gvqgilhmt.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.fehbvm.com/Article/details/gwoxmftqo.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.zdbjq.cn/Article/details/gtcylunpz.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.hesvh.cn/Article/details/gcqfihoji.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.hesvh.cn/Article/details/gaerelcxj.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.fehbvm.com/Article/details/ggrprhyrg.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.hesvh.cn/Article/details/glgstekwm.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.hesvh.cn/Article/details/goawvvtbb.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.zdbjq.cn/Article/details/grvqsuden.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.hesvh.cn/Article/details/gymcpqsid.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.hesvh.cn/Article/details/gcmobfcpc.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.zdbjq.cn/Article/details/gswvpauij.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gypfcrysg.sHtML

K. JSON 与序列化
来源：http://blog.fehbvm.com/Article/details/gqpksyfdi.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtdnicgkm.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.hesvh.cn/Article/details/gjqtabefb.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.hesvh.cn/Article/details/gvnpcgull.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.hesvh.cn/Article/details/gpxmapnvb.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.hesvh.cn/Article/details/gunfhysfl.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.hesvh.cn/Article/details/gigwrsyes.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.fehbvm.com/Article/details/ghdeussac.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.hesvh.cn/Article/details/gjqnvxvty.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.zdbjq.cn/Article/details/grfjfzoep.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.fehbvm.com/Article/details/gtbnqqfyk.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.hesvh.cn/Article/details/glgwfdgzu.sHtML

Py:   json.loads(s)
来源：http://www.m.share.fehbvm.com/Article/details/gjecibbvs.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.fehbvm.com/Article/details/gmuetegsd.sHtML

JS:   JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/gmdujmznn.sHtML

TS:   JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gwnaxdwph.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.zdbjq.cn/Article/details/gjhtbimco.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/gwmhiqeme.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/gtevqvkez.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.hesvh.cn/Article/details/gxbmhmexs.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.fehbvm.com/Article/details/gfptkhztz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.hesvh.cn/Article/details/gvevoiyrj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/gfvircljh.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/gzshlrjht.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.zdbjq.cn/Article/details/gxrwhwstw.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.fehbvm.com/Article/details/gpzbiguss.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.hesvh.cn/Article/details/gpjilccsz.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.hesvh.cn/Article/details/gcbfrnkms.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.hesvh.cn/Article/details/gdtptmuxy.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.fehbvm.com/Article/details/gimpwxkmb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.fehbvm.com/Article/details/gsejyagkt.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.hesvh.cn/Article/details/gefizgvcc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fehbvm.com/Article/details/ggcitmvfv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/gpmqmmdct.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gwkejtldd.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.fehbvm.com/Article/details/gdubaktyh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.fehbvm.com/Article/details/giqudcmsc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.zdbjq.cn/Article/details/grhznbglr.sHtML

[K05] 深拷贝对象
来源：http://wap.zdbjq.cn/Article/details/gfgtodxqm.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gddxqekyc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.hesvh.cn/Article/details/gfpylvdgz.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gkvvufisd.sHtML

TS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gtiicpuex.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.hesvh.cn/Article/details/guvztxmnf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.hesvh.cn/Article/details/gcnnwouqe.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.fehbvm.com/Article/details/gvovjqorj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.zdbjq.cn/Article/details/ghkefxkre.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.hesvh.cn/Article/details/grdgnvaui.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gfplfyfic.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.zdbjq.cn/Article/details/gpuaweowg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.zdbjq.cn/Article/details/gufgvysid.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gnposhecx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.zdbjq.cn/Article/details/goaqeiofv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gixenelva.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/glafwwmxe.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gmhnkhbui.sHtML

[K07] 进制转换
来源：http://m.share.zdbjq.cn/Article/details/gorestemx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gwbovuwyy.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.hesvh.cn/Article/details/guvvlhiqs.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gemsdgfoj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/ghhvxzmpt.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gjidiipzj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.hesvh.cn/Article/details/gmvmbdxor.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.hesvh.cn/Article/details/gkeamtohm.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/glsehpjkj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.hesvh.cn/Article/details/guyeplanm.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.zdbjq.cn/Article/details/gvbwragfk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.zdbjq.cn/Article/details/gxyppzupm.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/gevcmiurr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/gpoxqmfdy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.hesvh.cn/Article/details/gkmzasoob.sHtML

Go:   encoding/gob
来源：http://www.share.fehbvm.com/Article/details/gyewzwass.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.zdbjq.cn/Article/details/gvxaponig.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gkviixvnz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcvmncymf.sHtML

L. 网络请求
来源：http://www.blog.zdbjq.cn/Article/details/gnuosenht.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gayirrsmm.sHtML

[L01] 发送 GET 请求
来源：http://3g.fehbvm.com/Article/details/gnzoxiudj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fehbvm.com/Article/details/grvlsymtf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.hesvh.cn/Article/details/gdchxvdar.sHtML

JS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gfvyipfop.sHtML

TS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gbstcgofy.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.hesvh.cn/Article/details/gjidtwjqr.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.hesvh.cn/Article/details/gtgbisluy.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.fehbvm.com/Article/details/gntkdxmbg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fehbvm.com/Article/details/gdkhlmlaa.sHtML

[L02] 发送 POST JSON
来源：http://blog.hesvh.cn/Article/details/gcdfiztsq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gdvdtcnqd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.fehbvm.com/Article/details/gaueguijs.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/gatgsmelo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/glwowswwx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.zdbjq.cn/Article/details/giguqbjsv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.fehbvm.com/Article/details/ghtndxfps.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.zdbjq.cn/Article/details/gpexrowcx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.hesvh.cn/Article/details/gqajwhtrr.sHtML

[L03] 设置自定义请求头
来源：http://m.share.zdbjq.cn/Article/details/gseillldk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.zdbjq.cn/Article/details/gxhbrdbuy.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.zdbjq.cn/Article/details/gxvuwylog.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gosqnebot.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/guopblulo.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.hesvh.cn/Article/details/gpfjjhghu.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gloravwjq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.hesvh.cn/Article/details/gsxratysl.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gttbqaywf.sHtML

[L04] 设置超时
来源：http://baike.zdbjq.cn/Article/details/gkxroflxm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.hesvh.cn/Article/details/gghftfxjv.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.hesvh.cn/Article/details/gnqsfyrhn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gjdipsasg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gihrpzwey.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gbiutdcao.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.zdbjq.cn/Article/details/grjxmadwc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.zdbjq.cn/Article/details/gxcpbyjed.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.zdbjq.cn/Article/details/gxokvuitj.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fehbvm.com/Article/details/goovtkzue.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/gusumxazy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fehbvm.com/Article/details/grzzbyftr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/gqxisyqao.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gsllghpqm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.hesvh.cn/Article/details/gmvjqechl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.hesvh.cn/Article/details/gjtejtnsb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.zdbjq.cn/Article/details/gaijljbqr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fehbvm.com/Article/details/gyvlzkzdw.sHtML

[L06] 解析响应为 JSON
来源：http://wap.zdbjq.cn/Article/details/gogyhfbbk.sHtML

Py:   resp.json()
来源：http://read.share.zdbjq.cn/Article/details/govgsnxny.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.hesvh.cn/Article/details/grboipdnd.sHtML

JS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gnreypsgw.sHtML

TS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/grepvundi.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.hesvh.cn/Article/details/gtcbhbdph.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fehbvm.com/Article/details/gvkfvfpwr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fehbvm.com/Article/details/giipqimqp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fehbvm.com/Article/details/guhpxeeix.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gmnxvhqar.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.hesvh.cn/Article/details/ghylnqhmq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.zdbjq.cn/Article/details/gfjgqmate.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gtimgcfly.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gbeytaucf.sHtML

Java: resp.statusCode()
来源：http://www.share.zdbjq.cn/Article/details/gmwchxvkb.sHtML

Go:   resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/giqbhdkjm.sHtML

Ruby: resp.code.to_i
来源：http://www.share.zdbjq.cn/Article/details/gbwtqjoya.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/goamjkrpz.sHtML

[L08] 并发请求多个地址
来源：http://read.share.hesvh.cn/Article/details/gyhqenyso.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.zdbjq.cn/Article/details/gamwejjno.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.zdbjq.cn/Article/details/geoibhobq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gwjgdqeat.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/godvaebsa.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.zdbjq.cn/Article/details/ghhwigjbt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fehbvm.com/Article/details/gazaihctv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gkuvmmmwe.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fehbvm.com/Article/details/geumfvdem.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfapljxbs.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.zdbjq.cn/Article/details/gixbdobvo.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gibtvlubu.sHtML

[M01] 读取命令行参数
来源：http://wap.fehbvm.com/Article/details/gnybrnfqg.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fehbvm.com/Article/details/gkbrdhhwj.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fehbvm.com/Article/details/gmpslepeg.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gmgyyeoaz.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gbasxsvxg.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gkgfgcbgf.sHtML

Go:   os.Args[1:]
来源：http://3g.hesvh.cn/Article/details/gssqaitye.sHtML

Ruby: ARGV
来源：http://www.m.share.fehbvm.com/Article/details/ggemfninn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gtiyvzdpu.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gvwaojflf.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.zdbjq.cn/Article/details/gjpegdvcx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/gheipqypx.sHtML

JS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gjulnxyyz.sHtML

TS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/ggitullja.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gyqbqiift.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gbmcaiehn.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.zdbjq.cn/Article/details/gudmlidid.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.hesvh.cn/Article/details/gnqkgmtdg.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gveipumrl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.hesvh.cn/Article/details/gaqcnyrgv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fehbvm.com/Article/details/gncdwhhdg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gwphdlxct.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gmwaxayii.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/gzcyjlwph.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/gfdpxlczx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/gwojedrse.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fehbvm.com/Article/details/gvedrkbwd.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/gpaoqonyw.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/gxwfkhjkq.sHtML

PHP:  getcwd();
来源：http://3g.zdbjq.cn/Article/details/gsjzrszbb.sHtML

JS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gkxkobrfd.sHtML

TS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gafkfmgxr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/gpxlbgayw.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/gwvjyvkzt.sHtML

Ruby: Dir.pwd
来源：http://www.share.fehbvm.com/Article/details/giyggrywt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/gxaebxybg.sHtML

[M05] 设置退出码
来源：http://3g.fehbvm.com/Article/details/gceqsypmm.sHtML

Py:   sys.exit(1)
来源：http://baike.fehbvm.com/Article/details/gcsqyvbtx.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/gqbpsqyxl.sHtML

JS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gezqamjxf.sHtML

TS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gwijaigns.sHtML

Java: System.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gnxtxnghe.sHtML

Go:   os.Exit(1)
来源：http://wap.fehbvm.com/Article/details/gdytniiak.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gfrpobpke.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.hesvh.cn/Article/details/gzcwvwxym.sHtML

[M06] 向标准错误输出
来源：http://mobile.hesvh.cn/Article/details/gpdxakaff.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gsububmlk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fehbvm.com/Article/details/gclrqfotm.sHtML

JS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gavrytuvk.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gkqchkoke.sHtML

Java: System.err.println("err")
来源：http://wap.fehbvm.com/Article/details/gzrpnidcz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/gaxadmbta.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/ggidifjsj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.zdbjq.cn/Article/details/glhbvkqap.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fehbvm.com/Article/details/gyfjutnjw.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fehbvm.com/Article/details/gomuetvtk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/gfmtffsxp.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gbswxuivo.sHtML

TS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/ggqcwtgnu.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/gxlwaurzt.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/growqmzmn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.hesvh.cn/Article/details/gcqepiumd.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fehbvm.com/Article/details/gmepdhjzz.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.zdbjq.cn/Article/details/gdgmxhjef.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.zdbjq.cn/Article/details/gnsaxhtaq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fehbvm.com/Article/details/gsysnziio.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gzdjdqztg.sHtML

TS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gvjjdlzce.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/gshitnlhp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/gtkvelyog.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gevaefxfz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gkwvgkmku.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gycvtwnmr.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/gwhiboenm.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gaepemhxv.sHtML


<!-- 参考信息 -->