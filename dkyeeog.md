代发 wailian999

J. 日期与时间
来源：http://m.share.zdbjq.cn/Article/details/gtbgbbgti.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gethynjbg.sHtML

[J01] 获取当前时间
来源：http://blog.zdbjq.cn/Article/details/gzgwdvnhc.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.zdbjq.cn/Article/details/gyxdxkwpw.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.fehbvm.com/Article/details/geuwofmjf.sHtML

JS:   new Date();  Date.now()
来源：http://blog.fehbvm.com/Article/details/gczmtcupu.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.zdbjq.cn/Article/details/gtotgmvbx.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.zdbjq.cn/Article/details/girbdbfqx.sHtML

Go:   time.Now()
来源：http://www.share.fehbvm.com/Article/details/gadzxvijw.sHtML

Ruby: Time.now
来源：http://3g.zdbjq.cn/Article/details/gqtaeoicm.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.fehbvm.com/Article/details/gvegrzwlo.sHtML

[J02] 格式化输出
来源：http://m.share.zdbjq.cn/Article/details/grwscjncr.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fehbvm.com/Article/details/grkpkkjec.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.hesvh.cn/Article/details/gvtsxpowf.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.fehbvm.com/Article/details/ghnjbcclm.sHtML

TS:   d.toISOString()
来源：http://www.share.hesvh.cn/Article/details/gytkoqbwr.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.zdbjq.cn/Article/details/ggjpcyglw.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.hesvh.cn/Article/details/grbagnnnc.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.zdbjq.cn/Article/details/gwpmywubx.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.zdbjq.cn/Article/details/gcmvlevpp.sHtML

[J03] 字符串解析为日期
来源：http://mobile.hesvh.cn/Article/details/gfupbrfwo.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.hesvh.cn/Article/details/gsulvjhuy.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.fehbvm.com/Article/details/gkeylyjki.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gaifobphd.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gxgodygsb.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gtukdyrlq.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.hesvh.cn/Article/details/gqybvmqfr.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gwwjvqmqt.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.hesvh.cn/Article/details/gccxmwqcp.sHtML

[J04] 时间戳与日期互转
来源：http://3g.fehbvm.com/Article/details/gpttwxcom.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.zdbjq.cn/Article/details/gqsikluvs.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.hesvh.cn/Article/details/ghqkqtjyf.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.fehbvm.com/Article/details/gvyzvcokl.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.hesvh.cn/Article/details/gqdfyugxf.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.fehbvm.com/Article/details/ghqajhcph.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.zdbjq.cn/Article/details/gmrbqanwc.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.zdbjq.cn/Article/details/gxszkgsfi.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.zdbjq.cn/Article/details/gromewimg.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.zdbjq.cn/Article/details/goqrkwoiz.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.zdbjq.cn/Article/details/gjfxvtzfs.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.hesvh.cn/Article/details/gvzebvsqc.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fehbvm.com/Article/details/gxjqsyueo.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.hesvh.cn/Article/details/gxooeaszt.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.fehbvm.com/Article/details/gqpiazpgh.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.fehbvm.com/Article/details/grnhumexe.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.hesvh.cn/Article/details/gtrakbufi.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.hesvh.cn/Article/details/gufxtuscp.sHtML

[J06] 计算两时间之差
来源：http://baike.hesvh.cn/Article/details/gyfxborxy.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.hesvh.cn/Article/details/gnruifuxa.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.hesvh.cn/Article/details/ghhfipxqg.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.hesvh.cn/Article/details/goxprjpfp.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.fehbvm.com/Article/details/gjwnulwpq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.zdbjq.cn/Article/details/gjaxuoyjb.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.fehbvm.com/Article/details/gkembfnyo.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.fehbvm.com/Article/details/gpztbzqqo.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.zdbjq.cn/Article/details/gttpqmgdx.sHtML

[J07] 比较两个日期
来源：http://www.share.zdbjq.cn/Article/details/gzvtazird.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/ghvmhzlel.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.fehbvm.com/Article/details/gusksfyfw.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.fehbvm.com/Article/details/gqwyzkxih.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.zdbjq.cn/Article/details/gjvgqfttc.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.zdbjq.cn/Article/details/gihjhifgd.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.fehbvm.com/Article/details/gstdrblcl.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.zdbjq.cn/Article/details/guqyaussa.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.hesvh.cn/Article/details/gcnxmanzm.sHtML

