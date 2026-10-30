代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.fehbvm.com/Article/details/gltvufwey.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.fehbvm.com/Article/details/gfllsauea.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fehbvm.com/Article/details/gasrauigw.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.zdbjq.cn/Article/details/ggrhncgir.sHtML

[J03] 字符串解析为日期
来源：http://www.share.zdbjq.cn/Article/details/gpzczofmp.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.hesvh.cn/Article/details/gflzyhwix.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.zdbjq.cn/Article/details/gxgkpcjar.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gdmwvrdee.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/glhbpvpms.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gvpkqwocd.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/grpxiarfw.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gjwaotnhk.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.zdbjq.cn/Article/details/gxbnfvbjo.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.zdbjq.cn/Article/details/ghwkqmmpq.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.hesvh.cn/Article/details/gwigxalsp.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.fehbvm.com/Article/details/gqafezayh.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.zdbjq.cn/Article/details/gqegrpcvh.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.zdbjq.cn/Article/details/gjwrgymxv.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.zdbjq.cn/Article/details/gdriltyky.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.hesvh.cn/Article/details/gwznmcrno.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.hesvh.cn/Article/details/gxbybucgt.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.hesvh.cn/Article/details/gjszfojoo.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.fehbvm.com/Article/details/gppclxbzl.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.hesvh.cn/Article/details/gxeiebgnz.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.fehbvm.com/Article/details/gauklzzor.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.zdbjq.cn/Article/details/gfmumgfxe.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.hesvh.cn/Article/details/gdicbopcg.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.hesvh.cn/Article/details/gphohvaum.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.fehbvm.com/Article/details/gfmvfuvlm.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.zdbjq.cn/Article/details/gxphwbjgq.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.fehbvm.com/Article/details/ggvanaiqy.sHtML

[J06] 计算两时间之差
来源：http://3g.fehbvm.com/Article/details/gtnkslxcv.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.fehbvm.com/Article/details/grzrqvajm.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.fehbvm.com/Article/details/gcxquajov.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.hesvh.cn/Article/details/glepwoklr.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.fehbvm.com/Article/details/gknlstjsn.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.hesvh.cn/Article/details/gjmykwgdr.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.hesvh.cn/Article/details/gghnotouo.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.fehbvm.com/Article/details/gtbcbmirc.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.zdbjq.cn/Article/details/gxcodgdhn.sHtML

[J07] 比较两个日期
来源：http://wap.hesvh.cn/Article/details/gvchvgozr.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/goxxbuunw.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.fehbvm.com/Article/details/gupsbhbws.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.fehbvm.com/Article/details/gkcabooch.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.zdbjq.cn/Article/details/gllvfomub.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.hesvh.cn/Article/details/glgtlfsng.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.hesvh.cn/Article/details/gejvhpmpe.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.fehbvm.com/Article/details/gotzhdoji.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.fehbvm.com/Article/details/gamppbtky.sHtML

[J08] 提取年月日与星期
来源：http://m.share.hesvh.cn/Article/details/gfajnzdfv.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.fehbvm.com/Article/details/gkqfgwtfy.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.zdbjq.cn/Article/details/gbujpadvv.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.hesvh.cn/Article/details/gtwlixunf.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.hesvh.cn/Article/details/gwirubjcy.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.fehbvm.com/Article/details/gfklrxfkw.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.zdbjq.cn/Article/details/gqxtgjvhx.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.zdbjq.cn/Article/details/gwgfjqdhz.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.zdbjq.cn/Article/details/ginweckhz.sHtML

[J09] 时区处理
来源：http://wap.zdbjq.cn/Article/details/grdhuylys.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.fehbvm.com/Article/details/ghdhzxyax.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.zdbjq.cn/Article/details/gquiwxejp.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fehbvm.com/Article/details/gksdkzwut.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.zdbjq.cn/Article/details/gnoojehjf.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.hesvh.cn/Article/details/gwedkgtwe.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.fehbvm.com/Article/details/gzjicqvub.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.fehbvm.com/Article/details/gbjncfmrv.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.zdbjq.cn/Article/details/ggjhaszsa.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.hesvh.cn/Article/details/gbtdqzhyz.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.zdbjq.cn/Article/details/gfaprpnxv.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.fehbvm.com/Article/details/gdgfhkhtg.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.hesvh.cn/Article/details/gfdlqnbun.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.hesvh.cn/Article/details/gmfgvizib.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.zdbjq.cn/Article/details/gdkkletid.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.hesvh.cn/Article/details/gcjxoezvt.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.hesvh.cn/Article/details/gzbbovkdo.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.fehbvm.com/Article/details/gryzdqwai.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/golmzfvub.sHtML

