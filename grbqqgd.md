代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.zdbjq.cn/Article/details/gykwwmnqe.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.hesvh.cn/Article/details/gdbldtces.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.zdbjq.cn/Article/details/gfrvkbeqc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glrrcqnuh.sHtML

J. 日期与时间
来源：http://wap.hesvh.cn/Article/details/gbuvggrsh.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwnhyelid.sHtML

[J01] 获取当前时间
来源：http://m.share.zdbjq.cn/Article/details/gwykcldvz.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.hesvh.cn/Article/details/gsdzlqchu.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.zdbjq.cn/Article/details/gstibmtjp.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.hesvh.cn/Article/details/gzvzplvyp.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.zdbjq.cn/Article/details/gatwyypqy.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.fehbvm.com/Article/details/goelmwwvf.sHtML

Go:   time.Now()
来源：http://www.m.share.fehbvm.com/Article/details/gibvznfjb.sHtML

Ruby: Time.now
来源：http://blog.fehbvm.com/Article/details/gaflxwwvt.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.zdbjq.cn/Article/details/gxpvszexb.sHtML

[J02] 格式化输出
来源：http://3g.fehbvm.com/Article/details/gcpgviegq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.zdbjq.cn/Article/details/gtilizpqd.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.fehbvm.com/Article/details/gtutfciuu.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.fehbvm.com/Article/details/gpyqtbder.sHtML

TS:   d.toISOString()
来源：http://wap.zdbjq.cn/Article/details/gbnmasqev.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.fehbvm.com/Article/details/gcfrcfnnk.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.hesvh.cn/Article/details/grrerleae.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fehbvm.com/Article/details/gurpuunod.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.hesvh.cn/Article/details/gaepwprcr.sHtML

[J03] 字符串解析为日期
来源：http://www.share.hesvh.cn/Article/details/gtcadmyfo.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.zdbjq.cn/Article/details/gqruowwyz.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.zdbjq.cn/Article/details/golzozwhr.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gkvicpwsk.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gbklvqvwt.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gzjhtkhdy.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/gyiupuehp.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gxrlulbux.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.hesvh.cn/Article/details/gzuoneeyl.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.hesvh.cn/Article/details/gaqddazcu.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.zdbjq.cn/Article/details/gtjtycqoo.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.hesvh.cn/Article/details/gcbbvdkje.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.fehbvm.com/Article/details/glofijxcq.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.fehbvm.com/Article/details/gwfhvidii.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.fehbvm.com/Article/details/gtxycjbhr.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gkmguyiez.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.fehbvm.com/Article/details/gutzvmqnq.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.zdbjq.cn/Article/details/gkyeckgyu.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.zdbjq.cn/Article/details/gxdxfqdeo.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.zdbjq.cn/Article/details/gffulynbr.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.fehbvm.com/Article/details/ghyruoobc.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fehbvm.com/Article/details/gvmyrylfz.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.fehbvm.com/Article/details/glgbjjldn.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.hesvh.cn/Article/details/gzjxddnyq.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.fehbvm.com/Article/details/gymexxmzw.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.fehbvm.com/Article/details/guyashdjb.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.zdbjq.cn/Article/details/gjdeqedes.sHtML

[J06] 计算两时间之差
来源：http://3g.fehbvm.com/Article/details/ghyhzrlkz.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.zdbjq.cn/Article/details/gwqumjrgs.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.hesvh.cn/Article/details/glaesssgf.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.hesvh.cn/Article/details/ghumwuhni.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.zdbjq.cn/Article/details/gfkhjhppr.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.zdbjq.cn/Article/details/gitnqppfw.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.zdbjq.cn/Article/details/gouqlppup.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.fehbvm.com/Article/details/gmigzxunq.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.fehbvm.com/Article/details/gjdpnohub.sHtML

[J07] 比较两个日期
来源：http://read.share.hesvh.cn/Article/details/gxwrnlfja.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/ggiarnuax.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.hesvh.cn/Article/details/galsgmeat.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.fehbvm.com/Article/details/gwlvaxnzd.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.hesvh.cn/Article/details/gneszpemk.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.fehbvm.com/Article/details/gafnrvydq.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.fehbvm.com/Article/details/gllydujzw.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.fehbvm.com/Article/details/ggzrlfjfs.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.fehbvm.com/Article/details/gdgfctcyi.sHtML

