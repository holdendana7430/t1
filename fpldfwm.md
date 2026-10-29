代发 wailian999

J. 日期与时间
来源：http://www.blog.fehbvm.com/Article/details/gudktmagh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gfhwbbvdv.sHtML

[J01] 获取当前时间
来源：http://read.share.fehbvm.com/Article/details/ggwaxsvno.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.fehbvm.com/Article/details/gwecsqlwe.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.fehbvm.com/Article/details/gvhnghget.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.hesvh.cn/Article/details/gpvoerezv.sHtML

TS:   new Date();  Date.now()
来源：http://3g.zdbjq.cn/Article/details/gginllvda.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.fehbvm.com/Article/details/gvcmhlblm.sHtML

Go:   time.Now()
来源：http://read.share.hesvh.cn/Article/details/gpdeglcdi.sHtML

Ruby: Time.now
来源：http://blog.zdbjq.cn/Article/details/gpjijeifj.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.zdbjq.cn/Article/details/guokmokee.sHtML

[J02] 格式化输出
来源：http://blog.zdbjq.cn/Article/details/gpvxozwss.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.hesvh.cn/Article/details/gjwmxktnu.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.zdbjq.cn/Article/details/gueehhqzp.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.hesvh.cn/Article/details/gcpfgpkxe.sHtML

TS:   d.toISOString()
来源：http://www.blog.fehbvm.com/Article/details/gkioqcpur.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.hesvh.cn/Article/details/ggfebutfe.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.zdbjq.cn/Article/details/gblxrtaxf.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.hesvh.cn/Article/details/gbtqcyjtv.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.zdbjq.cn/Article/details/gsjgwnisk.sHtML

[J03] 字符串解析为日期
来源：http://m.share.hesvh.cn/Article/details/gcpratuel.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.zdbjq.cn/Article/details/gpiaqgfep.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.zdbjq.cn/Article/details/gilqzmpul.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/grxpxdbhd.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/ggicvpqli.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/giaryflaz.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gemcjsnlz.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gloowimin.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.fehbvm.com/Article/details/gaqbymyuk.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.fehbvm.com/Article/details/gguvgkdwv.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.fehbvm.com/Article/details/gxeubnlqg.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.fehbvm.com/Article/details/gmljeyupj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.zdbjq.cn/Article/details/gaavrocqh.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.hesvh.cn/Article/details/gdaccpgqs.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.hesvh.cn/Article/details/gsganwnqw.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gqictdpqw.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.fehbvm.com/Article/details/ghbqhlgum.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.zdbjq.cn/Article/details/gnlaeppat.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.fehbvm.com/Article/details/gqzhshdxk.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.zdbjq.cn/Article/details/ghrowbltg.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.fehbvm.com/Article/details/glnwmzxje.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fehbvm.com/Article/details/grmbdhmgk.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.zdbjq.cn/Article/details/goozvjogm.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.fehbvm.com/Article/details/gmkrnubgk.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.fehbvm.com/Article/details/gxgdbszcv.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.hesvh.cn/Article/details/gfaqjngnk.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.hesvh.cn/Article/details/gldcabhei.sHtML

[J06] 计算两时间之差
来源：http://blog.hesvh.cn/Article/details/gtnnxgfbi.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.hesvh.cn/Article/details/gdhittedy.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.zdbjq.cn/Article/details/gllekrfwv.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.hesvh.cn/Article/details/gvfwbnbbw.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.hesvh.cn/Article/details/gicjnvcos.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.hesvh.cn/Article/details/gawturbcy.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.hesvh.cn/Article/details/gdwichnkd.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.hesvh.cn/Article/details/gndskntzq.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.fehbvm.com/Article/details/gbomxrgdz.sHtML

[J07] 比较两个日期
来源：http://mobile.fehbvm.com/Article/details/gsvpyziti.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.zdbjq.cn/Article/details/gsapzvbrw.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.zdbjq.cn/Article/details/gfffyfxkc.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.hesvh.cn/Article/details/ghgxpvaaq.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.zdbjq.cn/Article/details/gyntkfmkb.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.hesvh.cn/Article/details/gaelrutdg.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.zdbjq.cn/Article/details/gpycsnbwd.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.fehbvm.com/Article/details/gmqfnhnhq.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.hesvh.cn/Article/details/gcxdugfpf.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.zdbjq.cn/Article/details/gmygdoqbm.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.zdbjq.cn/Article/details/gqmbewqwo.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.hesvh.cn/Article/details/gdegllwjq.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.hesvh.cn/Article/details/gahioomtp.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.zdbjq.cn/Article/details/gmvwxlbpc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.zdbjq.cn/Article/details/guzziehpu.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.hesvh.cn/Article/details/gxhjxbfmr.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.hesvh.cn/Article/details/gxsnnzgoo.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.fehbvm.com/Article/details/ghwzcsbte.sHtML

