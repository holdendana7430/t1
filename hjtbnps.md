代发 wailian999

J. 日期与时间
来源：http://blog.fehbvm.com/Article/details/gnpodezao.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzmrxrgkv.sHtML

[J01] 获取当前时间
来源：http://m.share.fehbvm.com/Article/details/gsoqcbuqf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.hesvh.cn/Article/details/gevudtoke.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.fehbvm.com/Article/details/giutgfnql.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.zdbjq.cn/Article/details/gdugkbrlb.sHtML

TS:   new Date();  Date.now()
来源：http://baike.hesvh.cn/Article/details/gxezsmsjn.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.fehbvm.com/Article/details/gcopvmwxz.sHtML

Go:   time.Now()
来源：http://baike.zdbjq.cn/Article/details/gltoecsjn.sHtML

Ruby: Time.now
来源：http://read.share.hesvh.cn/Article/details/gkkhjkbsh.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.zdbjq.cn/Article/details/gkbkxrhea.sHtML

[J02] 格式化输出
来源：http://m.share.zdbjq.cn/Article/details/gsvshvwxk.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fehbvm.com/Article/details/gqlgouspo.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.hesvh.cn/Article/details/gxrjdehpg.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.hesvh.cn/Article/details/gahnckzbw.sHtML

TS:   d.toISOString()
来源：http://mobile.zdbjq.cn/Article/details/gwnloasdi.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.zdbjq.cn/Article/details/gfglowgyw.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.zdbjq.cn/Article/details/gdnyqizfx.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.zdbjq.cn/Article/details/gfbiwiekb.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.hesvh.cn/Article/details/gfwuctlhi.sHtML

[J03] 字符串解析为日期
来源：http://read.share.zdbjq.cn/Article/details/gqlsfjhog.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.hesvh.cn/Article/details/gjegeiezj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.hesvh.cn/Article/details/gvpepmrsa.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gztxsdwoq.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gcsifvoak.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/geiyiavhi.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.fehbvm.com/Article/details/ghbgzarfa.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gzmgcmshz.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.fehbvm.com/Article/details/gtpfdrvfx.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.fehbvm.com/Article/details/gknwfxeyb.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.zdbjq.cn/Article/details/gfcqwhntk.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.hesvh.cn/Article/details/gsdlnuowb.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.fehbvm.com/Article/details/gsbsgqcdl.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.zdbjq.cn/Article/details/gmacspghy.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.fehbvm.com/Article/details/gtmyrdhgk.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.hesvh.cn/Article/details/gshuldayx.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.fehbvm.com/Article/details/gsjmgevxr.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.zdbjq.cn/Article/details/gzexptxmw.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.hesvh.cn/Article/details/gxgtlvsmc.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.fehbvm.com/Article/details/ggxunhqnw.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.fehbvm.com/Article/details/ggqewvlvc.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.hesvh.cn/Article/details/gcwitrioc.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.hesvh.cn/Article/details/giktwkymn.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.fehbvm.com/Article/details/gmvzqnfsy.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.hesvh.cn/Article/details/gzkqzafpz.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.hesvh.cn/Article/details/ggrttpihk.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.hesvh.cn/Article/details/gkulyuwvz.sHtML

[J06] 计算两时间之差
来源：http://baike.fehbvm.com/Article/details/gzxamgsgh.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.hesvh.cn/Article/details/gfnvbyzql.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.fehbvm.com/Article/details/ggzbhwdnw.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.zdbjq.cn/Article/details/giposbpxf.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.zdbjq.cn/Article/details/gfnwqlpix.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.hesvh.cn/Article/details/gbikqqiiz.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.hesvh.cn/Article/details/gyvpmgxgc.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.fehbvm.com/Article/details/gtbhuqnwd.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.fehbvm.com/Article/details/gdygredrz.sHtML

[J07] 比较两个日期
来源：http://3g.hesvh.cn/Article/details/gbkplefci.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.zdbjq.cn/Article/details/ggppqhyyl.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.zdbjq.cn/Article/details/gkxjmfzsg.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.zdbjq.cn/Article/details/gqbsmrxad.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.hesvh.cn/Article/details/gwnvwsyzm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.zdbjq.cn/Article/details/gwsxdfiwz.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.hesvh.cn/Article/details/gqqfcjlfa.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.hesvh.cn/Article/details/gdnwjfuyt.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.hesvh.cn/Article/details/gisscpvxn.sHtML