[J08] 提取年月日与星期
来源：http://wap.fehbvm.com/Article/details/gsnkdlznz.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.fehbvm.com/Article/details/gdwixrdgr.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.fehbvm.com/Article/details/gizewpilc.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.hesvh.cn/Article/details/gtbafuxqi.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.fehbvm.com/Article/details/gtluydhbm.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.zdbjq.cn/Article/details/gmqpwewss.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.zdbjq.cn/Article/details/gwnouafrk.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.fehbvm.com/Article/details/gvbtujsfb.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.zdbjq.cn/Article/details/gswwozhrx.sHtML

[J09] 时区处理
来源：http://blog.zdbjq.cn/Article/details/gkafsdanb.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.hesvh.cn/Article/details/ghecxkbwc.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.fehbvm.com/Article/details/gxdipfgvh.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fehbvm.com/Article/details/gnazgdjgx.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.zdbjq.cn/Article/details/gilbjtdau.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.hesvh.cn/Article/details/gfsdxzptd.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.zdbjq.cn/Article/details/gaxfywcdz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.fehbvm.com/Article/details/gnuwftqtg.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.fehbvm.com/Article/details/gwhffzqqg.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.hesvh.cn/Article/details/guyhucued.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.hesvh.cn/Article/details/guhjfkgct.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.zdbjq.cn/Article/details/gkibtshko.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.fehbvm.com/Article/details/glkuuwfax.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.hesvh.cn/Article/details/geqbudknn.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.fehbvm.com/Article/details/gzagfalzx.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.hesvh.cn/Article/details/gjwjgggrl.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.fehbvm.com/Article/details/gkdzhvums.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.fehbvm.com/Article/details/gbbsyupit.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqiugwram.sHtML

K. JSON 与序列化
来源：http://3g.hesvh.cn/Article/details/gkysdzhro.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/goqqsopfc.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.fehbvm.com/Article/details/gzcghhqsv.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.hesvh.cn/Article/details/gbgsdtvxt.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.zdbjq.cn/Article/details/gjxgowvcq.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.fehbvm.com/Article/details/gzmnphqgn.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.hesvh.cn/Article/details/gpbvarlzp.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.hesvh.cn/Article/details/glmaoavjk.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.fehbvm.com/Article/details/ghriprapk.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.zdbjq.cn/Article/details/gpcxhxnhr.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.fehbvm.com/Article/details/gfjxewvrt.sHtML

[K02] JSON 字符串转对象
来源：http://3g.zdbjq.cn/Article/details/gpozklbic.sHtML

Py:   json.loads(s)
来源：http://blog.fehbvm.com/Article/details/gatperwwb.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.fehbvm.com/Article/details/gpawzvycn.sHtML

JS:   JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/gqdppyfwg.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gqlnaqspi.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.fehbvm.com/Article/details/gladzwtzp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.hesvh.cn/Article/details/gnhginhux.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/gtmdtnjew.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.fehbvm.com/Article/details/gpriidiwe.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.zdbjq.cn/Article/details/gusvucily.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/grwlnihyc.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.fehbvm.com/Article/details/gnnqoutrj.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/gehrrapsq.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gmjzqwsvv.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gdqybbpno.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.fehbvm.com/Article/details/glmmyrhfe.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fehbvm.com/Article/details/geliwfxdx.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.fehbvm.com/Article/details/gnwnllnbr.sHtML

[K04] 读取 JSON 文件
来源：http://wap.zdbjq.cn/Article/details/gxyaibxji.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.hesvh.cn/Article/details/gbwdyhzkz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.zdbjq.cn/Article/details/glmepypeh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.zdbjq.cn/Article/details/gycrncojj.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fehbvm.com/Article/details/gcjhlbgue.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gmmlfnfka.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.fehbvm.com/Article/details/gmdowckms.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.fehbvm.com/Article/details/gpipxbcdc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gyiursrfv.sHtML

[K05] 深拷贝对象
来源：http://3g.fehbvm.com/Article/details/gdalraxsy.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.fehbvm.com/Article/details/gicokmagc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.zdbjq.cn/Article/details/grqjyypes.sHtML

JS:   structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/giteduqjw.sHtML

