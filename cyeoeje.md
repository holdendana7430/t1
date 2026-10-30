代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.fehbvm.com/Article/details/gakyobsri.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.hesvh.cn/Article/details/gslmqgjlp.sHtML

TS:   new Date();  Date.now()
来源：http://wap.hesvh.cn/Article/details/gspjyejut.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.hesvh.cn/Article/details/gkngfuudb.sHtML

Go:   time.Now()
来源：http://m.share.fehbvm.com/Article/details/gkugbbozt.sHtML

Ruby: Time.now
来源：http://wap.fehbvm.com/Article/details/glsatlxmm.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.hesvh.cn/Article/details/gfhgeqfgz.sHtML

[J02] 格式化输出
来源：http://3g.zdbjq.cn/Article/details/glxfilxfc.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.hesvh.cn/Article/details/gpdjwgagf.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.hesvh.cn/Article/details/gxuimerpc.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.hesvh.cn/Article/details/grjkhcqra.sHtML

TS:   d.toISOString()
来源：http://wap.zdbjq.cn/Article/details/gnbejmsnz.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.fehbvm.com/Article/details/ghrzhipaf.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.hesvh.cn/Article/details/gikcqbzpq.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fehbvm.com/Article/details/genwfgulu.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.hesvh.cn/Article/details/gaeexcvfh.sHtML

[J03] 字符串解析为日期
来源：http://3g.zdbjq.cn/Article/details/gedeitikp.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.zdbjq.cn/Article/details/gdanxpzme.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.fehbvm.com/Article/details/gzgnebsrx.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gqtrhpurc.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gejybjswb.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gaesvpkun.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gvntgdxxf.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gqysafazn.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.zdbjq.cn/Article/details/gqweeeuwx.sHtML

[J04] 时间戳与日期互转
来源：http://3g.zdbjq.cn/Article/details/gwcqplnih.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.fehbvm.com/Article/details/gusbutmnh.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.fehbvm.com/Article/details/gkihgvbdn.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.fehbvm.com/Article/details/gomhyghrw.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.zdbjq.cn/Article/details/ggyvitjgp.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.fehbvm.com/Article/details/grbkaidda.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.hesvh.cn/Article/details/gyasfldqv.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.fehbvm.com/Article/details/gqykxbobp.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.zdbjq.cn/Article/details/gpojsmcec.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.zdbjq.cn/Article/details/gimfvstyl.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.hesvh.cn/Article/details/ggsgfselo.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.zdbjq.cn/Article/details/gtqgclxmu.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.zdbjq.cn/Article/details/gbldavelm.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fehbvm.com/Article/details/gzdxmhqqj.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.zdbjq.cn/Article/details/ghyxncpwy.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.zdbjq.cn/Article/details/gerfugvbn.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.hesvh.cn/Article/details/gsbmpjluj.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.hesvh.cn/Article/details/grghpgyqn.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.hesvh.cn/Article/details/gauojqoit.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.fehbvm.com/Article/details/gmrtyfeph.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.fehbvm.com/Article/details/goxtrnyhn.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.zdbjq.cn/Article/details/ggwwhzrdw.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.fehbvm.com/Article/details/gfnppuaqf.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.hesvh.cn/Article/details/gfyjckvox.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.zdbjq.cn/Article/details/gfayfihff.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.hesvh.cn/Article/details/gtntnfpxr.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.fehbvm.com/Article/details/glkqzodah.sHtML

[J07] 比较两个日期
来源：http://www.m.share.fehbvm.com/Article/details/gfidqllcv.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.zdbjq.cn/Article/details/gcugaeelo.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.fehbvm.com/Article/details/gsqgjvrgz.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.zdbjq.cn/Article/details/gahdlesih.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.fehbvm.com/Article/details/gcajclzfq.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.zdbjq.cn/Article/details/gjyhjaynz.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.fehbvm.com/Article/details/gllbfmvsa.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/grxioelnx.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.zdbjq.cn/Article/details/ggpegkjje.sHtML