[J08] 提取年月日与星期
来源：http://www.share.fehbvm.com/Article/details/gxrfymbnf.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.fehbvm.com/Article/details/gjvqthurd.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.hesvh.cn/Article/details/gmepywvlx.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.fehbvm.com/Article/details/gplfzwtob.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.zdbjq.cn/Article/details/ggltzzmnx.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.hesvh.cn/Article/details/gcqrdprdj.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.hesvh.cn/Article/details/gpxzannpq.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.fehbvm.com/Article/details/gfpsyeltr.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.zdbjq.cn/Article/details/gwavxzguf.sHtML

[J09] 时区处理
来源：http://wap.zdbjq.cn/Article/details/gtvjpbcuy.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.hesvh.cn/Article/details/goovrhuvz.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.fehbvm.com/Article/details/gcqrcjsih.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.zdbjq.cn/Article/details/gofhskctf.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.hesvh.cn/Article/details/gifpqwgrl.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.zdbjq.cn/Article/details/guizmpdpl.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.hesvh.cn/Article/details/gtstythzz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.fehbvm.com/Article/details/gqqzmorev.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.fehbvm.com/Article/details/gzomnzxhu.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.zdbjq.cn/Article/details/gqerdttgu.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.zdbjq.cn/Article/details/guyvyomkh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.hesvh.cn/Article/details/gknzpxpzs.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.zdbjq.cn/Article/details/gaqwjbgzv.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.fehbvm.com/Article/details/ghhdcwcvb.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.hesvh.cn/Article/details/gjrhoakyj.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.hesvh.cn/Article/details/graauqwtf.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.fehbvm.com/Article/details/gvaralydx.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.zdbjq.cn/Article/details/gpvctnjqx.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gocncgcfw.sHtML

K. JSON 与序列化
来源：http://wap.hesvh.cn/Article/details/gzbkiczyv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gcogzfejj.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.hesvh.cn/Article/details/gydrceymn.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.hesvh.cn/Article/details/gcainfqyt.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.zdbjq.cn/Article/details/gobphgtbu.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.fehbvm.com/Article/details/gsvstqjsz.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.hesvh.cn/Article/details/gwymesjwm.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.fehbvm.com/Article/details/gxfqcfthp.sHtML

Go:   json.Marshal(obj)
来源：http://wap.fehbvm.com/Article/details/gskfyqden.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.zdbjq.cn/Article/details/gukpmireh.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.hesvh.cn/Article/details/goccqwsuz.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.fehbvm.com/Article/details/gazomhpww.sHtML

Py:   json.loads(s)
来源：http://mobile.zdbjq.cn/Article/details/glgiaxiwk.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.zdbjq.cn/Article/details/gtnayspvd.sHtML

JS:   JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/gqctsaplo.sHtML

TS:   JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/gomalepsu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.fehbvm.com/Article/details/gdtphlvlc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.fehbvm.com/Article/details/gvcpwuwla.sHtML

Ruby: JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/ghchfdwkf.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.fehbvm.com/Article/details/gxnliituq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.fehbvm.com/Article/details/gyrjxeybx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/gpbpjrlve.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.zdbjq.cn/Article/details/gacvgduxx.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.hesvh.cn/Article/details/gjocmpksx.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/geypeexlm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.zdbjq.cn/Article/details/glfvgrgle.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.zdbjq.cn/Article/details/ggejoheya.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.zdbjq.cn/Article/details/gcqdsakrt.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.hesvh.cn/Article/details/gmhwwqbge.sHtML

[K04] 读取 JSON 文件
来源：http://baike.hesvh.cn/Article/details/gbdneojdy.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.hesvh.cn/Article/details/gtrkveepb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.zdbjq.cn/Article/details/gvhzygmkp.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.zdbjq.cn/Article/details/gfturlzsg.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/gdboykwii.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.hesvh.cn/Article/details/ggkzgbynq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/gxskivbzl.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.fehbvm.com/Article/details/guwpnidgo.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/gdoyjtvhw.sHtML

[K05] 深拷贝对象
来源：http://baike.zdbjq.cn/Article/details/gpdbebwzl.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.hesvh.cn/Article/details/gajagjttq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.zdbjq.cn/Article/details/gbrpmmafs.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gqlgbpxym.sHtML

