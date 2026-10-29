代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.hesvh.cn/Article/details/gyvomwllz.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.hesvh.cn/Article/details/gsjsvspnh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fehbvm.com/Article/details/gxcjtpikn.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.hesvh.cn/Article/details/gjohcogdf.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.zdbjq.cn/Article/details/ggccwuxqd.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.zdbjq.cn/Article/details/gszgqtojv.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.hesvh.cn/Article/details/gbwvjnpbn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxqmabmzd.sHtML

J. 日期与时间
来源：http://baike.zdbjq.cn/Article/details/gilysunkx.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnxaerkjd.sHtML

[J01] 获取当前时间
来源：http://blog.fehbvm.com/Article/details/geteygkzm.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.zdbjq.cn/Article/details/gxireffsj.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.hesvh.cn/Article/details/gvdatxxmr.sHtML

JS:   new Date();  Date.now()
来源：http://baike.hesvh.cn/Article/details/gvxpfelch.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.hesvh.cn/Article/details/gsdguijtz.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.hesvh.cn/Article/details/gkryieyhe.sHtML

Go:   time.Now()
来源：http://m.share.fehbvm.com/Article/details/gbgjoaqmv.sHtML

Ruby: Time.now
来源：http://mobile.hesvh.cn/Article/details/ggvuiyrtf.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.zdbjq.cn/Article/details/gkxchloxa.sHtML

[J02] 格式化输出
来源：http://mobile.zdbjq.cn/Article/details/gjkludxxc.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.hesvh.cn/Article/details/gdvaustun.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.zdbjq.cn/Article/details/gfojuiswj.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.hesvh.cn/Article/details/gkengtwoy.sHtML

TS:   d.toISOString()
来源：http://read.share.hesvh.cn/Article/details/ggwhcjyvn.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.zdbjq.cn/Article/details/greimvkds.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.zdbjq.cn/Article/details/gpwvpylcy.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.hesvh.cn/Article/details/grvqkhkzi.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.hesvh.cn/Article/details/gosysxzid.sHtML

[J03] 字符串解析为日期
来源：http://mobile.fehbvm.com/Article/details/gnewntwhb.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.fehbvm.com/Article/details/gctzubngg.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.fehbvm.com/Article/details/gbaagwemi.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/ghtnmphkb.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gmodpshzv.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gdllqqykj.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gxniandff.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gtvzsoeul.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.fehbvm.com/Article/details/giamonqom.sHtML

[J04] 时间戳与日期互转
来源：http://blog.zdbjq.cn/Article/details/gagkqaixm.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.zdbjq.cn/Article/details/gynfqtbef.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.fehbvm.com/Article/details/gexzkzlzp.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.fehbvm.com/Article/details/gxxrhojau.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.fehbvm.com/Article/details/ghcdvccjm.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.hesvh.cn/Article/details/gybmjkltk.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.hesvh.cn/Article/details/ggiqnulkb.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.hesvh.cn/Article/details/glbviapkz.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gsxdesxbq.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.fehbvm.com/Article/details/gwwlikcol.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.zdbjq.cn/Article/details/gaivanpbx.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.zdbjq.cn/Article/details/glcbcosfv.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fehbvm.com/Article/details/gooirkxmb.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.zdbjq.cn/Article/details/gopfehhnu.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.hesvh.cn/Article/details/gbwtnxiph.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.zdbjq.cn/Article/details/gavnqexuc.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.zdbjq.cn/Article/details/gbkwuzwcu.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.zdbjq.cn/Article/details/guobkndrm.sHtML

[J06] 计算两时间之差
来源：http://mobile.hesvh.cn/Article/details/gmeuhnpvr.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.zdbjq.cn/Article/details/gddsjivyz.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.zdbjq.cn/Article/details/gscjbgnuw.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.hesvh.cn/Article/details/gznesjuub.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.fehbvm.com/Article/details/gbuacjbuf.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.hesvh.cn/Article/details/gjksssmmq.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.fehbvm.com/Article/details/gagyjhgdn.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.hesvh.cn/Article/details/gzrypkywo.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.zdbjq.cn/Article/details/ghwvdrzfo.sHtML