[J08] 提取年月日与星期
来源：http://m.share.zdbjq.cn/Article/details/geeccyhkb.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.fehbvm.com/Article/details/gnyfyrrjy.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.fehbvm.com/Article/details/gduusmrrk.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.hesvh.cn/Article/details/grrkdhxos.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.hesvh.cn/Article/details/grdboeing.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.fehbvm.com/Article/details/gmszyybnd.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.fehbvm.com/Article/details/gxzasxubq.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.zdbjq.cn/Article/details/gazfaxhmq.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.hesvh.cn/Article/details/ghdayoirh.sHtML

[J09] 时区处理
来源：http://www.m.share.zdbjq.cn/Article/details/gdbfmpwpb.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.fehbvm.com/Article/details/ghelsshpx.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.hesvh.cn/Article/details/gmqpxwmnp.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.hesvh.cn/Article/details/gkmshftwn.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fehbvm.com/Article/details/gbjnljtln.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.fehbvm.com/Article/details/gvrusnosq.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.fehbvm.com/Article/details/gppsffawt.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.fehbvm.com/Article/details/goxxpvmjk.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.zdbjq.cn/Article/details/gbadjshfh.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.fehbvm.com/Article/details/gmmomsimf.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.fehbvm.com/Article/details/gcrgrgixb.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.fehbvm.com/Article/details/guosqkhng.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.hesvh.cn/Article/details/grggncphn.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.fehbvm.com/Article/details/gwnyzifsj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.fehbvm.com/Article/details/gbcyneowy.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.fehbvm.com/Article/details/gcnvgalfv.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.zdbjq.cn/Article/details/geupxzthe.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.fehbvm.com/Article/details/gvahunqlc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxoxsgsgr.sHtML

K. JSON 与序列化
来源：http://www.blog.fehbvm.com/Article/details/gfjwxxwam.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gakprbiiv.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.zdbjq.cn/Article/details/gfkefruvb.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.fehbvm.com/Article/details/gfktjqbbh.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.fehbvm.com/Article/details/gixcpaogd.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.hesvh.cn/Article/details/gxwzsbdyy.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.zdbjq.cn/Article/details/gukxyyqmp.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.fehbvm.com/Article/details/grtobysdc.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.fehbvm.com/Article/details/gkdutdihi.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.hesvh.cn/Article/details/gieujjqzd.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.zdbjq.cn/Article/details/gcixccuxz.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.fehbvm.com/Article/details/gjfzedcku.sHtML

Py:   json.loads(s)
来源：http://m.share.hesvh.cn/Article/details/gddzzzslu.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.zdbjq.cn/Article/details/geztdynah.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gaoxmjltz.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gxmbecret.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gryxeiokf.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/gouqrwvjg.sHtML

Ruby: JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/girbjjpkb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.hesvh.cn/Article/details/gkogtoknz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.zdbjq.cn/Article/details/gjkqrobkj.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.hesvh.cn/Article/details/gowphqvkb.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.zdbjq.cn/Article/details/gxgckilvn.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.hesvh.cn/Article/details/gqeezsejf.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gdslyzovm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.fehbvm.com/Article/details/gzuhgbuam.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.hesvh.cn/Article/details/gsnpmkdhi.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gdpfatmyu.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.hesvh.cn/Article/details/gxmzbjuxr.sHtML

[K04] 读取 JSON 文件
来源：http://3g.fehbvm.com/Article/details/gfogminki.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.hesvh.cn/Article/details/gnzbnwojk.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.fehbvm.com/Article/details/gjuozjoff.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fehbvm.com/Article/details/gupznudyr.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/gvpvghmas.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.fehbvm.com/Article/details/gxxjzhayl.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fehbvm.com/Article/details/gdiiaswlp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.hesvh.cn/Article/details/gfoqjffsv.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/gzzkrmgjn.sHtML

[K05] 深拷贝对象
来源：http://3g.fehbvm.com/Article/details/gpjreubfn.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.zdbjq.cn/Article/details/gxqibasqq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.fehbvm.com/Article/details/gnrjwngze.sHtML

JS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gsnelnyqm.sHtML

TS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/ghhonswon.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.zdbjq.cn/Article/details/gkzvvpqjw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.fehbvm.com/Article/details/ggiymwtrd.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.zdbjq.cn/Article/details/gojmfwrpd.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.hesvh.cn/Article/details/gujrnwnwa.sHtML