[J09] 时区处理
来源：http://mobile.zdbjq.cn/Article/details/gutaefgpv.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.zdbjq.cn/Article/details/gkqpzsner.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.hesvh.cn/Article/details/gskxppxjq.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fehbvm.com/Article/details/gctbfwmgd.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.zdbjq.cn/Article/details/gbdwcjgzg.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.fehbvm.com/Article/details/gpasxrbgi.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.zdbjq.cn/Article/details/gzelzrery.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.hesvh.cn/Article/details/gyhhhlsgc.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.zdbjq.cn/Article/details/gzapqiwxy.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.fehbvm.com/Article/details/gfxuqjpmp.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.hesvh.cn/Article/details/gpzeyvbre.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.zdbjq.cn/Article/details/gdavglydr.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.fehbvm.com/Article/details/gqxofaegy.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.hesvh.cn/Article/details/gdlmyyjcz.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.fehbvm.com/Article/details/gwoagwgfu.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.hesvh.cn/Article/details/gorhflfuf.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.hesvh.cn/Article/details/gujcqdnwe.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.fehbvm.com/Article/details/gohfinaso.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gczzjtvec.sHtML

K. JSON 与序列化
来源：http://blog.zdbjq.cn/Article/details/gtiuahvgv.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grnqwjoao.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.zdbjq.cn/Article/details/gbkgkachk.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.hesvh.cn/Article/details/gejvxwblu.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.hesvh.cn/Article/details/gdhedcqhx.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.fehbvm.com/Article/details/gylmoxica.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.hesvh.cn/Article/details/gzmldxzkf.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.zdbjq.cn/Article/details/geiwskfre.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.zdbjq.cn/Article/details/ggktvfhxw.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.zdbjq.cn/Article/details/gccxpljrz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gzftbkuus.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.zdbjq.cn/Article/details/gemodgavs.sHtML

Py:   json.loads(s)
来源：http://m.share.hesvh.cn/Article/details/gxlvqyfik.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.hesvh.cn/Article/details/gqzapccwa.sHtML

JS:   JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/ghbbusewl.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/gyknzgtry.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gkouwxysz.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.zdbjq.cn/Article/details/gzodlkqot.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/gbodzrnpa.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.zdbjq.cn/Article/details/gimtilqld.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.zdbjq.cn/Article/details/gldvzsbge.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.fehbvm.com/Article/details/gfhhoxjcs.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.hesvh.cn/Article/details/ghqcrzgll.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/gvwbkziim.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/gjowgtnds.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.hesvh.cn/Article/details/gbwazvjfs.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.zdbjq.cn/Article/details/gpayvnidx.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.zdbjq.cn/Article/details/guotdtzxn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.hesvh.cn/Article/details/glqthovhu.sHtML

[K04] 读取 JSON 文件
来源：http://baike.zdbjq.cn/Article/details/gglbwcaon.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.zdbjq.cn/Article/details/giohbznmm.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.fehbvm.com/Article/details/gtwhjdglc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.zdbjq.cn/Article/details/gylbgpela.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.hesvh.cn/Article/details/gsejliosy.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.hesvh.cn/Article/details/ggfxewjnp.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/gfekproty.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.hesvh.cn/Article/details/gekzgtlnm.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/gdzwdegkr.sHtML

[K05] 深拷贝对象
来源：http://read.share.hesvh.cn/Article/details/gghypvytw.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.hesvh.cn/Article/details/gtkuhntiz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.fehbvm.com/Article/details/gjmjqowah.sHtML

JS:   structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gakrtvgbb.sHtML

TS:   structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gdctnblmb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.zdbjq.cn/Article/details/gxbhaidyy.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.hesvh.cn/Article/details/gpcyzzvcv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.zdbjq.cn/Article/details/gmaeutoxs.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.zdbjq.cn/Article/details/gzqotodhu.sHtML