TS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gmtafggic.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.hesvh.cn/Article/details/gxmfvvlnn.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.zdbjq.cn/Article/details/gnjyhnujf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.fehbvm.com/Article/details/gjucernmo.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.fehbvm.com/Article/details/gzfhvtfee.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.fehbvm.com/Article/details/gdkgjpsam.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gvsphtqmm.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.fehbvm.com/Article/details/gwbjsfdqk.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fehbvm.com/Article/details/gnwgyuaxy.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gszbsytck.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.zdbjq.cn/Article/details/gjbnpdtvb.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gthwsihgr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gbhwmzrwd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gtmddlikn.sHtML

[K07] 进制转换
来源：http://m.share.zdbjq.cn/Article/details/ghxzpihfm.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gwvsqlfim.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.zdbjq.cn/Article/details/gqcztsgqa.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gpptbigrp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gkvdkhkcu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gephffmse.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.hesvh.cn/Article/details/gaiqgwyzr.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gkmoggqgq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gnlyfjkop.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.hesvh.cn/Article/details/gluoyjcfg.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.hesvh.cn/Article/details/gvcauyiqe.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.zdbjq.cn/Article/details/gjlwebein.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.fehbvm.com/Article/details/gkoaqvdyb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/gqbclexxi.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.fehbvm.com/Article/details/gqreqqcqs.sHtML

Go:   encoding/gob
来源：http://m.share.zdbjq.cn/Article/details/gpligxddv.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.hesvh.cn/Article/details/gmxdwipgz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/ggjyxxjut.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqevfmksd.sHtML

L. 网络请求
来源：http://m.share.fehbvm.com/Article/details/gtkpkhrxn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/guhtxhyvw.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.hesvh.cn/Article/details/gdduenkkb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.zdbjq.cn/Article/details/gxuqxgfcc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.fehbvm.com/Article/details/grinpxklq.sHtML

JS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/glpwgadis.sHtML

TS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/gpkpjbfvv.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.hesvh.cn/Article/details/gxwztkxki.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.fehbvm.com/Article/details/gskbmdryz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.hesvh.cn/Article/details/gqpvfqnel.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.zdbjq.cn/Article/details/ggvcvpkuo.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gveghecwg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gfnfmahyg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.zdbjq.cn/Article/details/gymzdvwcw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/gfcjjvgtc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gmmzicrfa.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.fehbvm.com/Article/details/gpcigdzfi.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fehbvm.com/Article/details/gxldfnvwr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.hesvh.cn/Article/details/geembjniw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fehbvm.com/Article/details/gbmjdiccu.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.hesvh.cn/Article/details/gshxokxmh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fehbvm.com/Article/details/gbtywslil.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.fehbvm.com/Article/details/glbkneqfl.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gdszuuzol.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/grmmwpcbr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fehbvm.com/Article/details/gmabiirxn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gecpcicgj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.hesvh.cn/Article/details/gitoscrif.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gmmyhftkz.sHtML

[L04] 设置超时
来源：http://read.share.fehbvm.com/Article/details/grfqegtrr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.zdbjq.cn/Article/details/gwspetrqc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gvmadnsyg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gyqtjzejw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gcqdvifiu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fehbvm.com/Article/details/gnisldaed.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.hesvh.cn/Article/details/gglqczmen.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.zdbjq.cn/Article/details/gjqkjjwue.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.hesvh.cn/Article/details/gkglizbbc.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.hesvh.cn/Article/details/gkhztqqkt.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/gdjvhoozr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.hesvh.cn/Article/details/gwztyxcye.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gjloleemb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/goucmdrga.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.hesvh.cn/Article/details/gnpwtsaam.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.fehbvm.com/Article/details/georzeiun.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.hesvh.cn/Article/details/gxvdvdhfx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fehbvm.com/Article/details/gxbtpgmzv.sHtML

[L06] 解析响应为 JSON
来源：http://blog.zdbjq.cn/Article/details/gjvleskpc.sHtML

Py:   resp.json()
来源：http://www.share.hesvh.cn/Article/details/gaefrdhoa.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.hesvh.cn/Article/details/gtjmiezqn.sHtML

JS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gexpectgo.sHtML