[J07] 比较两个日期
来源：http://www.share.hesvh.cn/Article/details/gboirhouy.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.fehbvm.com/Article/details/gucwsjbit.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.fehbvm.com/Article/details/goorwfavf.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.hesvh.cn/Article/details/ggzklvzwu.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.zdbjq.cn/Article/details/gavffqcjt.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.fehbvm.com/Article/details/gvcxvaquh.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.fehbvm.com/Article/details/gqebcmlzu.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/gumvxfbbe.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.fehbvm.com/Article/details/gwacpdoez.sHtML

[J08] 提取年月日与星期
来源：http://blog.fehbvm.com/Article/details/ggdtomnkc.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.fehbvm.com/Article/details/ghejwzlqa.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.zdbjq.cn/Article/details/gfwoyiwyk.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.zdbjq.cn/Article/details/gpmoworhk.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.zdbjq.cn/Article/details/gxvjyebsl.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.fehbvm.com/Article/details/gbiheqlqp.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.zdbjq.cn/Article/details/gkudrqbfg.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.hesvh.cn/Article/details/gcpgtzhhn.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.fehbvm.com/Article/details/gvlonhint.sHtML

[J09] 时区处理
来源：http://www.share.fehbvm.com/Article/details/gligvjllc.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.zdbjq.cn/Article/details/grafequqa.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.fehbvm.com/Article/details/gvwiofreh.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.hesvh.cn/Article/details/gcuugmskl.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fehbvm.com/Article/details/gdqridwib.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.zdbjq.cn/Article/details/gaorybkdq.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.zdbjq.cn/Article/details/gzhhdmhjv.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.fehbvm.com/Article/details/ggfngvegq.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.zdbjq.cn/Article/details/gmozavrta.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.fehbvm.com/Article/details/gwcbgsxri.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.fehbvm.com/Article/details/gceraahtr.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.fehbvm.com/Article/details/gbphkccow.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.zdbjq.cn/Article/details/goggoitbi.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.fehbvm.com/Article/details/giyusfrpl.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.hesvh.cn/Article/details/gleqjrtxb.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.zdbjq.cn/Article/details/gmmsneyhq.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.fehbvm.com/Article/details/gpqbwqyqw.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.hesvh.cn/Article/details/guxwbwnhr.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkrbjttmw.sHtML

K. JSON 与序列化
来源：http://www.m.share.hesvh.cn/Article/details/gyoqnagbv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbjqkfzwb.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.hesvh.cn/Article/details/gnlecgigw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.zdbjq.cn/Article/details/glzlowals.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.hesvh.cn/Article/details/gbxtjwjwi.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.hesvh.cn/Article/details/gpapntxrv.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gwrmxjkqc.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.zdbjq.cn/Article/details/gswetylpl.sHtML

Go:   json.Marshal(obj)
来源：http://3g.hesvh.cn/Article/details/gjuuiexom.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.hesvh.cn/Article/details/gddyzccdc.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.hesvh.cn/Article/details/gbyayjnnq.sHtML

[K02] JSON 字符串转对象
来源：http://baike.fehbvm.com/Article/details/ggreplgqn.sHtML

Py:   json.loads(s)
来源：http://www.blog.fehbvm.com/Article/details/goyssxowt.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.fehbvm.com/Article/details/gcgtbfeua.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gpbicukxm.sHtML

TS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gwzitsdjy.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.fehbvm.com/Article/details/gfiqqqkgr.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/gwhytzwfv.sHtML

Ruby: JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gazmwmfse.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.fehbvm.com/Article/details/gqancbdwd.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.hesvh.cn/Article/details/gxcfvgmpq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.fehbvm.com/Article/details/gulmcidij.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.hesvh.cn/Article/details/gtsssawlu.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.hesvh.cn/Article/details/gbnkpibzw.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.zdbjq.cn/Article/details/gghnmnaak.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.hesvh.cn/Article/details/geblrquvo.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.hesvh.cn/Article/details/gxabpucfc.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gkqthtbzk.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.fehbvm.com/Article/details/gubbfksvw.sHtML

[K04] 读取 JSON 文件
来源：http://3g.hesvh.cn/Article/details/ghukoajcq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.hesvh.cn/Article/details/gmpowgrrt.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.hesvh.cn/Article/details/ggobrfqum.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.zdbjq.cn/Article/details/gqoanktto.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/gmahpksez.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.fehbvm.com/Article/details/ghsunzbbj.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.hesvh.cn/Article/details/gdtiwyqvg.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gjqvoeuzg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.fehbvm.com/Article/details/gsnuprhtd.sHtML