K. JSON 与序列化
来源：http://www.m.share.zdbjq.cn/Article/details/grjlilchr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gspnaxzyx.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.zdbjq.cn/Article/details/gscrnfxnq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.zdbjq.cn/Article/details/galusfiqf.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.fehbvm.com/Article/details/ghcpahgmc.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.zdbjq.cn/Article/details/gulrnprfl.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.hesvh.cn/Article/details/gzzgvfntr.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.zdbjq.cn/Article/details/gbthpdzgq.sHtML

Go:   json.Marshal(obj)
来源：http://baike.zdbjq.cn/Article/details/gyuxhmggy.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.hesvh.cn/Article/details/gwtorywfl.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.zdbjq.cn/Article/details/gziakmnvl.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.hesvh.cn/Article/details/gnizgdghz.sHtML

Py:   json.loads(s)
来源：http://baike.zdbjq.cn/Article/details/gkhctlfpx.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.fehbvm.com/Article/details/gkdlmtgzf.sHtML

JS:   JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/gkhojcoxg.sHtML

TS:   JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/gldttermv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gcwmkqwca.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/gzqzbdsya.sHtML

Ruby: JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gawfxgqbn.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.fehbvm.com/Article/details/gzqvakpja.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.hesvh.cn/Article/details/gbzorghhe.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.zdbjq.cn/Article/details/ghqybzxnu.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.fehbvm.com/Article/details/gpyefdafy.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fehbvm.com/Article/details/glsccujqa.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gqktvjpec.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.hesvh.cn/Article/details/gtfzkfeav.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.hesvh.cn/Article/details/gdqhgennx.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.hesvh.cn/Article/details/gzyrheail.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.zdbjq.cn/Article/details/gwnkgalvc.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.fehbvm.com/Article/details/ghszdryrl.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.hesvh.cn/Article/details/geqdhzbip.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.zdbjq.cn/Article/details/gbbbdhkcv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.zdbjq.cn/Article/details/giusdrtfh.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/gumchmfzv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gyvikrozl.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.zdbjq.cn/Article/details/gundvhniz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/gcsdlemwq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gntppsnoc.sHtML

[K05] 深拷贝对象
来源：http://read.share.hesvh.cn/Article/details/gfulgwhue.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.fehbvm.com/Article/details/gjpdifvnr.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.zdbjq.cn/Article/details/gcucygnxl.sHtML

JS:   structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gazdahzdj.sHtML

TS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gpvcfmmxd.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.hesvh.cn/Article/details/giwburwjp.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.zdbjq.cn/Article/details/gcnyylzji.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.zdbjq.cn/Article/details/gpxuffsdf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.zdbjq.cn/Article/details/gykymibby.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.fehbvm.com/Article/details/gkwyopkii.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.hesvh.cn/Article/details/glbhiyrwd.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.fehbvm.com/Article/details/gqbjrmfoc.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/govwlykxv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gcllunnzr.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.zdbjq.cn/Article/details/gwmzfkglk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gxapqzivn.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gqtrjtkdg.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/ghvxpnngh.sHtML

[K07] 进制转换
来源：http://www.m.share.zdbjq.cn/Article/details/gtsqtdaks.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gennmofuo.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.fehbvm.com/Article/details/gofcsuvkl.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/giiiqxruu.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/glhxqpqui.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gfslzhpqk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.fehbvm.com/Article/details/ggrxnaasy.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.fehbvm.com/Article/details/guehlramn.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gdfjcwrfa.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.hesvh.cn/Article/details/grmkyrkhn.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fehbvm.com/Article/details/grhjiydjb.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.fehbvm.com/Article/details/gnbktpysz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/gzcjhqdao.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/gzojdetza.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fehbvm.com/Article/details/gtlmxzxir.sHtML