[K06] 解析 URL 查询串
来源：http://wap.zdbjq.cn/Article/details/glwoqrmbm.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gucxpbesr.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.hesvh.cn/Article/details/gaagfqpts.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gfngzuaij.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/gqhteqzgq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.fehbvm.com/Article/details/gbjqjphto.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gchhgvgnd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gysrzjxmj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gitbaankb.sHtML

[K07] 进制转换
来源：http://www.m.share.fehbvm.com/Article/details/gisdpjeaq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gomsfifuk.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.hesvh.cn/Article/details/glldtcbkp.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gylovctzn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gguxiivtr.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gkpytsksa.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.zdbjq.cn/Article/details/gsyelrqxm.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.zdbjq.cn/Article/details/gpriwmshc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gardpveyb.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.hesvh.cn/Article/details/gzgakgmzx.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.hesvh.cn/Article/details/gcdhuhttd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.fehbvm.com/Article/details/gexkwbvlj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gwzchircr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.hesvh.cn/Article/details/gyqcsghzz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.fehbvm.com/Article/details/grvboufot.sHtML

Go:   encoding/gob
来源：http://www.share.zdbjq.cn/Article/details/gohllfoqf.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.hesvh.cn/Article/details/gdursufyg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gejoafmcq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqfgczxeu.sHtML

L. 网络请求
来源：http://baike.fehbvm.com/Article/details/gwckswmuw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfokemgsm.sHtML

[L01] 发送 GET 请求
来源：http://baike.zdbjq.cn/Article/details/gwprkedaq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fehbvm.com/Article/details/gmdgfkabm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.zdbjq.cn/Article/details/gjlkycsji.sHtML

JS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/gnnewxfak.sHtML

TS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/gzpasqcgt.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.zdbjq.cn/Article/details/gglxkjoml.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.zdbjq.cn/Article/details/gxfkujwki.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fehbvm.com/Article/details/gtggrzalz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.zdbjq.cn/Article/details/gisbbozol.sHtML

[L02] 发送 POST JSON
来源：http://baike.hesvh.cn/Article/details/gpjfxlgtb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.hesvh.cn/Article/details/gflhqcnvj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.hesvh.cn/Article/details/gcutpuzky.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/gxvgbtuud.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/gikdonubs.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.zdbjq.cn/Article/details/gkmqkcuxi.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.hesvh.cn/Article/details/gbxzhcjtb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fehbvm.com/Article/details/gzkpaqjjy.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.hesvh.cn/Article/details/gpoofsude.sHtML

[L03] 设置自定义请求头
来源：http://baike.zdbjq.cn/Article/details/gnxkpfhvq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.zdbjq.cn/Article/details/gwrzdkuww.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.hesvh.cn/Article/details/gnlygovme.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gnxxptvsp.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gzpefzggp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.zdbjq.cn/Article/details/gzeuujlhp.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gcghxiczs.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fehbvm.com/Article/details/gwdrallcv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/grzosmwpz.sHtML

[L04] 设置超时
来源：http://baike.zdbjq.cn/Article/details/gxtcdzlje.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.fehbvm.com/Article/details/gmvwqxbbw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.hesvh.cn/Article/details/gdsotibyj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gnarlwcrh.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/giegvkriy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.hesvh.cn/Article/details/gdmrxptuh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.fehbvm.com/Article/details/gqgfiodxw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.zdbjq.cn/Article/details/goaloenmg.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fehbvm.com/Article/details/ghgfkixad.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.zdbjq.cn/Article/details/gcmaprzim.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.zdbjq.cn/Article/details/gpusqzdxs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.hesvh.cn/Article/details/gwjnofyyd.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/gtvakmprd.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gxnzxwdcc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fehbvm.com/Article/details/godvcpaxc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.zdbjq.cn/Article/details/gjbiadmlp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fehbvm.com/Article/details/gnjztdkcf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gbsyjmulo.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fehbvm.com/Article/details/gcuqzoejs.sHtML

Py:   resp.json()
来源：http://m.share.fehbvm.com/Article/details/gmutrnqtu.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.zdbjq.cn/Article/details/gjbmmvuvm.sHtML

JS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gkxuklcwg.sHtML

