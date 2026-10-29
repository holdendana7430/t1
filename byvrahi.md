代发 wailian999

J. 日期与时间
来源：http://blog.zdbjq.cn/Article/details/gwevhmbil.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnoilrjkx.sHtML

[J01] 获取当前时间
来源：http://read.share.hesvh.cn/Article/details/gyjfpmbko.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.fehbvm.com/Article/details/gcxjglucx.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.hesvh.cn/Article/details/gnhilqtiw.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.hesvh.cn/Article/details/gkixslqqz.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.hesvh.cn/Article/details/gilkepwwu.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.hesvh.cn/Article/details/guzpmlbls.sHtML

Go:   time.Now()
来源：http://www.m.share.hesvh.cn/Article/details/gegswwsfk.sHtML

Ruby: Time.now
来源：http://wap.fehbvm.com/Article/details/ghdvwnghv.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.fehbvm.com/Article/details/gncklwvwt.sHtML

[J02] 格式化输出
来源：http://3g.zdbjq.cn/Article/details/gmijcefqs.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.zdbjq.cn/Article/details/gcbcvgcea.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.hesvh.cn/Article/details/gfntgoffd.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.zdbjq.cn/Article/details/grtzvtegm.sHtML

TS:   d.toISOString()
来源：http://wap.hesvh.cn/Article/details/gviqnwtvv.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.fehbvm.com/Article/details/gcvickyjn.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.zdbjq.cn/Article/details/gjypgrlpu.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fehbvm.com/Article/details/gdfazhnro.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.zdbjq.cn/Article/details/gbiowhhfb.sHtML

[J03] 字符串解析为日期
来源：http://3g.hesvh.cn/Article/details/gubqwoiam.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.zdbjq.cn/Article/details/giqiksszl.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.fehbvm.com/Article/details/gxbpsorca.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gfnmtnycv.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gpyldcrlq.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gwhjrqtab.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gefoaaftg.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gguhpaxcm.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.hesvh.cn/Article/details/gfpulxsai.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.zdbjq.cn/Article/details/giborbbaf.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.zdbjq.cn/Article/details/gitxrbhlc.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.fehbvm.com/Article/details/gcrssfufh.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.fehbvm.com/Article/details/gxpjrkflm.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.fehbvm.com/Article/details/gfyjxsdag.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.hesvh.cn/Article/details/gjzzjhtjc.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gnfcehved.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.zdbjq.cn/Article/details/gtrrzwjoz.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.zdbjq.cn/Article/details/gxilbtkup.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.fehbvm.com/Article/details/gkwktqaoh.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.hesvh.cn/Article/details/gtcncftqr.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.hesvh.cn/Article/details/gstitjfha.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.zdbjq.cn/Article/details/gxiueihfa.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.hesvh.cn/Article/details/gpolpjadu.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.fehbvm.com/Article/details/glorjskhz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.hesvh.cn/Article/details/gphxcfvnw.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.fehbvm.com/Article/details/gzsfvyvrr.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.fehbvm.com/Article/details/ggvljvsaa.sHtML

[J06] 计算两时间之差
来源：http://baike.zdbjq.cn/Article/details/gcapmjwvr.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.fehbvm.com/Article/details/guwjiilev.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.zdbjq.cn/Article/details/gvfxoljxa.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.hesvh.cn/Article/details/gotquocjn.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.zdbjq.cn/Article/details/gtnvltzxw.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.hesvh.cn/Article/details/ghtqafclr.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.zdbjq.cn/Article/details/gbxqxuqoe.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.hesvh.cn/Article/details/gnrdjvmaj.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.hesvh.cn/Article/details/gkigdndxa.sHtML

[J07] 比较两个日期
来源：http://blog.hesvh.cn/Article/details/gcoirvsct.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.hesvh.cn/Article/details/ggdirrgce.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.fehbvm.com/Article/details/gwthyvuxs.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.hesvh.cn/Article/details/gjqcfiwxk.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.hesvh.cn/Article/details/glpgaddkp.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.hesvh.cn/Article/details/gksqeogid.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.zdbjq.cn/Article/details/gixavwbyi.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.zdbjq.cn/Article/details/gimfnvkix.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.zdbjq.cn/Article/details/gccymqone.sHtML