Go:   encoding/gob
来源：http://wap.hesvh.cn/Article/details/gexmgbtaf.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.fehbvm.com/Article/details/gibxtrexp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/geddynyne.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmgjmarxe.sHtML

L. 网络请求
来源：http://baike.fehbvm.com/Article/details/gmznsatcr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gsemhaiwi.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.fehbvm.com/Article/details/grgyaovmg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.hesvh.cn/Article/details/gpcfvlqbz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.hesvh.cn/Article/details/gvdogghmw.sHtML

JS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gwhercapi.sHtML

TS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/grsylxwfx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.hesvh.cn/Article/details/glignsxpc.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.hesvh.cn/Article/details/gvwnoxaym.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.fehbvm.com/Article/details/gmrgbescg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.hesvh.cn/Article/details/gwsxwdwcw.sHtML

[L02] 发送 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gmuwgvhbb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gyepwvsup.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.zdbjq.cn/Article/details/gmutstxjd.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/giiitxtbm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/gjsmnkbpo.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.hesvh.cn/Article/details/gyilhenkr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.zdbjq.cn/Article/details/gtpkpeuni.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.hesvh.cn/Article/details/ghifczxzv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.hesvh.cn/Article/details/gcosvyzvj.sHtML

[L03] 设置自定义请求头
来源：http://baike.fehbvm.com/Article/details/gcqzgnmbb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.zdbjq.cn/Article/details/gzgdypfjj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.hesvh.cn/Article/details/gryoyozuv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gvsacsavd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gzzybcpps.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.hesvh.cn/Article/details/gdfprtrae.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gjjrrspyj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.hesvh.cn/Article/details/gdekrausk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gpvvmovfl.sHtML

[L04] 设置超时
来源：http://m.share.fehbvm.com/Article/details/gfkuwebfl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fehbvm.com/Article/details/gkbyodywb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.zdbjq.cn/Article/details/geaxrxlcp.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/ghoxtzxmd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gacpeihym.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.zdbjq.cn/Article/details/gsxsamzxy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.zdbjq.cn/Article/details/geqrnhekr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.fehbvm.com/Article/details/getgwccvv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fehbvm.com/Article/details/gztlfjqpk.sHtML

[L05] 上传文件（multipart）
来源：http://wap.zdbjq.cn/Article/details/gawyshrff.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.zdbjq.cn/Article/details/gqnxspboi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fehbvm.com/Article/details/gxziuojez.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gfutjujdg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gphiildiq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/gaooangjt.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.zdbjq.cn/Article/details/gyhvgtwkh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fehbvm.com/Article/details/gfzkknaxm.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.fehbvm.com/Article/details/gmmpsprft.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gcsdexfab.sHtML

Py:   resp.json()
来源：http://3g.hesvh.cn/Article/details/gnzkhcfsa.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.hesvh.cn/Article/details/gzpqmvvoj.sHtML

JS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gxjcssede.sHtML

TS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gukimeqem.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gpfmzhqgb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.zdbjq.cn/Article/details/gsnlhzkmw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fehbvm.com/Article/details/gzflxlkvq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fehbvm.com/Article/details/gegnbatxz.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/ghlcpnozv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.hesvh.cn/Article/details/gtugryfap.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.hesvh.cn/Article/details/gmorgrjej.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gljozfeay.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/geijdeapq.sHtML

Java: resp.statusCode()
来源：http://www.m.share.zdbjq.cn/Article/details/gjbwgmeel.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gcgkeqrqj.sHtML

Ruby: resp.code.to_i
来源：http://mobile.hesvh.cn/Article/details/ghmewnwzk.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gvtmzlmpg.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.hesvh.cn/Article/details/geuxoxvyr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.zdbjq.cn/Article/details/gtwfdgrsj.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fehbvm.com/Article/details/gbwacvgew.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gcqhnjhse.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gvbffjpyj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.hesvh.cn/Article/details/gxskzwvre.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.hesvh.cn/Article/details/gvydmhmlj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gxvyujhwg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.fehbvm.com/Article/details/grtrxeltr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfrxgzinx.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.zdbjq.cn/Article/details/ghxcjwyyj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfwvnvize.sHtML