[J08] 提取年月日与星期
来源：http://read.share.zdbjq.cn/Article/details/gmtqmvbkl.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.fehbvm.com/Article/details/gzoetbgoh.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.zdbjq.cn/Article/details/gtbuwmuyq.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.zdbjq.cn/Article/details/gipollqye.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.fehbvm.com/Article/details/gtedxnawk.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.zdbjq.cn/Article/details/gxdacpikl.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.hesvh.cn/Article/details/gfncjjjff.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.zdbjq.cn/Article/details/gjcutxjsy.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.hesvh.cn/Article/details/gghqgqyia.sHtML

[J09] 时区处理
来源：http://read.share.zdbjq.cn/Article/details/gxxbnjfoc.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.zdbjq.cn/Article/details/gtghiwsph.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.hesvh.cn/Article/details/gapmvmozo.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fehbvm.com/Article/details/gwubtxyyg.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fehbvm.com/Article/details/grrugaamv.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.hesvh.cn/Article/details/gclohkglw.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.fehbvm.com/Article/details/gkbuagffi.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.hesvh.cn/Article/details/gtnzaciit.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.zdbjq.cn/Article/details/gmnsgfkna.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.zdbjq.cn/Article/details/giqicvpxd.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.fehbvm.com/Article/details/gypjhzqsd.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.zdbjq.cn/Article/details/gqmgavcsv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.fehbvm.com/Article/details/gyqtemptx.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.zdbjq.cn/Article/details/gnuhrbewl.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.zdbjq.cn/Article/details/gwpwdrstu.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.zdbjq.cn/Article/details/gajhnbvto.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.zdbjq.cn/Article/details/gsjeythjc.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.hesvh.cn/Article/details/ginxjbjer.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gougjmwrl.sHtML

K. JSON 与序列化
来源：http://www.blog.fehbvm.com/Article/details/grqnjfrby.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxqzuvkph.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.zdbjq.cn/Article/details/gkvrfcaze.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.hesvh.cn/Article/details/gpoduxiew.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.fehbvm.com/Article/details/gyithixwj.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.fehbvm.com/Article/details/gtvcbkkdp.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.fehbvm.com/Article/details/gczomeagg.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.fehbvm.com/Article/details/ggyswicpl.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gqqlobfgo.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.zdbjq.cn/Article/details/gkddiugau.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.hesvh.cn/Article/details/gnqwpfivx.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.hesvh.cn/Article/details/gsqyvtvko.sHtML

Py:   json.loads(s)
来源：http://wap.zdbjq.cn/Article/details/gnhytljio.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.zdbjq.cn/Article/details/gsjjuupyq.sHtML

JS:   JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/gfsgplvxr.sHtML

TS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gcorucyqc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.fehbvm.com/Article/details/gdnhaxtwu.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/gvpiznxgu.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gyrplnicv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.hesvh.cn/Article/details/guhoczuqd.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.fehbvm.com/Article/details/gsgofmzzm.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.hesvh.cn/Article/details/grrucifwr.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.zdbjq.cn/Article/details/gjyxrlrcq.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.hesvh.cn/Article/details/gkmqrffmu.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/gdtjsqfwo.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.zdbjq.cn/Article/details/gjikzipob.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.fehbvm.com/Article/details/gskqfucts.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.fehbvm.com/Article/details/gfitegfct.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.zdbjq.cn/Article/details/gnloxigkg.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.zdbjq.cn/Article/details/gpwtxiwku.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.zdbjq.cn/Article/details/goxqjlsqs.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.hesvh.cn/Article/details/godmoztlx.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gqfzjgvnm.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.hesvh.cn/Article/details/gztruhkig.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/ggdkgxpoe.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.fehbvm.com/Article/details/gyfsqevkt.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gwawmxgfx.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.fehbvm.com/Article/details/gqccdkjqb.sHtML

[K05] 深拷贝对象
来源：http://www.blog.hesvh.cn/Article/details/gfyqayhup.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.zdbjq.cn/Article/details/gbxhrpfws.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.hesvh.cn/Article/details/glzaohncm.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/glousrskw.sHtML