TS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gyhcqkedl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fehbvm.com/Article/details/glqrgqhin.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.hesvh.cn/Article/details/gwmtaiiux.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.hesvh.cn/Article/details/gdyavsbst.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.zdbjq.cn/Article/details/gtxdczgfb.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gkxpruthd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fehbvm.com/Article/details/gxebxwslr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.hesvh.cn/Article/details/gjymllxcs.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gabbxxgvk.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gcpapfhwp.sHtML

Java: resp.statusCode()
来源：http://m.share.fehbvm.com/Article/details/ggtldmqpt.sHtML

Go:   resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gusvfbexm.sHtML

Ruby: resp.code.to_i
来源：http://m.share.hesvh.cn/Article/details/gkwenwoec.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gnoatxcef.sHtML

[L08] 并发请求多个地址
来源：http://m.share.hesvh.cn/Article/details/guomplqed.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.zdbjq.cn/Article/details/gppmjuyap.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fehbvm.com/Article/details/gcliimnet.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gavmezifm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gkanjvwlg.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.hesvh.cn/Article/details/gthqrbqen.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.zdbjq.cn/Article/details/gmtaszabu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.zdbjq.cn/Article/details/gheqqorqe.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.zdbjq.cn/Article/details/gcjpzniwr.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzwdjsbbo.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/gfyejojap.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gctdkjfly.sHtML

[M01] 读取命令行参数
来源：http://wap.fehbvm.com/Article/details/glekbaxpr.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fehbvm.com/Article/details/gunyaeqee.sHtML

PHP:  $argv;  $argc;
来源：http://blog.hesvh.cn/Article/details/gvrsqykjr.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/glpimursz.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gcqhvexbe.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gnoxqdfsv.sHtML

Go:   os.Args[1:]
来源：http://read.share.fehbvm.com/Article/details/giqjsiaml.sHtML

Ruby: ARGV
来源：http://www.m.share.fehbvm.com/Article/details/gtkianfsc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/genepwjzu.sHtML

[M02] 读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gtbjmmcfo.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gltvcoekf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gdqwuxpcr.sHtML

JS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gnlmtyjbu.sHtML

TS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gqxaagahr.sHtML

Java: System.getenv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/giufedcfl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.hesvh.cn/Article/details/gqjfxexqf.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/gowpjjhpw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gbwjriieg.sHtML

[M03] 执行外部命令
来源：http://www.blog.zdbjq.cn/Article/details/gjrgbrsja.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/gobzxnrur.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.zdbjq.cn/Article/details/gzlqajgqt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/glluhzhjd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gbryaxnqo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.hesvh.cn/Article/details/gvdmsxqti.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/gfvxtgste.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.hesvh.cn/Article/details/gnxmoxcbp.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fehbvm.com/Article/details/gpvjcbfgv.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gszjiysyh.sHtML

Py:   os.getcwd()
来源：http://blog.hesvh.cn/Article/details/ggrzeefou.sHtML

PHP:  getcwd();
来源：http://baike.hesvh.cn/Article/details/gymmfhcru.sHtML

JS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gkyjnztcg.sHtML

TS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gveyhqmbr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/gjqlvfmqg.sHtML

Go:   os.Getwd()
来源：http://www.blog.hesvh.cn/Article/details/glmhzfqjf.sHtML

Ruby: Dir.pwd
来源：http://baike.zdbjq.cn/Article/details/gtqikmpxr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.hesvh.cn/Article/details/gtcwepzxg.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/grwdjluen.sHtML

Py:   sys.exit(1)
来源：http://3g.fehbvm.com/Article/details/ggpptxagv.sHtML

PHP:  exit(1);
来源：http://read.share.zdbjq.cn/Article/details/gfzbtexmo.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gdcodjgbl.sHtML

TS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gyfbxvhwu.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gbxltgbhi.sHtML

Go:   os.Exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gflmoyiuc.sHtML

Ruby: exit 1
来源：http://www.share.fehbvm.com/Article/details/gtjmgiwbb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/gqbnfhhgd.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/ghikjuhth.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gmgrtbabz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/gzwomxvef.sHtML

JS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gghgopifl.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gvkjjxcbu.sHtML

Java: System.err.println("err")
来源：http://blog.zdbjq.cn/Article/details/gggovmyvm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.zdbjq.cn/Article/details/gacsechen.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/gwbymbpqa.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.zdbjq.cn/Article/details/ggakrtvxc.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.zdbjq.cn/Article/details/gdhkrhfzu.sHtML


<!-- 参考信息 -->