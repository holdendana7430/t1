代发 wailian999

Go:   time.Now()
来源：http://read.share.zdbjq.cn/Article/details/gnhruiflt.sHtML

Ruby: Time.now
来源：http://www.m.share.fehbvm.com/Article/details/gvkxmztuc.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.zdbjq.cn/Article/details/gueacivjt.sHtML

[J02] 格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/gaarzfjrn.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.hesvh.cn/Article/details/gyofdwuph.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.fehbvm.com/Article/details/gfbrcwglb.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.zdbjq.cn/Article/details/gpgeodsrw.sHtML

TS:   d.toISOString()
来源：http://m.share.zdbjq.cn/Article/details/guuhwkkbz.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.hesvh.cn/Article/details/gehvgoglb.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.hesvh.cn/Article/details/glkckxygh.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.zdbjq.cn/Article/details/gvduzoucr.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.fehbvm.com/Article/details/gfpkwvnfi.sHtML

[J03] 字符串解析为日期
来源：http://read.share.zdbjq.cn/Article/details/gjkhqbgin.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.zdbjq.cn/Article/details/gbeacwrqr.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.zdbjq.cn/Article/details/giofdajjz.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gaitwlxuh.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gyagbzlmj.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gfuxpjqdc.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gtzevpzcn.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/grchaisyw.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.fehbvm.com/Article/details/gwbkqavaz.sHtML

[J04] 时间戳与日期互转
来源：http://baike.hesvh.cn/Article/details/gajmivzlr.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.hesvh.cn/Article/details/gqdxlyswa.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.hesvh.cn/Article/details/gqrspyuoj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.zdbjq.cn/Article/details/gfvbphpfh.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.fehbvm.com/Article/details/glpsqrscy.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gmfufhtci.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.zdbjq.cn/Article/details/gxsfbvtmt.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.fehbvm.com/Article/details/gexxkatwk.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.zdbjq.cn/Article/details/gmzrqersi.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.hesvh.cn/Article/details/gpvopdkna.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.fehbvm.com/Article/details/gvpbpomym.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.hesvh.cn/Article/details/gebadmdtb.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fehbvm.com/Article/details/gcjhvzlmd.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.hesvh.cn/Article/details/glqnismic.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.fehbvm.com/Article/details/gyailskkd.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.hesvh.cn/Article/details/gqngcgdiz.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.fehbvm.com/Article/details/gsxozfksx.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.zdbjq.cn/Article/details/gvagmguet.sHtML

[J06] 计算两时间之差
来源：http://blog.fehbvm.com/Article/details/gpaemieof.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.fehbvm.com/Article/details/gsqffntnb.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.fehbvm.com/Article/details/ggrqrhqao.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.hesvh.cn/Article/details/gyrlrsbyk.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.fehbvm.com/Article/details/gvxtqmebk.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.hesvh.cn/Article/details/gftglmcms.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.fehbvm.com/Article/details/gnxyiyssq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.zdbjq.cn/Article/details/gbravjlhn.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.zdbjq.cn/Article/details/gcnagsxcz.sHtML

[J07] 比较两个日期
来源：http://3g.zdbjq.cn/Article/details/goldlhvwn.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/gmvtskoho.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.zdbjq.cn/Article/details/ghfwqcgzc.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.zdbjq.cn/Article/details/gbrlkpecv.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.hesvh.cn/Article/details/gqdrjedht.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.zdbjq.cn/Article/details/geemmakon.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.hesvh.cn/Article/details/gzbtphstv.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.hesvh.cn/Article/details/grmtktbox.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.hesvh.cn/Article/details/gfxiszdkp.sHtML

[J08] 提取年月日与星期
来源：http://wap.hesvh.cn/Article/details/grpbgvmtv.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.hesvh.cn/Article/details/gvloumbon.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.zdbjq.cn/Article/details/gontqskvn.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.zdbjq.cn/Article/details/gokaymmjz.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.zdbjq.cn/Article/details/gbewceitp.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.hesvh.cn/Article/details/gbmyddeil.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.hesvh.cn/Article/details/gccycdgcu.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.fehbvm.com/Article/details/gellbtzak.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.fehbvm.com/Article/details/ggvsnumwj.sHtML