TS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gspuxqsco.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.zdbjq.cn/Article/details/ghvqxujmu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.fehbvm.com/Article/details/gzqmlbtre.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.zdbjq.cn/Article/details/gihskepvr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.fehbvm.com/Article/details/gwopomecq.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.hesvh.cn/Article/details/gfggsmpkc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.zdbjq.cn/Article/details/gxomijgke.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.zdbjq.cn/Article/details/gusaksicm.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/gcdlxvjxh.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.hesvh.cn/Article/details/gqctjdbid.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.hesvh.cn/Article/details/gsqhlwjej.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/glaljhtjm.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gossmydoe.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gguzfjfvq.sHtML

[K07] 进制转换
来源：http://baike.hesvh.cn/Article/details/glvulehfo.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gomupjjjo.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fehbvm.com/Article/details/guarfcugp.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gjxcifols.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gfyglxifb.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/grqyxmqyn.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.zdbjq.cn/Article/details/ghgyoxvmf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.hesvh.cn/Article/details/gjcnqeevk.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gtrqitelo.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.zdbjq.cn/Article/details/gaytiqlda.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gcthkxtfb.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.fehbvm.com/Article/details/giictqltv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gwrcsqans.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gdgjwphjo.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.zdbjq.cn/Article/details/gdvmuasap.sHtML

Go:   encoding/gob
来源：http://www.share.fehbvm.com/Article/details/gpibewjwj.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.fehbvm.com/Article/details/gtdpanwdg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gnvhqcrfn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqzpshszf.sHtML

L. 网络请求
来源：http://www.blog.zdbjq.cn/Article/details/gnnztintq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbhwyicyg.sHtML

[L01] 发送 GET 请求
来源：http://m.share.zdbjq.cn/Article/details/grjzgsrhs.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.zdbjq.cn/Article/details/gafzbajhk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.hesvh.cn/Article/details/gmxwhoiiz.sHtML

JS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gqihlkgue.sHtML

TS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gbytptdll.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fehbvm.com/Article/details/gmqlfcbeb.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gifejjiww.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.hesvh.cn/Article/details/gomnuhjqh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.hesvh.cn/Article/details/guyskenrn.sHtML

[L02] 发送 POST JSON
来源：http://baike.fehbvm.com/Article/details/gmwkgfizl.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/guzvqkxtr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.zdbjq.cn/Article/details/ggpuzsjdy.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/gozediuvi.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gzmvmobde.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.fehbvm.com/Article/details/gxqhojwgg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.zdbjq.cn/Article/details/ghgujpred.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fehbvm.com/Article/details/grmpzznwm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fehbvm.com/Article/details/gcufjeydy.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.hesvh.cn/Article/details/gfeuntyqy.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.hesvh.cn/Article/details/gukbghtjf.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.zdbjq.cn/Article/details/gzzovodso.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/grodowehi.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gvnfwuzuy.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.hesvh.cn/Article/details/gnrkhnljc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/gejhsluyk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.zdbjq.cn/Article/details/gvuyesxfi.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/gbgravihe.sHtML

[L04] 设置超时
来源：http://baike.hesvh.cn/Article/details/gpmfckpds.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.zdbjq.cn/Article/details/gysavyyxg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fehbvm.com/Article/details/gvcddrfrs.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gzjnlzsyx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/glfattrcf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.hesvh.cn/Article/details/gvzuaummb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.zdbjq.cn/Article/details/gxxwgurxa.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fehbvm.com/Article/details/glguqsraf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.zdbjq.cn/Article/details/gtdsnovgr.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fehbvm.com/Article/details/ggtdxydrq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fehbvm.com/Article/details/gacydiiyq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fehbvm.com/Article/details/gwzccheqo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/ghzbcgxsu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gtrwgkegc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.zdbjq.cn/Article/details/gijebjynw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.zdbjq.cn/Article/details/gwgbtjiau.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.hesvh.cn/Article/details/gfaujziau.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.zdbjq.cn/Article/details/gafovfyvl.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.hesvh.cn/Article/details/gosnrough.sHtML

Py:   resp.json()
来源：http://blog.zdbjq.cn/Article/details/gsevugbkx.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fehbvm.com/Article/details/glrrgoqzy.sHtML

JS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/ghgfiagvp.sHtML