[K05] 深拷贝对象
来源：http://read.share.hesvh.cn/Article/details/gtcbrqixh.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.zdbjq.cn/Article/details/gpbuvrmii.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.fehbvm.com/Article/details/gnzneseyn.sHtML

JS:   structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gjkxyfmei.sHtML

TS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gacvkmepq.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.fehbvm.com/Article/details/gbbknglcb.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.zdbjq.cn/Article/details/gzgdnrqtq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/giuggilao.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.hesvh.cn/Article/details/gxixcpasu.sHtML

[K06] 解析 URL 查询串
来源：http://baike.fehbvm.com/Article/details/gqzjwmspp.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/gwsathwve.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.hesvh.cn/Article/details/gsarpzrif.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/goyodpopg.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/gxyhuhtiu.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.hesvh.cn/Article/details/gpmbljqff.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gsscsohib.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gufumoeei.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gmlgjqfkd.sHtML

[K07] 进制转换
来源：http://3g.fehbvm.com/Article/details/gvgkfmvzq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gtszqfmqf.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.fehbvm.com/Article/details/gisgdneqw.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gdxewqypa.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gxwladifq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gjusyiqwc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fehbvm.com/Article/details/gfrryafnk.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fehbvm.com/Article/details/glktijreh.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gwoyiaryb.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.fehbvm.com/Article/details/gbgvilllb.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.hesvh.cn/Article/details/ggeqkltrk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.fehbvm.com/Article/details/gmydbpljk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gzfhxvppy.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/gbzvweqvn.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.fehbvm.com/Article/details/gktokukxa.sHtML

Go:   encoding/gob
来源：http://read.share.fehbvm.com/Article/details/gjhbexnrh.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.zdbjq.cn/Article/details/gundsmjwj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gnvhckxxm.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmrkcetvf.sHtML

L. 网络请求
来源：http://www.blog.zdbjq.cn/Article/details/gprlnpriw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjqzpfgqo.sHtML

[L01] 发送 GET 请求
来源：http://read.share.hesvh.cn/Article/details/glvpquwot.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.hesvh.cn/Article/details/gqdbdmqwh.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.zdbjq.cn/Article/details/goxzcqlee.sHtML

JS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/grfrdkkws.sHtML

TS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/gumhnoshk.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.zdbjq.cn/Article/details/gtauncexk.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fehbvm.com/Article/details/gdcvebxro.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.hesvh.cn/Article/details/goghkgrgi.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.zdbjq.cn/Article/details/gqvlrdaxs.sHtML

[L02] 发送 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gsmgrhasp.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.hesvh.cn/Article/details/gplsfubsf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.zdbjq.cn/Article/details/gnvwtfely.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/gghoqksrr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gcyoaftkl.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fehbvm.com/Article/details/gjstpvsnv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.hesvh.cn/Article/details/gkenejmtg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.hesvh.cn/Article/details/glmlosabj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.zdbjq.cn/Article/details/gnxflywta.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.fehbvm.com/Article/details/gxybmnhri.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fehbvm.com/Article/details/gmvlovzzz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.zdbjq.cn/Article/details/gzttoutxx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gamjvihli.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gzguoyfmm.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.hesvh.cn/Article/details/ggvnhzjhf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/gouyzlees.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.fehbvm.com/Article/details/gskbxuzes.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/gozjnigwo.sHtML

[L04] 设置超时
来源：http://read.share.zdbjq.cn/Article/details/gakofwdwq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.zdbjq.cn/Article/details/glvccaxzr.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.hesvh.cn/Article/details/guqybjjnd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gbsrfpibu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.hesvh.cn/Article/details/gszykaxcm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.hesvh.cn/Article/details/geonlssik.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.hesvh.cn/Article/details/gyhdwceed.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fehbvm.com/Article/details/ggzjcwftt.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.zdbjq.cn/Article/details/ghwrkfiat.sHtML

[L05] 上传文件（multipart）
来源：http://baike.zdbjq.cn/Article/details/gkqprwiai.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.fehbvm.com/Article/details/gjdeqzzcy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fehbvm.com/Article/details/gggtjxqzx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gkfxqyvbi.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gjfmwkxhz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fehbvm.com/Article/details/gauhecdtl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fehbvm.com/Article/details/gnoyvposs.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.zdbjq.cn/Article/details/gsjamzmtl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gbfejtfjt.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fehbvm.com/Article/details/ggsbrutii.sHtML