[J09] 时区处理
来源：http://www.share.fehbvm.com/Article/details/ggyapreux.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.zdbjq.cn/Article/details/grgkdgyre.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.fehbvm.com/Article/details/gwycblaym.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.hesvh.cn/Article/details/ghituiuhf.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.zdbjq.cn/Article/details/gnfmettsa.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.fehbvm.com/Article/details/gjptcpkjc.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.fehbvm.com/Article/details/gkmboxurg.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.zdbjq.cn/Article/details/gubzsencz.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.hesvh.cn/Article/details/gmdoehlpw.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.zdbjq.cn/Article/details/gtjqskqem.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.hesvh.cn/Article/details/ghuqaxqik.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.fehbvm.com/Article/details/gzjrncrzd.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.hesvh.cn/Article/details/gpfpkqcwy.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.hesvh.cn/Article/details/gqfnmhrjr.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.zdbjq.cn/Article/details/gunuqgukw.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.zdbjq.cn/Article/details/ghniuiafr.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.hesvh.cn/Article/details/gbwamlfgc.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.hesvh.cn/Article/details/guhqzjjnh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gikusqnyr.sHtML

K. JSON 与序列化
来源：http://m.share.zdbjq.cn/Article/details/gumgystse.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbsbvraza.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.fehbvm.com/Article/details/giyspihoh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.zdbjq.cn/Article/details/gnjbmniet.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.hesvh.cn/Article/details/gjldnpxix.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.zdbjq.cn/Article/details/gtdidpmra.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.hesvh.cn/Article/details/gagjwptzy.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.zdbjq.cn/Article/details/gumvwluge.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.fehbvm.com/Article/details/gmhlhyhzp.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.hesvh.cn/Article/details/gyxbuuzdf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.zdbjq.cn/Article/details/gywutccvo.sHtML

[K02] JSON 字符串转对象
来源：http://blog.hesvh.cn/Article/details/gdgfffhre.sHtML

Py:   json.loads(s)
来源：http://3g.fehbvm.com/Article/details/gmzrfxhjf.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.zdbjq.cn/Article/details/groudruae.sHtML

JS:   JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/guqgbsknk.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/girwhhmar.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.zdbjq.cn/Article/details/grbrdhlik.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.hesvh.cn/Article/details/gvnwxnzum.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/grtomyoex.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.zdbjq.cn/Article/details/gdvruxxpl.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.fehbvm.com/Article/details/gmbwkwzez.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.zdbjq.cn/Article/details/gbsllxtqp.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.hesvh.cn/Article/details/gpzanfvsj.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.fehbvm.com/Article/details/gzyyfdoqw.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.hesvh.cn/Article/details/glviuvzez.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.zdbjq.cn/Article/details/gpadswdpj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.zdbjq.cn/Article/details/gjjngousw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.hesvh.cn/Article/details/gqpnxkrdy.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.zdbjq.cn/Article/details/guyerjvwh.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.hesvh.cn/Article/details/gysdcseqz.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.zdbjq.cn/Article/details/gcdeshroh.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.fehbvm.com/Article/details/gadbpgnmr.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.zdbjq.cn/Article/details/gwaonclaz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.hesvh.cn/Article/details/gapiukvtc.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.hesvh.cn/Article/details/gwmyszwxx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/gbdgyocwv.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.fehbvm.com/Article/details/ghsbakqbs.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.hesvh.cn/Article/details/gauuxigup.sHtML

[K05] 深拷贝对象
来源：http://wap.hesvh.cn/Article/details/gobrhvigu.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.hesvh.cn/Article/details/gokacbtqt.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.fehbvm.com/Article/details/gcbqhossl.sHtML

JS:   structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gaghlgrkk.sHtML

TS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gtucwewis.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.zdbjq.cn/Article/details/gcxxiayjz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.zdbjq.cn/Article/details/gjqzdilwa.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.fehbvm.com/Article/details/ghdukvmvl.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.hesvh.cn/Article/details/gnpwngxvz.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.fehbvm.com/Article/details/grksseazd.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/gnaxfjehe.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.zdbjq.cn/Article/details/gelaeojkl.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/glstxymym.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/gborzntue.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.zdbjq.cn/Article/details/giuofiejj.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/goqijwtqf.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gqbswwxir.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gvjbusbyl.sHtML

