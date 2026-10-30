代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkuiwemt.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmpxwgal.sHtML

TS:   new Date();  Date.now()
来源：http://wap.fanxiaobao.xyz/Article/details/gtedmetps.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.fanxiaobao.xyz/Article/details/guhrdeboc.sHtML

Go:   time.Now()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorqviudf.sHtML

Ruby: Time.now
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhqfytpi.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.fanxiaobao.xyz/Article/details/gjsmsodmb.sHtML

[J02] 格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmzkzxql.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fanxiaobao.xyz/Article/details/gsjhfnhsu.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.fanxiaobao.xyz/Article/details/gfuftvlik.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqicwsptx.sHtML

TS:   d.toISOString()
来源：http://3g.fanxiaobao.xyz/Article/details/gwiwakplb.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.fanxiaobao.xyz/Article/details/grfvdjkme.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.fanxiaobao.xyz/Article/details/gnolvjkgb.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqsmsddh.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.fanxiaobao.xyz/Article/details/gohaeixse.sHtML

[J03] 字符串解析为日期
来源：http://wap.fanxiaobao.xyz/Article/details/gymnjrbgk.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.fanxiaobao.xyz/Article/details/gglycttpp.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.fanxiaobao.xyz/Article/details/ghrycyhgo.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.fanxiaobao.xyz/Article/details/gnsfcdzym.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.fanxiaobao.xyz/Article/details/gatumnbbt.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.fanxiaobao.xyz/Article/details/ghbnbynti.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.fanxiaobao.xyz/Article/details/gdwplwqxx.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.fanxiaobao.xyz/Article/details/gxzhnpvcq.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.fanxiaobao.xyz/Article/details/gwkmyqlxw.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.fanxiaobao.xyz/Article/details/grvaismrt.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.fanxiaobao.xyz/Article/details/gnarxohwu.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.fanxiaobao.xyz/Article/details/gvuhdxfcn.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.fanxiaobao.xyz/Article/details/gtfrfozbg.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.fanxiaobao.xyz/Article/details/grbewdyxr.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwwxagis.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/gqqdiksgx.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvocnkyud.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.fanxiaobao.xyz/Article/details/gntcwbypa.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbxiegtw.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.fanxiaobao.xyz/Article/details/gduulhyhb.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.fanxiaobao.xyz/Article/details/gcefdiaca.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepentwso.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fanxiaobao.xyz/Article/details/gabyqjohu.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkqudgth.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqntsxyl.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.fanxiaobao.xyz/Article/details/gpeapupwq.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.fanxiaobao.xyz/Article/details/ggbbecffn.sHtML

[J06] 计算两时间之差
来源：http://mobile.fanxiaobao.xyz/Article/details/glskymboz.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpuordgjj.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.fanxiaobao.xyz/Article/details/gxuqxtfju.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.fanxiaobao.xyz/Article/details/gvymgvcxo.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.fanxiaobao.xyz/Article/details/gggobjmgj.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.fanxiaobao.xyz/Article/details/gcuzbidhk.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlaluplf.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.fanxiaobao.xyz/Article/details/gsxtqxnlk.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbkxhazx.sHtML

[J07] 比较两个日期
来源：http://wap.fanxiaobao.xyz/Article/details/gnufbrbkp.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjxmvvvw.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqapnfsud.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.fanxiaobao.xyz/Article/details/gqjwelgjj.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyhgunch.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.fanxiaobao.xyz/Article/details/ggecxbmth.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gojkgweqv.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.fanxiaobao.xyz/Article/details/gprrutzho.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.fanxiaobao.xyz/Article/details/gexkvsnro.sHtML

[J08] 提取年月日与星期
来源：http://blog.fanxiaobao.xyz/Article/details/geoqaaihw.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.fanxiaobao.xyz/Article/details/gwzsemulc.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.fanxiaobao.xyz/Article/details/gzazeqnyw.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdzdzwbc.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlcbidiw.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.fanxiaobao.xyz/Article/details/gpwxmpors.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwtvidyd.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.fanxiaobao.xyz/Article/details/gimdtjokd.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwwuoilp.sHtML