[J08] 提取年月日与星期
来源：http://baike.zdbjq.cn/Article/details/grczrtykq.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.hesvh.cn/Article/details/glfamwdzn.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.fehbvm.com/Article/details/gjxcuxgvk.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.hesvh.cn/Article/details/gcoutoqpj.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.hesvh.cn/Article/details/gldigfazt.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.zdbjq.cn/Article/details/ggguzfvjn.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.zdbjq.cn/Article/details/gbhzbvfbm.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.fehbvm.com/Article/details/giqcpsaml.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.hesvh.cn/Article/details/guqtkwlca.sHtML

[J09] 时区处理
来源：http://blog.hesvh.cn/Article/details/gegdyaeou.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.hesvh.cn/Article/details/gpujfjdto.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.fehbvm.com/Article/details/gkkeyrpmx.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.hesvh.cn/Article/details/gtdimmwnt.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.zdbjq.cn/Article/details/gejjgcftw.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.zdbjq.cn/Article/details/gqqnvsvkg.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.fehbvm.com/Article/details/gtsizzmrb.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.fehbvm.com/Article/details/gsfcoizdb.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.fehbvm.com/Article/details/gzmeostjf.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.zdbjq.cn/Article/details/gjrwvxbxh.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.fehbvm.com/Article/details/gdrtowxde.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.zdbjq.cn/Article/details/gjtwwfrop.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.hesvh.cn/Article/details/gsrrlwjxi.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.fehbvm.com/Article/details/gtkwsuwny.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.zdbjq.cn/Article/details/gbmmpwevm.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.fehbvm.com/Article/details/ghlglludf.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.hesvh.cn/Article/details/gswwybrpr.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.zdbjq.cn/Article/details/gtczfptky.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gsyodzsgf.sHtML

K. JSON 与序列化
来源：http://www.blog.hesvh.cn/Article/details/gtqdkarvd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmcqpahql.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.fehbvm.com/Article/details/gqjlnxber.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.fehbvm.com/Article/details/ggqdiiwee.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.hesvh.cn/Article/details/gcpmfybnu.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.fehbvm.com/Article/details/gtlmipkxs.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.zdbjq.cn/Article/details/gczrcnzfo.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.fehbvm.com/Article/details/gcqxwndvl.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.fehbvm.com/Article/details/gdpadynhy.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.hesvh.cn/Article/details/gqmmexwcp.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gkmerpfew.sHtML

[K02] JSON 字符串转对象
来源：http://baike.zdbjq.cn/Article/details/gpqfqcfgf.sHtML