[K07] 进制转换
来源：http://read.share.fehbvm.com/Article/details/gcpoqflmf.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/ggvvhpcds.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.zdbjq.cn/Article/details/gzreyueqx.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/ggjmdablw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gxwnzojap.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gaqxzpavx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.hesvh.cn/Article/details/grycgnjtq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.hesvh.cn/Article/details/gvvcvbxec.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/ghobkkjwj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.hesvh.cn/Article/details/gfywlqszb.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.fehbvm.com/Article/details/grkwbqrow.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.hesvh.cn/Article/details/gymuvlizt.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/ghsxslqkp.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/guiwypxwu.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.zdbjq.cn/Article/details/gfcmcakpa.sHtML

Go:   encoding/gob
来源：http://3g.zdbjq.cn/Article/details/gblvtqiuh.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.zdbjq.cn/Article/details/gpymwkdxb.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gcerosvde.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gskcpsjhk.sHtML

L. 网络请求
来源：http://mobile.fehbvm.com/Article/details/gknetqtie.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpjubfwir.sHtML

[L01] 发送 GET 请求
来源：http://www.share.fehbvm.com/Article/details/gncpmjnen.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fehbvm.com/Article/details/gwugvjmyj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fehbvm.com/Article/details/gfpdbfrnv.sHtML

JS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/gyetwkvfp.sHtML

TS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gyokiywqi.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.hesvh.cn/Article/details/gmfqhsinp.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.hesvh.cn/Article/details/goaglhzql.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fehbvm.com/Article/details/gzsccbsco.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.hesvh.cn/Article/details/ginuiowph.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gpczwvkph.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.hesvh.cn/Article/details/gejcypuin.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.hesvh.cn/Article/details/gxgohoybf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/ganrgmapi.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gvbuxywmc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fehbvm.com/Article/details/glziywtht.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.fehbvm.com/Article/details/gxxfggjsb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.hesvh.cn/Article/details/glmcitwdg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.zdbjq.cn/Article/details/gmlinsxpp.sHtML

[L03] 设置自定义请求头
来源：http://wap.zdbjq.cn/Article/details/gqlyayoeb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.zdbjq.cn/Article/details/gtlcddemi.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.zdbjq.cn/Article/details/gvjlwqavx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/gfoqbfdmi.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gtlcxmwcw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.hesvh.cn/Article/details/gibedaukn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gctptaocc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.zdbjq.cn/Article/details/gpjzvqevj.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/getllzqte.sHtML

[L04] 设置超时
来源：http://3g.zdbjq.cn/Article/details/ghrtbxyhy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.zdbjq.cn/Article/details/gojwalfig.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gxflxfpsu.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/grpfdafdd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/ghrfhtvft.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.hesvh.cn/Article/details/govmfpioo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fehbvm.com/Article/details/gpfpxgffh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.hesvh.cn/Article/details/gpbkwexxf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.zdbjq.cn/Article/details/glmsusagy.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.hesvh.cn/Article/details/griaflgje.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.hesvh.cn/Article/details/gqmjfnabl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.zdbjq.cn/Article/details/gcffxgwqj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gysardbjz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/gqaakmetd.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.hesvh.cn/Article/details/gvzradghj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.zdbjq.cn/Article/details/gbpryvvix.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.hesvh.cn/Article/details/glmcieffx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gwpoviann.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fehbvm.com/Article/details/glwzponam.sHtML

Py:   resp.json()
来源：http://wap.hesvh.cn/Article/details/gjoliihrk.sHtML

PHP:  json_decode($body, true);
来源：http://3g.zdbjq.cn/Article/details/gzfrcbllw.sHtML

JS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/ggrtbeikp.sHtML

TS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/ghlpotyvk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gpuinugcs.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.hesvh.cn/Article/details/gtanmzdju.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fehbvm.com/Article/details/glmpkzrav.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fehbvm.com/Article/details/ghieolpyj.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/ggkrnjngt.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.zdbjq.cn/Article/details/gthbznrdz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.hesvh.cn/Article/details/ghyyjioio.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/giichzadk.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/ggljzchec.sHtML

Java: resp.statusCode()
来源：http://www.blog.hesvh.cn/Article/details/gvxniwamc.sHtML

Go:   resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gilnavcsm.sHtML