[J09] 时区处理
来源：http://m.share.fanxiaobao.xyz/Article/details/glszrkxyj.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqpmfkoj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.fanxiaobao.xyz/Article/details/gdhhispxq.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fanxiaobao.xyz/Article/details/giazrfuhk.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fanxiaobao.xyz/Article/details/gliheshub.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdpqbqre.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbaodestz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhnhbixe.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnbccgli.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.fanxiaobao.xyz/Article/details/gbggoksyl.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.fanxiaobao.xyz/Article/details/gxoufxgkz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.fanxiaobao.xyz/Article/details/glyzvqumd.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gjdalvnws.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/gmrflroav.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gqphamqxp.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.fanxiaobao.xyz/Article/details/gqhczlmbu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.fanxiaobao.xyz/Article/details/gafnxshiu.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gibsdbawh.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ghdfsqxhq.sHtML

K. JSON 与序列化
来源：http://www.blog.fanxiaobao.xyz/Article/details/givyjckgt.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gxagiakuk.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrdjzoxd.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmmtktxa.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmolrabzz.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdadnkwm.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/ghgfvahmn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guamjprha.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrawldmb.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyendlyv.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gxqmobbcp.sHtML

[K02] JSON 字符串转对象
来源：http://3g.fanxiaobao.xyz/Article/details/gaqzaqinz.sHtML