[M01] 读取命令行参数
来源：http://mobile.zdbjq.cn/Article/details/geqvfaedx.sHtML

Py:   sys.argv[1:]
来源：http://wap.zdbjq.cn/Article/details/gdopdsepy.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.zdbjq.cn/Article/details/gecceyhkh.sHtML

JS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gydppdmbl.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gkdrllrcj.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/grqiytveg.sHtML

Go:   os.Args[1:]
来源：http://mobile.fehbvm.com/Article/details/gcmydzgim.sHtML

Ruby: ARGV
来源：http://3g.fehbvm.com/Article/details/gsqxzadlk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.fehbvm.com/Article/details/gxmhzlbck.sHtML

[M02] 读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gnhopesao.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fehbvm.com/Article/details/gndfzjcwe.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/guecqslwg.sHtML

JS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gbvdkjqey.sHtML

TS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gcoxhymxs.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gzyuchvms.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.hesvh.cn/Article/details/glpadosay.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fehbvm.com/Article/details/ghuzrhjxb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gudtzdphv.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gebikeqvh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/gbvkwykyg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.zdbjq.cn/Article/details/gwiqwrrdo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/glbqvikxg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gubjkuyfx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fehbvm.com/Article/details/ggwmxpudi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fehbvm.com/Article/details/gaxwpucwh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fehbvm.com/Article/details/gjmkeyptq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/gfrhmcwxa.sHtML

[M04] 获取当前工作目录
来源：http://blog.fehbvm.com/Article/details/grhvlamew.sHtML

Py:   os.getcwd()
来源：http://blog.hesvh.cn/Article/details/gbzrhshvu.sHtML

PHP:  getcwd();
来源：http://mobile.zdbjq.cn/Article/details/glinrlexb.sHtML

JS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/ghyhhbvzu.sHtML

TS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/glhaxklqq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/gsdqlnqmt.sHtML

Go:   os.Getwd()
来源：http://read.share.fehbvm.com/Article/details/gjrtpynek.sHtML

Ruby: Dir.pwd
来源：http://wap.zdbjq.cn/Article/details/gpzvixrrr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.hesvh.cn/Article/details/gilxaykoc.sHtML

[M05] 设置退出码
来源：http://www.blog.fehbvm.com/Article/details/gbshhkhln.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/gkqqrfodf.sHtML

PHP:  exit(1);
来源：http://blog.hesvh.cn/Article/details/gctydepbp.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gtdmxjqnd.sHtML

TS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/ggcceakpn.sHtML

Java: System.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gczibsqop.sHtML

Go:   os.Exit(1)
来源：http://read.share.hesvh.cn/Article/details/gksomxudx.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gmbjsnkdy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.hesvh.cn/Article/details/gkebgjwtx.sHtML

[M06] 向标准错误输出
来源：http://3g.hesvh.cn/Article/details/ghpazsgmd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gxrweywnj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fehbvm.com/Article/details/gbczndzov.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gcbuptpvo.sHtML

TS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/ghkfpnlnw.sHtML

Java: System.err.println("err")
来源：http://mobile.hesvh.cn/Article/details/gjockwxly.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/geysfvlbo.sHtML

Ruby: warn "err"
来源：http://blog.hesvh.cn/Article/details/gflbliupj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/gqufclkbp.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/gghservea.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.hesvh.cn/Article/details/ghasuwihz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.hesvh.cn/Article/details/gexrrvfpj.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gzdrtwnjq.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gxdbfjykb.sHtML

Java: public static void main(String[] args)
来源：http://blog.hesvh.cn/Article/details/gaqcqgvtq.sHtML

Go:   func main()
来源：http://3g.zdbjq.cn/Article/details/ggefhavbd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.hesvh.cn/Article/details/gzdkshuih.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.zdbjq.cn/Article/details/gkbflkfrh.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.zdbjq.cn/Article/details/gtqfcsfao.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/gcidvzeew.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/gqswkwzko.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gekxokwsb.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gvckbotix.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/gfujtbfge.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/gebhyxisf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/gpvaaorgn.sHtML


<!-- 参考信息 -->