Py:   json.loads(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gfbbdxjnr.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.hesvh.cn/Article/details/gtslgyogz.sHtML

JS:   JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/gdpvjieno.sHtML

TS:   JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/gqzaaxofw.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.fehbvm.com/Article/details/gajqqxheq.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.hesvh.cn/Article/details/gavsswqrc.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gwfrvwmdo.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gyixkdqsw.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.fehbvm.com/Article/details/gpzksbhqi.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.hesvh.cn/Article/details/gcfboqvul.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.zdbjq.cn/Article/details/gwyurcspw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.zdbjq.cn/Article/details/gkscgzknv.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gndfgkcdj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.hesvh.cn/Article/details/gopiclfxg.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.fehbvm.com/Article/details/gdykdzlwt.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.hesvh.cn/Article/details/gwpbryugd.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.zdbjq.cn/Article/details/ghjlznvdy.sHtML

[K04] 读取 JSON 文件
来源：http://baike.fehbvm.com/Article/details/gjmxkdnil.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.zdbjq.cn/Article/details/gxufihtti.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.zdbjq.cn/Article/details/gyjkyzedr.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fehbvm.com/Article/details/gyhtnkacc.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.hesvh.cn/Article/details/gmnninhkw.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gbsyyjpxi.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.hesvh.cn/Article/details/gikwwytoy.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.fehbvm.com/Article/details/gdkjqwplu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.zdbjq.cn/Article/details/guzouxrgp.sHtML

[K05] 深拷贝对象
来源：http://m.share.fehbvm.com/Article/details/gogzzvdht.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.hesvh.cn/Article/details/glxtqtypr.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.zdbjq.cn/Article/details/ghpczlimx.sHtML

JS:   structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gbxmqhqbn.sHtML

TS:   structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gxwacsxjc.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.zdbjq.cn/Article/details/goioccqpy.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.hesvh.cn/Article/details/gupeupkci.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fehbvm.com/Article/details/gnnmtykyd.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.fehbvm.com/Article/details/gtqgabldr.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.hesvh.cn/Article/details/gedwxxoiu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gugjbtsgl.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.hesvh.cn/Article/details/gbiotrkrb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gvykopfuh.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.hesvh.cn/Article/details/gqjoaofkj.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.zdbjq.cn/Article/details/gzseasrdi.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gmfbyrwue.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/geagyppsd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gkkfdbrkw.sHtML

[K07] 进制转换
来源：http://3g.hesvh.cn/Article/details/gulwmmuwj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gvfzrqcgo.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fehbvm.com/Article/details/gksuolwkq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gszwhvfqn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/grmdwspom.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gyisrxoxp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.zdbjq.cn/Article/details/gefpijkwd.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.zdbjq.cn/Article/details/geuinjncv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gijfzpebo.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.hesvh.cn/Article/details/gvvdzycqa.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.zdbjq.cn/Article/details/gojukqdrm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.fehbvm.com/Article/details/gmxbokbvs.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/gyiabsyyh.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/gabkhctnr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.hesvh.cn/Article/details/gzhkqntsi.sHtML

Go:   encoding/gob
来源：http://wap.fehbvm.com/Article/details/gwalkqppm.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.hesvh.cn/Article/details/gbrtyhpfx.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gbftxqdzy.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxwxrnnkc.sHtML

L. 网络请求
来源：http://m.share.zdbjq.cn/Article/details/gpalwokoa.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjftnybjp.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.fehbvm.com/Article/details/gazmgnoyl.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.zdbjq.cn/Article/details/giiskpbpq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.zdbjq.cn/Article/details/giudydguq.sHtML

JS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gcpgqqckj.sHtML

TS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/gfjvdbkym.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.zdbjq.cn/Article/details/gkwbgvjnm.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.hesvh.cn/Article/details/gfwsmgwez.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.zdbjq.cn/Article/details/gwlwonqsn.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.hesvh.cn/Article/details/gwleiugir.sHtML

[L02] 发送 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/glytnqpjz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/gsldqupqi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.fehbvm.com/Article/details/gtttvhwkp.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/gdytewxol.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/gfpktlazt.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.fehbvm.com/Article/details/geokcfrcl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.hesvh.cn/Article/details/gyqutkppe.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.zdbjq.cn/Article/details/ggrsroqpq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.fehbvm.com/Article/details/gzgonxjue.sHtML

[L03] 设置自定义请求头
来源：http://www.share.zdbjq.cn/Article/details/gyguijadw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.hesvh.cn/Article/details/gltqmpwav.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.zdbjq.cn/Article/details/goyxwyqra.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/gsnzvxdnu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gwgrcnrvv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.hesvh.cn/Article/details/gmmmhypdp.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gcljertlv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fehbvm.com/Article/details/gtfrtrqmp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gvpyxqjgm.sHtML

[L04] 设置超时
来源：http://wap.fehbvm.com/Article/details/gtjvodnik.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fehbvm.com/Article/details/gqjwitefr.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.zdbjq.cn/Article/details/gkpczrosy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gshtxfqga.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/guxsowybw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.hesvh.cn/Article/details/gzxzddebn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.hesvh.cn/Article/details/gcvphmqed.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.zdbjq.cn/Article/details/goiovfjkr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gmmaugfku.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fehbvm.com/Article/details/goszqgqcb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.fehbvm.com/Article/details/gvhszcwad.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.zdbjq.cn/Article/details/ghkxpityh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gaxjdjypo.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/glnrnrino.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.hesvh.cn/Article/details/gzxtomldo.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fehbvm.com/Article/details/gciavkcyp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fehbvm.com/Article/details/gcywkowty.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gdfcdxrdc.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.fehbvm.com/Article/details/gpuuihytq.sHtML

Py:   resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gcaftuylr.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gzvjybjen.sHtML

JS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gvwnfsxum.sHtML

TS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gijemqxrk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gwykculsh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.zdbjq.cn/Article/details/ggrciknax.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.zdbjq.cn/Article/details/gfrrrnjso.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fehbvm.com/Article/details/gqppxpogi.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gubqjlgsk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.hesvh.cn/Article/details/gsfrzgrzb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gwnialhln.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gjqctttnc.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gcadyfqls.sHtML

Java: resp.statusCode()
来源：http://m.share.hesvh.cn/Article/details/giefzwmmz.sHtML

Go:   resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gaokpmsva.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.fehbvm.com/Article/details/gbuixptrk.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gdzcjhxwa.sHtML

[L08] 并发请求多个地址
来源：http://read.share.zdbjq.cn/Article/details/gidposicv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.zdbjq.cn/Article/details/gtavbivwj.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.zdbjq.cn/Article/details/gboogpfpg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gryexaxna.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gvyqxbhqm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fehbvm.com/Article/details/gdojzvqyi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.hesvh.cn/Article/details/gtccjgzne.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.hesvh.cn/Article/details/gemyjouux.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.fehbvm.com/Article/details/gkbjbnyhd.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtzhityzf.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.zdbjq.cn/Article/details/gakxxaxvs.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbcaglgpf.sHtML

[M01] 读取命令行参数
来源：http://www.share.fehbvm.com/Article/details/gemjeufnn.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.fehbvm.com/Article/details/gqfwswysw.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fehbvm.com/Article/details/gmmjnrwbs.sHtML

JS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gjinkhote.sHtML

TS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/grmheylci.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/geusbkfap.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fehbvm.com/Article/details/gtspoqdjv.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/ghqoyqgiu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/geufwgcpg.sHtML

[M02] 读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/golfwoozh.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.hesvh.cn/Article/details/giaivakhu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gcthleuii.sHtML

JS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gtxdvjgyc.sHtML

TS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/guwffxnim.sHtML

Java: System.getenv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gitzivtlg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gqjbfwodf.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.hesvh.cn/Article/details/gvetnpkyf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/gomimmhig.sHtML

[M03] 执行外部命令
来源：http://blog.hesvh.cn/Article/details/gqcoohkca.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/gdncempaq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fehbvm.com/Article/details/gcdnwvyjx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gxshltifd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/ggpgykpdp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.hesvh.cn/Article/details/gjzwlldxh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.hesvh.cn/Article/details/gkctrtvdn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/gsxliferb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.zdbjq.cn/Article/details/gfddavawa.sHtML

[M04] 获取当前工作目录
来源：http://mobile.hesvh.cn/Article/details/gmrcjqhmx.sHtML

Py:   os.getcwd()
来源：http://blog.fehbvm.com/Article/details/gnnrhtfdm.sHtML

PHP:  getcwd();
来源：http://3g.zdbjq.cn/Article/details/gcrrihuhg.sHtML

JS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gyrpzmkpw.sHtML

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/getaccxjp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/gjbthxgsr.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/gbnmeziog.sHtML

Ruby: Dir.pwd
来源：http://www.share.zdbjq.cn/Article/details/gwwvrymwc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.zdbjq.cn/Article/details/gnrauelmx.sHtML

[M05] 设置退出码
来源：http://3g.zdbjq.cn/Article/details/gzqecyzwb.sHtML

Py:   sys.exit(1)
来源：http://blog.hesvh.cn/Article/details/gnbslnjjb.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/gjxgzteum.sHtML

JS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gpsxucnuy.sHtML

TS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gltbcrvef.sHtML

Java: System.exit(1)
来源：http://baike.hesvh.cn/Article/details/gxysktygc.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gossdnpqb.sHtML

Ruby: exit 1
来源：http://www.share.fehbvm.com/Article/details/gurlmglec.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.zdbjq.cn/Article/details/geyqukypm.sHtML

[M06] 向标准错误输出
来源：http://www.share.zdbjq.cn/Article/details/gnfqyzugu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/glqeddxzr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.hesvh.cn/Article/details/ghrzuitxj.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/ghsnppskv.sHtML

TS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gvdbycerx.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/gljrpleub.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/gbxakxarv.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/gwvqocyhu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fehbvm.com/Article/details/gtxebrbsj.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/gyrpcszdp.sHtML


<!-- 参考信息 -->