TS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gbgbhpwhv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.hesvh.cn/Article/details/gonargtzn.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.zdbjq.cn/Article/details/gvohttzid.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.fehbvm.com/Article/details/gpoubbhaf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.fehbvm.com/Article/details/gjyaxnfmm.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.zdbjq.cn/Article/details/gxhngqbpt.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.hesvh.cn/Article/details/gxjgublav.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.hesvh.cn/Article/details/gwrvxgwko.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/gskqvflkw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/gtahgdfsd.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.zdbjq.cn/Article/details/guqkbhcmj.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gqiwtcfvo.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gxperbjwx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gptilglix.sHtML

[K07] 进制转换
来源：http://3g.zdbjq.cn/Article/details/gccykinsd.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gpmmwwqeg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.fehbvm.com/Article/details/gwkjbibqq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gizgvxvaa.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gynlliudi.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gfnmqdtcm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.zdbjq.cn/Article/details/gkvgqenxv.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.zdbjq.cn/Article/details/gvleqblsm.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gkcnoyxgr.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.hesvh.cn/Article/details/gjsourgem.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.fehbvm.com/Article/details/gqkzviaev.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.hesvh.cn/Article/details/gadleclls.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/gyfyjrraa.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/gznjktism.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.zdbjq.cn/Article/details/guhhifexg.sHtML

Go:   encoding/gob
来源：http://www.blog.zdbjq.cn/Article/details/gmzzmdhoq.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.zdbjq.cn/Article/details/gokdxboxt.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gylqkvvgm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghkeiohxi.sHtML

L. 网络请求
来源：http://m.share.zdbjq.cn/Article/details/gilbcljlw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gncslanjv.sHtML

[L01] 发送 GET 请求
来源：http://3g.hesvh.cn/Article/details/gcwgrradf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.zdbjq.cn/Article/details/giovynlge.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fehbvm.com/Article/details/gyufojhnx.sHtML

JS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/guxhvklyw.sHtML

TS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/gbqacxriv.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.zdbjq.cn/Article/details/gqgszftgd.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.hesvh.cn/Article/details/glnqycyrn.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.hesvh.cn/Article/details/gbsfdeumh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.hesvh.cn/Article/details/gwcilmzsu.sHtML

[L02] 发送 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gwmhcxowj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.hesvh.cn/Article/details/gbctzgnsi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.zdbjq.cn/Article/details/gexoztwxw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gxfgjzied.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gxexzrjxy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.zdbjq.cn/Article/details/gwazuxsps.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.hesvh.cn/Article/details/gkjoytsil.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.zdbjq.cn/Article/details/ghnmfmaam.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.hesvh.cn/Article/details/gqqiincpp.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.hesvh.cn/Article/details/gigdkoggh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.hesvh.cn/Article/details/gqoibcqdh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fehbvm.com/Article/details/gdzurovvg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gkkbdvhct.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/gfuuevmje.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.fehbvm.com/Article/details/gpvrlnrzl.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gwpuqsjnu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.hesvh.cn/Article/details/gpktzibvy.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/galxywbyg.sHtML

[L04] 设置超时
来源：http://blog.zdbjq.cn/Article/details/gvmvfsvty.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.hesvh.cn/Article/details/gbundhfxs.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.hesvh.cn/Article/details/gadazsixr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/gldfnbwpk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gemprcryb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gttgjehds.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fehbvm.com/Article/details/gcsdhcdtu.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fehbvm.com/Article/details/gbpqefscu.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.hesvh.cn/Article/details/gpmyawpwx.sHtML

[L05] 上传文件（multipart）
来源：http://3g.fehbvm.com/Article/details/grzsmmcja.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fehbvm.com/Article/details/gdhonbfpq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.hesvh.cn/Article/details/gkfkuhjol.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/godcdltgo.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gixuexmvc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.zdbjq.cn/Article/details/gaqrvcofa.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.hesvh.cn/Article/details/ggylwelmc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.hesvh.cn/Article/details/gilqmbwxr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.hesvh.cn/Article/details/gbbeqewiy.sHtML

[L06] 解析响应为 JSON
来源：http://3g.hesvh.cn/Article/details/guftmdbwp.sHtML

Py:   resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gpblhbxin.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fehbvm.com/Article/details/gdnuyquxv.sHtML

JS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gmrsqwxxy.sHtML