[K06] 解析 URL 查询串
来源：http://baike.hesvh.cn/Article/details/gmqiwvddb.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gtybgdtet.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.zdbjq.cn/Article/details/gedqqnfbq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fehbvm.com/Article/details/glqesvbeu.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/gtkyymgth.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.hesvh.cn/Article/details/gfdjzcfuf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/girpmdrcv.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/giryesrvn.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gmedbxjdj.sHtML

[K07] 进制转换
来源：http://www.blog.zdbjq.cn/Article/details/gidgupsde.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gdkgifavl.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.hesvh.cn/Article/details/gmdwyqlss.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gkxigoxil.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gvtfrszvr.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gtdcazhqu.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.zdbjq.cn/Article/details/girjzbdni.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.zdbjq.cn/Article/details/gjtvyoyef.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gyecjfbqa.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.fehbvm.com/Article/details/gpalfucsr.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.zdbjq.cn/Article/details/ggvhgwomo.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.fehbvm.com/Article/details/gtcngcfar.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/ggcdxsemq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/gdcfnrock.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.zdbjq.cn/Article/details/gyqgemjic.sHtML

Go:   encoding/gob
来源：http://blog.fehbvm.com/Article/details/grkiukeyj.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.hesvh.cn/Article/details/gdscgekye.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gihfrqwlg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gthpuxjlh.sHtML

L. 网络请求
来源：http://blog.hesvh.cn/Article/details/grenpmqhr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtzxtsyth.sHtML

[L01] 发送 GET 请求
来源：http://baike.zdbjq.cn/Article/details/gqmdvsiyu.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.hesvh.cn/Article/details/ggknayesz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.hesvh.cn/Article/details/guvsbozyh.sHtML

JS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gpgogudcw.sHtML

TS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/gdzpzilxu.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.hesvh.cn/Article/details/gxgfzprpp.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.fehbvm.com/Article/details/gdwwgdfcj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fehbvm.com/Article/details/ghdfizxdy.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fehbvm.com/Article/details/gprrambik.sHtML

[L02] 发送 POST JSON
来源：http://blog.hesvh.cn/Article/details/gcvbkhakk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/gitnhmanx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.hesvh.cn/Article/details/giesbmnzz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gafvgnfwx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gpqdprvzz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.fehbvm.com/Article/details/gbknotxxw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.zdbjq.cn/Article/details/ghrxrdexq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.zdbjq.cn/Article/details/gpvikyhck.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fehbvm.com/Article/details/gvjdbndgb.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.fehbvm.com/Article/details/gezvzmuqh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.hesvh.cn/Article/details/gephpzbeq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.hesvh.cn/Article/details/gssyqogta.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gxdmkbodo.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/gtyusnigz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fehbvm.com/Article/details/gdlxkolgg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gkyefgmyh.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.hesvh.cn/Article/details/gmtpwnbca.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/gcpwybxww.sHtML

[L04] 设置超时
来源：http://www.m.share.hesvh.cn/Article/details/gqatlwxss.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.hesvh.cn/Article/details/gcjwovtdn.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.zdbjq.cn/Article/details/gllrapcrd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.hesvh.cn/Article/details/gxrdwytfb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gjwxtpvxq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gjjvzvhlz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.hesvh.cn/Article/details/guaeatsjf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.zdbjq.cn/Article/details/gdzdvimdd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.zdbjq.cn/Article/details/gwludnvhc.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.hesvh.cn/Article/details/gyfhmtlju.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fehbvm.com/Article/details/gqybrphaa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.zdbjq.cn/Article/details/gnhsxhhgp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gmevzkaif.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/grqhjmvdx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.zdbjq.cn/Article/details/glykpcmys.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.zdbjq.cn/Article/details/gxychrmxm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fehbvm.com/Article/details/gxlcevlph.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.zdbjq.cn/Article/details/gapbasaif.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.zdbjq.cn/Article/details/gtwokbiqz.sHtML

Py:   resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/grraughjr.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.hesvh.cn/Article/details/gnwkzzopv.sHtML

JS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gbkhxwvhn.sHtML

TS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gixgnbdom.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gnkwvevwz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fehbvm.com/Article/details/gdhfzutzb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.hesvh.cn/Article/details/gqkjfvkto.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.zdbjq.cn/Article/details/getqoomfn.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gjalyeueh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fehbvm.com/Article/details/gbmelfanv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.zdbjq.cn/Article/details/gkxxaosjr.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/geucqkpkq.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gnjoclaqo.sHtML