Py:   json.loads(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqurnoayk.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.fanxiaobao.xyz/Article/details/galhsmlvy.sHtML

JS:   JSON.parse(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gdbbsradn.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsodrihj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.fanxiaobao.xyz/Article/details/gvxgsuoha.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqvauoig.sHtML

Ruby: JSON.parse(s)
来源：http://wap.fanxiaobao.xyz/Article/details/grvwpcywv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.fanxiaobao.xyz/Article/details/ghyrkoufn.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.fanxiaobao.xyz/Article/details/gfukckpxe.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuafddlo.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbrmquju.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gkqfbtfxy.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggoefmzyk.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gubwjzkig.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.fanxiaobao.xyz/Article/details/gkrxmdjou.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gdsedobck.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.fanxiaobao.xyz/Article/details/gglkruasi.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gluikernk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhxzkmfo.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.fanxiaobao.xyz/Article/details/grotmhris.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glabybvxh.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fanxiaobao.xyz/Article/details/ghthdxpyd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzzhsifx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.fanxiaobao.xyz/Article/details/gndikabrz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.fanxiaobao.xyz/Article/details/gziozpdjx.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.fanxiaobao.xyz/Article/details/gypjiuupg.sHtML

[K05] 深拷贝对象
来源：http://wap.fanxiaobao.xyz/Article/details/gqkaonxit.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvhstchr.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhvjrezi.sHtML

JS:   structuredClone(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gnvljslez.sHtML

TS:   structuredClone(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gkilfxlmw.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.fanxiaobao.xyz/Article/details/gngwcvjvi.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.fanxiaobao.xyz/Article/details/gabmjtsna.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.fanxiaobao.xyz/Article/details/gteaaomci.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.fanxiaobao.xyz/Article/details/giwswtvsk.sHtML

[K06] 解析 URL 查询串
来源：http://baike.fanxiaobao.xyz/Article/details/gdeafjqjs.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fanxiaobao.xyz/Article/details/gtyraujkr.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.fanxiaobao.xyz/Article/details/grownrxom.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxinzbmn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghinhyhpi.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.fanxiaobao.xyz/Article/details/gfiyepjbc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwcklqld.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.fanxiaobao.xyz/Article/details/grqzglayo.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.fanxiaobao.xyz/Article/details/gxzbfgsck.sHtML

[K07] 进制转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhszmmpt.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.fanxiaobao.xyz/Article/details/gdesavddz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.fanxiaobao.xyz/Article/details/glibryieb.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.fanxiaobao.xyz/Article/details/gozrechyv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.fanxiaobao.xyz/Article/details/gmplaodux.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzicinlf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpztshti.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.fanxiaobao.xyz/Article/details/gucmjikck.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fanxiaobao.xyz/Article/details/gmfowmblf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.fanxiaobao.xyz/Article/details/grslgusvk.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/ghwkyoqcu.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvfnlhbt.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvdgdmqj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsxptylg.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fanxiaobao.xyz/Article/details/gtuewzglw.sHtML

Go:   encoding/gob
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzyzbuag.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxmcoywf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.fanxiaobao.xyz/Article/details/gimwvgort.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gqytzufal.sHtML

L. 网络请求
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxffjoxl.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gqekmfxse.sHtML

[L01] 发送 GET 请求
来源：http://www.share.fanxiaobao.xyz/Article/details/ganpxklhh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakjazlcs.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqluhkveg.sHtML

JS:   await fetch(url)
来源：http://baike.fanxiaobao.xyz/Article/details/glgrldqzg.sHtML

TS:   await fetch(url)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfxieiyn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.fanxiaobao.xyz/Article/details/gypfzckog.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.fanxiaobao.xyz/Article/details/ggwfqkqkq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.fanxiaobao.xyz/Article/details/gpbgqzmak.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkjnjpeh.sHtML

[L02] 发送 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gwgccyxti.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.fanxiaobao.xyz/Article/details/grkruzvky.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.fanxiaobao.xyz/Article/details/ggmdftsyn.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fanxiaobao.xyz/Article/details/ghsqeeqbe.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrvsfyfb.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fanxiaobao.xyz/Article/details/ghwtjluca.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fanxiaobao.xyz/Article/details/gvoqwrtdj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjyspdcs.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.fanxiaobao.xyz/Article/details/ghiwinogh.sHtML

[L03] 设置自定义请求头
来源：http://blog.fanxiaobao.xyz/Article/details/gamfubhmr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fanxiaobao.xyz/Article/details/gjslmjidv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagrwbkbz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fanxiaobao.xyz/Article/details/ggtnaezcu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fanxiaobao.xyz/Article/details/gzoudumdl.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fanxiaobao.xyz/Article/details/goibmibui.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fanxiaobao.xyz/Article/details/gnorhrsdh.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.fanxiaobao.xyz/Article/details/gzmuwtkqi.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fanxiaobao.xyz/Article/details/gopqlizuu.sHtML

[L04] 设置超时
来源：http://blog.fanxiaobao.xyz/Article/details/grcqwgbmt.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.fanxiaobao.xyz/Article/details/gzfynvxlx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrwtqqql.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggybelvro.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fanxiaobao.xyz/Article/details/gykqfgzxw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.fanxiaobao.xyz/Article/details/ghaugagyc.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogriilhw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fanxiaobao.xyz/Article/details/gexxqbqhh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.fanxiaobao.xyz/Article/details/gkebxyiog.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fanxiaobao.xyz/Article/details/gppwoaiya.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.fanxiaobao.xyz/Article/details/givnwhndj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdeiwpbco.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fanxiaobao.xyz/Article/details/gxizyrshn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fanxiaobao.xyz/Article/details/gepfbpxtx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.fanxiaobao.xyz/Article/details/gkpsdftky.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givrggprg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttgpfiwq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gjxxqdriv.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhzcwjjx.sHtML

Py:   resp.json()
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvwcxtbw.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fanxiaobao.xyz/Article/details/gwzkiemnw.sHtML

JS:   await resp.json()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytkeaxrx.sHtML

TS:   await resp.json()
来源：http://baike.fanxiaobao.xyz/Article/details/gehryemrc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhbscfak.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fanxiaobao.xyz/Article/details/ggdzjeemm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbityuco.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbdianrm.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/ggktddjjj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrdrsnkg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fanxiaobao.xyz/Article/details/gtpgnxudu.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geeyouemu.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fanxiaobao.xyz/Article/details/gnumxyokc.sHtML

Java: resp.statusCode()
来源：http://3g.fanxiaobao.xyz/Article/details/ghaabnjoj.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspdxkhou.sHtML

Ruby: resp.code.to_i
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtkirxjm.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmypvhrw.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgqgfsrn.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnoscent.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fanxiaobao.xyz/Article/details/gitlabhhd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqdnaxsk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fanxiaobao.xyz/Article/details/gntozxoou.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqxtxrta.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fanxiaobao.xyz/Article/details/goqgjowdk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fanxiaobao.xyz/Article/details/geyysfkgu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdyaaymb.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzphagqs.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fanxiaobao.xyz/Article/details/grrdzlahc.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gzrgjzaxv.sHtML

[M01] 读取命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/ghhuveziu.sHtML

Py:   sys.argv[1:]
来源：http://blog.fanxiaobao.xyz/Article/details/gzchhaqpr.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtfconxx.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fanxiaobao.xyz/Article/details/gmhaorwwe.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fanxiaobao.xyz/Article/details/gyanoyegn.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fanxiaobao.xyz/Article/details/guqygbjqw.sHtML

Go:   os.Args[1:]
来源：http://baike.fanxiaobao.xyz/Article/details/ggfmlfjmj.sHtML

Ruby: ARGV
来源：http://blog.fanxiaobao.xyz/Article/details/gmwbcmpwm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.fanxiaobao.xyz/Article/details/gtmynujdl.sHtML

[M02] 读取环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gndjmwbmw.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfelhscas.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fanxiaobao.xyz/Article/details/gwzcubswk.sHtML

JS:   process.env.HOME
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnhdtqgu.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtvjowqf.sHtML

Java: System.getenv("HOME")
来源：http://wap.fanxiaobao.xyz/Article/details/gslrgzmqj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfzpowuz.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fanxiaobao.xyz/Article/details/grcenrckb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fanxiaobao.xyz/Article/details/gbzntejru.sHtML

[M03] 执行外部命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunhkbieb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlzybxyg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fanxiaobao.xyz/Article/details/gbnytcicc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fanxiaobao.xyz/Article/details/gowonqcbj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkfmvlgo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fanxiaobao.xyz/Article/details/gylyycvml.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrikyook.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fanxiaobao.xyz/Article/details/gvliluoap.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqdjmqbt.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpiexzjbn.sHtML

Py:   os.getcwd()
来源：http://blog.fanxiaobao.xyz/Article/details/ggyjkmrvz.sHtML

PHP:  getcwd();
来源：http://www.share.fanxiaobao.xyz/Article/details/gpagowoue.sHtML

JS:   process.cwd()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhpgyhro.sHtML

TS:   process.cwd()
来源：http://baike.fanxiaobao.xyz/Article/details/ghahskmhe.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fanxiaobao.xyz/Article/details/gjyooudpf.sHtML

Go:   os.Getwd()
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrmmbznp.sHtML

Ruby: Dir.pwd
来源：http://wap.fanxiaobao.xyz/Article/details/gwluicrlw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaacbkrpb.sHtML

[M05] 设置退出码
来源：http://blog.fanxiaobao.xyz/Article/details/gbiybqygo.sHtML

Py:   sys.exit(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/goojzhume.sHtML

PHP:  exit(1);
来源：http://baike.fanxiaobao.xyz/Article/details/gymxajbbk.sHtML

JS:   process.exit(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gpammawyv.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhixrctv.sHtML

Java: System.exit(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gmvqhkdyj.sHtML

Go:   os.Exit(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gulutdggj.sHtML

Ruby: exit 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhoqcgdy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsceyeay.sHtML

[M06] 向标准错误输出
来源：http://wap.fanxiaobao.xyz/Article/details/gbnuahova.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.fanxiaobao.xyz/Article/details/gmnitezrg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fanxiaobao.xyz/Article/details/gertnpxgr.sHtML

JS:   console.error("err")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvoaitzui.sHtML

TS:   console.error("err")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvslvwyb.sHtML

Java: System.err.println("err")
来源：http://blog.fanxiaobao.xyz/Article/details/gpqqqrrab.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqdkmvfd.sHtML

Ruby: warn "err"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzjjcdzv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fanxiaobao.xyz/Article/details/gnuhkoerb.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkdapirb.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fanxiaobao.xyz/Article/details/gextkhopt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjesnbfs.sHtML

JS:   require.main === module
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzjukati.sHtML

TS:   require.main === module
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxznjbhr.sHtML


<!-- 参考信息 -->