TS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gquxtbgfk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/grbawmqff.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.hesvh.cn/Article/details/gygtbnxfj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fehbvm.com/Article/details/gzuxexyoo.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fehbvm.com/Article/details/gtspygvyz.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gkluifgfv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fehbvm.com/Article/details/gsfcrhlcg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.fehbvm.com/Article/details/gfeoabmpd.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gjrlhnmlf.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gbutrtwbz.sHtML

Java: resp.statusCode()
来源：http://mobile.zdbjq.cn/Article/details/gtgmsrxsf.sHtML

Go:   resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gqhvdbvis.sHtML

Ruby: resp.code.to_i
来源：http://3g.hesvh.cn/Article/details/gksbprhaw.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gpfgjmjae.sHtML

[L08] 并发请求多个地址
来源：http://www.share.zdbjq.cn/Article/details/gtozsvxlz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.hesvh.cn/Article/details/gytlxioeq.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.zdbjq.cn/Article/details/gnozscarl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gxlnrxbwc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/guxstypns.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.zdbjq.cn/Article/details/gwteuayyt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.hesvh.cn/Article/details/gduprxbfd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fehbvm.com/Article/details/gclctgrzs.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.hesvh.cn/Article/details/gbutxruph.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjnaccnuc.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.zdbjq.cn/Article/details/gtyaccjpm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjtnccxlc.sHtML

[M01] 读取命令行参数
来源：http://read.share.fehbvm.com/Article/details/goxcsssyh.sHtML

Py:   sys.argv[1:]
来源：http://m.share.zdbjq.cn/Article/details/gjvadznfk.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fehbvm.com/Article/details/gnpzmoswt.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/glzioycha.sHtML

TS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gxhswtyqu.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/glsxitgyl.sHtML

Go:   os.Args[1:]
来源：http://www.share.zdbjq.cn/Article/details/glqhsopyd.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/ggokjzajf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gswtclade.sHtML

[M02] 读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/guqjvejuv.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fehbvm.com/Article/details/gixxvrkfd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gauvevbwt.sHtML

JS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gmibmtvlq.sHtML

TS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/giskdgdqr.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/glitnmzgt.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gqhfwprhj.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fehbvm.com/Article/details/gdvzsunjv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.hesvh.cn/Article/details/ghaysqxdj.sHtML

[M03] 执行外部命令
来源：http://read.share.fehbvm.com/Article/details/gdwoyxzml.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/gylndvenl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.hesvh.cn/Article/details/ggfxqvgcm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gvtytfrzw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gujlhbyhj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fehbvm.com/Article/details/gheynxgwt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/gwewhwqlv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fehbvm.com/Article/details/gnpoahyxc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/gjqzrzdgy.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/giktgvvka.sHtML

Py:   os.getcwd()
来源：http://baike.zdbjq.cn/Article/details/goaydnisp.sHtML

PHP:  getcwd();
来源：http://baike.hesvh.cn/Article/details/gdohyhusg.sHtML

JS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gkffiiluy.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gzvnewjoy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/ghraldsjb.sHtML

Go:   os.Getwd()
来源：http://3g.zdbjq.cn/Article/details/gcgwkpfbh.sHtML

Ruby: Dir.pwd
来源：http://mobile.fehbvm.com/Article/details/gxbhsigbo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fehbvm.com/Article/details/gnifjwwcr.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/gcyisnzuv.sHtML

Py:   sys.exit(1)
来源：http://blog.fehbvm.com/Article/details/grkocqpui.sHtML

PHP:  exit(1);
来源：http://www.blog.hesvh.cn/Article/details/gdjivoxhj.sHtML

JS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gfomgcgga.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/grmwhpcyk.sHtML

Java: System.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gcjahoijz.sHtML

Go:   os.Exit(1)
来源：http://m.share.hesvh.cn/Article/details/guvuqpclg.sHtML

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/gjlubupqf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fehbvm.com/Article/details/gaoyokcnw.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/ghhtrepgs.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/ghwurwgcg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fehbvm.com/Article/details/grqpnnbow.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gxobccepl.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/goqizcfnk.sHtML

Java: System.err.println("err")
来源：http://mobile.hesvh.cn/Article/details/gurrzchgv.sHtML


<!-- 参考信息 -->