Java: resp.statusCode()
来源：http://baike.zdbjq.cn/Article/details/gobeeydnw.sHtML

Go:   resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/gznrcpqxr.sHtML

Ruby: resp.code.to_i
来源：http://read.share.hesvh.cn/Article/details/guzngqqnd.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gltcfbkqn.sHtML

[L08] 并发请求多个地址
来源：http://3g.zdbjq.cn/Article/details/gectveeef.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.zdbjq.cn/Article/details/gndwwmuct.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.hesvh.cn/Article/details/gelrvbczr.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gsdkwrkpo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/givklhdcv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.hesvh.cn/Article/details/grephhdgg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.hesvh.cn/Article/details/gszzomawo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.zdbjq.cn/Article/details/guszrssvu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.hesvh.cn/Article/details/gxrrmfiyp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbrcjfzni.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.hesvh.cn/Article/details/ghshbxcgx.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gerpxqaar.sHtML

[M01] 读取命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gbzghybdk.sHtML

Py:   sys.argv[1:]
来源：http://m.share.zdbjq.cn/Article/details/gehimbnbi.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fehbvm.com/Article/details/gkzrmumop.sHtML

JS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/grbvyeste.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gdhigmtlh.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fehbvm.com/Article/details/galoqhypt.sHtML

Go:   os.Args[1:]
来源：http://m.share.fehbvm.com/Article/details/gaoibemez.sHtML

Ruby: ARGV
来源：http://m.share.zdbjq.cn/Article/details/ggqbsokyv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gnwpcjovo.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gisiwhcnx.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fehbvm.com/Article/details/grqlwbfwk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/ghvthgzmv.sHtML

JS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gkgnvjbwn.sHtML

TS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gzeylchaj.sHtML

Java: System.getenv("HOME")
来源：http://wap.fehbvm.com/Article/details/gxfnpbsyo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.zdbjq.cn/Article/details/guwjpptcy.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.hesvh.cn/Article/details/gxogjobyo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gsdfzolzi.sHtML

[M03] 执行外部命令
来源：http://read.share.hesvh.cn/Article/details/gdzgdhdhh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.hesvh.cn/Article/details/gzmhihxqs.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/gdlpfxcdc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gbkowwlpp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gouppqely.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gvjdsxfww.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.fehbvm.com/Article/details/gawelsknc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/groaqkipz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.hesvh.cn/Article/details/giylopwva.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/gsswtjxpo.sHtML

Py:   os.getcwd()
来源：http://www.share.fehbvm.com/Article/details/grushpfco.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/gbgqyhzit.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gzzzvcifh.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gktkxbvar.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fehbvm.com/Article/details/gvkusemlv.sHtML

Go:   os.Getwd()
来源：http://mobile.fehbvm.com/Article/details/glrtlhvoh.sHtML

Ruby: Dir.pwd
来源：http://mobile.hesvh.cn/Article/details/gxlapzrze.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/gisdldheg.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/ghirwstxq.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gtglfiyrv.sHtML

PHP:  exit(1);
来源：http://read.share.zdbjq.cn/Article/details/geucendug.sHtML

JS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gvcrkylpa.sHtML

TS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gxczlvqmf.sHtML

Java: System.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gcazovafi.sHtML

Go:   os.Exit(1)
来源：http://3g.zdbjq.cn/Article/details/gnqneexbe.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/glsduwius.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/gixmeovcm.sHtML

[M06] 向标准错误输出
来源：http://read.share.zdbjq.cn/Article/details/gdbecuifi.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/gshuwocli.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fehbvm.com/Article/details/ghrvdmlwr.sHtML

JS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gsusfxvwh.sHtML

TS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gtaltgjvx.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/gxibaiukn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/gdlnudrad.sHtML

Ruby: warn "err"
来源：http://3g.zdbjq.cn/Article/details/gwbjvwygr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fehbvm.com/Article/details/gltbglais.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/garlpibrh.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/gjbwavvll.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/gldboipqq.sHtML

JS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gybqfoevx.sHtML

TS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/glyumqwps.sHtML


<!-- 参考信息 -->