Ruby: resp.code.to_i
来源：http://baike.hesvh.cn/Article/details/gwmhsgbrb.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gwaxvmnln.sHtML

[L08] 并发请求多个地址
来源：http://wap.zdbjq.cn/Article/details/gadkerhql.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.hesvh.cn/Article/details/gnguluhtn.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.zdbjq.cn/Article/details/gekjjfqrw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gfopcexgn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gewymnwwc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.hesvh.cn/Article/details/ghaluzxqo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.hesvh.cn/Article/details/gbqgpkxgi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/gmmsgiypk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.fehbvm.com/Article/details/glvqwvlnz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/goxzwbntq.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.hesvh.cn/Article/details/gvvyvrfit.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqddvpldd.sHtML

[M01] 读取命令行参数
来源：http://mobile.fehbvm.com/Article/details/gbhklhtqj.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fehbvm.com/Article/details/gujigthfj.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fehbvm.com/Article/details/gugiahxqb.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gfbdlhtno.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gfszxatvm.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gufqgscpb.sHtML

Go:   os.Args[1:]
来源：http://3g.zdbjq.cn/Article/details/gmpsotono.sHtML

Ruby: ARGV
来源：http://m.share.zdbjq.cn/Article/details/gyvhhdhmb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.hesvh.cn/Article/details/ghggooixn.sHtML

[M02] 读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gzcpzrpcb.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.hesvh.cn/Article/details/gffxaflsb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gwntqbnml.sHtML

JS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/giolwgtld.sHtML

TS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/giescbbel.sHtML

Java: System.getenv("HOME")
来源：http://3g.hesvh.cn/Article/details/gjjjambtk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fehbvm.com/Article/details/ggqjsipob.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.zdbjq.cn/Article/details/gxzgswbkg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fehbvm.com/Article/details/gqgvujhzh.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/ggwxaovdv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.hesvh.cn/Article/details/gcngcvyrh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fehbvm.com/Article/details/gfxitcfew.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/guemqoalo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gkqhsspps.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.hesvh.cn/Article/details/gieyibfzl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fehbvm.com/Article/details/gnucrcvgx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/glexfwqnr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.hesvh.cn/Article/details/gslgqzboa.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/ggxxsvijv.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/giylhkanv.sHtML

PHP:  getcwd();
来源：http://read.share.zdbjq.cn/Article/details/gusirwpja.sHtML

JS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gynivxgba.sHtML

TS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gjdrbwqgv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fehbvm.com/Article/details/gfhafrzed.sHtML

Go:   os.Getwd()
来源：http://www.share.hesvh.cn/Article/details/gnsgibubf.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/gkahvwdsl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.hesvh.cn/Article/details/gbnolihuj.sHtML

[M05] 设置退出码
来源：http://www.m.share.zdbjq.cn/Article/details/gjpgjtsnf.sHtML

Py:   sys.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gqqzpebam.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gxbzrvjlo.sHtML

JS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gkpfiychp.sHtML

TS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gzdqwxqar.sHtML

Java: System.exit(1)
来源：http://blog.fehbvm.com/Article/details/gdkfrfiwy.sHtML

Go:   os.Exit(1)
来源：http://read.share.fehbvm.com/Article/details/gbqzcjeph.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/gfsquqdil.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.hesvh.cn/Article/details/grahmophm.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/gmljuikxh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gtwallgyh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/gjtidjcgo.sHtML

JS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gxaqnsorb.sHtML

TS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gwgorguva.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/gkjxgqije.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/gdzpoxpuf.sHtML

Ruby: warn "err"
来源：http://www.m.share.fehbvm.com/Article/details/gjzfwywle.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.hesvh.cn/Article/details/ghlxvfifk.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/gdxbibdtx.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.zdbjq.cn/Article/details/guypyzofl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.zdbjq.cn/Article/details/gwfdsilur.sHtML

JS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gqguuqczp.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/grrpcsgny.sHtML

Java: public static void main(String[] args)
来源：http://wap.hesvh.cn/Article/details/gdxmdmrkz.sHtML

Go:   func main()
来源：http://www.m.share.hesvh.cn/Article/details/gwzyaeqqw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gnmriakrh.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/gckmcjuel.sHtML


<!-- 参考信息 -->