TS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gpvoaxded.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fehbvm.com/Article/details/gdlgnkzkb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.zdbjq.cn/Article/details/gpcnhrjoh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.hesvh.cn/Article/details/ghqfthudn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.zdbjq.cn/Article/details/gqpwshflp.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gxmhsfbjk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.zdbjq.cn/Article/details/guaejgxin.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fehbvm.com/Article/details/gkvsfzurq.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gjczttpjx.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/goqtacvnl.sHtML

Java: resp.statusCode()
来源：http://read.share.fehbvm.com/Article/details/gfnacdoua.sHtML

Go:   resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gtpzgomdn.sHtML

Ruby: resp.code.to_i
来源：http://www.share.hesvh.cn/Article/details/glhekchto.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gbplzgumg.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fehbvm.com/Article/details/gjzxksbop.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.zdbjq.cn/Article/details/glpqtxszj.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.zdbjq.cn/Article/details/gdpmsllzn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gtdntdizm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gbhqyyivc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.hesvh.cn/Article/details/grkwosiht.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fehbvm.com/Article/details/grdvbqxpm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fehbvm.com/Article/details/glhgcnybb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fehbvm.com/Article/details/gwbepjqot.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gewugbehy.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.hesvh.cn/Article/details/gypmfgeqa.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ganwuyypx.sHtML

[M01] 读取命令行参数
来源：http://m.share.fehbvm.com/Article/details/gjhonrkzs.sHtML

Py:   sys.argv[1:]
来源：http://blog.hesvh.cn/Article/details/grtpnmgir.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/gweylzhdx.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/grmpugitp.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gbzzneqkw.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fehbvm.com/Article/details/gizdbxurv.sHtML

Go:   os.Args[1:]
来源：http://mobile.zdbjq.cn/Article/details/gjigitfig.sHtML

Ruby: ARGV
来源：http://wap.zdbjq.cn/Article/details/guukttycq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gzgafrxzv.sHtML

[M02] 读取环境变量
来源：http://blog.hesvh.cn/Article/details/gxxcrmopj.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.hesvh.cn/Article/details/gtnkvzvxb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gidxxtlwa.sHtML

JS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gafuzdpnq.sHtML

TS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gnwjqmtnw.sHtML

Java: System.getenv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gebmurkzp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gbfuzcdwm.sHtML

Ruby: ENV["HOME"]
来源：http://baike.hesvh.cn/Article/details/gjpkgwfvu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.hesvh.cn/Article/details/guifqavec.sHtML

[M03] 执行外部命令
来源：http://mobile.hesvh.cn/Article/details/gumyqmuuv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.zdbjq.cn/Article/details/gxsbktusn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fehbvm.com/Article/details/goynhvorf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/graeecpyk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gdwecnoou.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/gmepyowkt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/grnhoesxg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fehbvm.com/Article/details/gtgccarsk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/gxtsnqyqo.sHtML

[M04] 获取当前工作目录
来源：http://www.share.hesvh.cn/Article/details/gjqhmopfu.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/gbyjssrqk.sHtML

PHP:  getcwd();
来源：http://www.blog.hesvh.cn/Article/details/gfilahzou.sHtML

JS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/ggvbrulef.sHtML

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gxebvejft.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.hesvh.cn/Article/details/guppddqog.sHtML

Go:   os.Getwd()
来源：http://www.share.fehbvm.com/Article/details/gtcsgwkzh.sHtML

Ruby: Dir.pwd
来源：http://wap.fehbvm.com/Article/details/gepuqynss.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.hesvh.cn/Article/details/gdxxleywn.sHtML

[M05] 设置退出码
来源：http://read.share.fehbvm.com/Article/details/glhvlhbtn.sHtML

Py:   sys.exit(1)
来源：http://blog.hesvh.cn/Article/details/gvwhalgzr.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/gfcpzslkm.sHtML

JS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gskjvvqay.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gmuwxsepi.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gpcdsutge.sHtML

Go:   os.Exit(1)
来源：http://3g.hesvh.cn/Article/details/gxsqfsqqe.sHtML

Ruby: exit 1
来源：http://www.share.fehbvm.com/Article/details/gjtjaznql.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/ggtzthxoq.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/gtrbmgpsj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gtpagijta.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/gwdxzqkio.sHtML

JS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gfxhdxmdl.sHtML

TS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gkbksdwsf.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/gofkmqegu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.zdbjq.cn/Article/details/gnevsosjm.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/gcjoyliem.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gaqvdyaue.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/gusnicvjw.sHtML


<!-- 参考信息 -->