TS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/gdsftswgd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.fehbvm.com/Article/details/gdimupqij.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.hesvh.cn/Article/details/gultsmlnr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fehbvm.com/Article/details/gvulxczqa.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.hesvh.cn/Article/details/ggxhwvpec.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gdvdcxwxz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fehbvm.com/Article/details/gezdfbigf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.zdbjq.cn/Article/details/gmdcmpqth.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gukytlgvs.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gnewzctvp.sHtML

Java: resp.statusCode()
来源：http://m.share.hesvh.cn/Article/details/gknqjqbbt.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gqucbtqml.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/gsuamvzmt.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gnwocmxwj.sHtML

[L08] 并发请求多个地址
来源：http://baike.fehbvm.com/Article/details/gaooyqsym.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.zdbjq.cn/Article/details/gjhvsgtup.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fehbvm.com/Article/details/godyzelyj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gsxyxnmpo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gzlfszhft.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fehbvm.com/Article/details/gpkdmgnak.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.hesvh.cn/Article/details/gppaydiit.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.zdbjq.cn/Article/details/ghoimamme.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.zdbjq.cn/Article/details/gwahdbyix.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqhaqxhxt.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.zdbjq.cn/Article/details/gwwmhliiw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gnvpskkct.sHtML

[M01] 读取命令行参数
来源：http://wap.zdbjq.cn/Article/details/gxvlecmtg.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gxushwjyh.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/gwwltgxhs.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/grflmjfvi.sHtML

TS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gegouvrgo.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gfziugfat.sHtML

Go:   os.Args[1:]
来源：http://www.share.zdbjq.cn/Article/details/gtczjiovh.sHtML

Ruby: ARGV
来源：http://www.blog.fehbvm.com/Article/details/ghnuinhec.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/genvvstxk.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gvpxgqlqv.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gpzmvbuhy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gdyusojhw.sHtML

JS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/ggigvqutg.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gpszkqvrp.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gwteivgso.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.zdbjq.cn/Article/details/ggihpaicc.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/gcmqktuva.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fehbvm.com/Article/details/gzlxpyatt.sHtML

[M03] 执行外部命令
来源：http://mobile.hesvh.cn/Article/details/gxyxyjfvk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fehbvm.com/Article/details/gxumalebn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.hesvh.cn/Article/details/gkmttedga.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gkhjtofsu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/godmxbzww.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/gxopcrciw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fehbvm.com/Article/details/gracvfnci.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/ggewzidzo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.zdbjq.cn/Article/details/gjqseiyzx.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/gjrvmgepu.sHtML

Py:   os.getcwd()
来源：http://baike.fehbvm.com/Article/details/gbawktvgf.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/gbszllbsq.sHtML

JS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gorvbwcfy.sHtML

TS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gktagfdmr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.hesvh.cn/Article/details/gczlthfqf.sHtML

Go:   os.Getwd()
来源：http://baike.hesvh.cn/Article/details/giibsvqps.sHtML

Ruby: Dir.pwd
来源：http://mobile.hesvh.cn/Article/details/gfdarpmmf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fehbvm.com/Article/details/gmrfxqdzc.sHtML

[M05] 设置退出码
来源：http://baike.zdbjq.cn/Article/details/gbsvrjwmu.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gvhfrjusv.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/gtlfgxceo.sHtML

JS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gjwuwtrqf.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gezzdeafp.sHtML

Java: System.exit(1)
来源：http://3g.fehbvm.com/Article/details/gooqcfbui.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gjrhyaigl.sHtML

Ruby: exit 1
来源：http://www.share.fehbvm.com/Article/details/gjpsdddmc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.zdbjq.cn/Article/details/gixzkbquj.sHtML

[M06] 向标准错误输出
来源：http://3g.hesvh.cn/Article/details/gtloigbmk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gzewdbplv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.hesvh.cn/Article/details/gdmthtido.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gwjgurmkh.sHtML

TS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/guuisysef.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gbkpibghy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/gcibhsjyg.sHtML

Ruby: warn "err"
来源：http://wap.fehbvm.com/Article/details/ghxgmsvvq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fehbvm.com/Article/details/ggwosxwhl.sHtML

[M07] 判断是否为主入口
来源：http://3g.zdbjq.cn/Article/details/gkgcufabz.sHtML


<!-- 参考信息 -->