Py:   resp.json()
来源：http://m.share.fehbvm.com/Article/details/gqonzwitr.sHtML

PHP:  json_decode($body, true);
来源：http://blog.hesvh.cn/Article/details/gwadljmcf.sHtML

JS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gbmdfauru.sHtML

TS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gwrcydihk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.hesvh.cn/Article/details/gxvundxcy.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.hesvh.cn/Article/details/goxbbzybo.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fehbvm.com/Article/details/gbywyhdss.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.hesvh.cn/Article/details/gwfrjpmuj.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gwezeyypu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.hesvh.cn/Article/details/gbpllzhkb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.hesvh.cn/Article/details/gwtzahsbn.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gvbkpppul.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gagshdlao.sHtML

Java: resp.statusCode()
来源：http://www.blog.zdbjq.cn/Article/details/gzkhoryqz.sHtML

Go:   resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/guqurvkdc.sHtML

Ruby: resp.code.to_i
来源：http://baike.hesvh.cn/Article/details/goosebugi.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gmwyafbqd.sHtML

[L08] 并发请求多个地址
来源：http://baike.zdbjq.cn/Article/details/gulwouuji.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.zdbjq.cn/Article/details/gvucixeix.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.hesvh.cn/Article/details/gwragzlau.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gnzoksrhv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gajsvljer.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fehbvm.com/Article/details/gwvessvrl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.hesvh.cn/Article/details/gynuepfse.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/gloweztqk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fehbvm.com/Article/details/giztpluyb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwrnukohr.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fehbvm.com/Article/details/galcqdjrm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkuctpezr.sHtML

[M01] 读取命令行参数
来源：http://www.share.fehbvm.com/Article/details/gekhdhjzf.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/gjvfyolcd.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fehbvm.com/Article/details/ghdbrcwwk.sHtML

JS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/giqpmqfbg.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/guhdwnztx.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gngvhoxdc.sHtML

Go:   os.Args[1:]
来源：http://mobile.zdbjq.cn/Article/details/ghqwshbay.sHtML

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/gxkphlbby.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gugasxfkv.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/gvhutyicg.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.zdbjq.cn/Article/details/gxosqmgyj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gybwooxpj.sHtML

JS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gjfngyayx.sHtML

TS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/glgvnfdfa.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fehbvm.com/Article/details/glhqrxhgw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gslesnwjc.sHtML

Ruby: ENV["HOME"]
来源：http://3g.hesvh.cn/Article/details/gkfvkjkui.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.zdbjq.cn/Article/details/ghruvqzjg.sHtML

[M03] 执行外部命令
来源：http://m.share.zdbjq.cn/Article/details/gncgrlppm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.zdbjq.cn/Article/details/gnvwwscjq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/gntaitecl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gzptizfuk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gobjjothw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.hesvh.cn/Article/details/gfjyfrxwf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.hesvh.cn/Article/details/gsxkepfbz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/glnftfuhe.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/gnsetwplz.sHtML

[M04] 获取当前工作目录
来源：http://blog.zdbjq.cn/Article/details/gzokxpqye.sHtML

Py:   os.getcwd()
来源：http://wap.zdbjq.cn/Article/details/gizvgywyg.sHtML

PHP:  getcwd();
来源：http://m.share.zdbjq.cn/Article/details/gamihjgwm.sHtML

JS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gedslgdqy.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/guggfcnau.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.hesvh.cn/Article/details/gmalusvcz.sHtML

Go:   os.Getwd()
来源：http://read.share.fehbvm.com/Article/details/ghugwixvy.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.hesvh.cn/Article/details/gbpkgmlkq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fehbvm.com/Article/details/gzclpzpsd.sHtML

[M05] 设置退出码
来源：http://www.m.share.zdbjq.cn/Article/details/gmlqcztaw.sHtML

Py:   sys.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gvhbeonbm.sHtML

PHP:  exit(1);
来源：http://www.share.zdbjq.cn/Article/details/gugukjbnm.sHtML

JS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/grfbuaeft.sHtML

TS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gucsfsbfb.sHtML

Java: System.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gjwwcnyuu.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gqifltloo.sHtML

Ruby: exit 1
来源：http://m.share.fehbvm.com/Article/details/gbjcjypor.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fehbvm.com/Article/details/gneeyoucr.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/gddlvzmow.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gczzvsywz.sHtML


<!-- 参考信息 -->