代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.fanxiaobao.xyz/Article/details/gqmummypc.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisrxfzdj.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fanxiaobao.xyz/Article/details/gwktczgpg.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqmjacsu.sHtML

[J03] 字符串解析为日期
来源：http://m.share.fanxiaobao.xyz/Article/details/gawahxhlz.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbeycawzl.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvgfvvxf.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbttzkczw.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.fanxiaobao.xyz/Article/details/gniwwenqx.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxibqvjh.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.fanxiaobao.xyz/Article/details/ggstgeimo.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmzzubwi.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopalvqta.sHtML

[J04] 时间戳与日期互转
来源：http://baike.fanxiaobao.xyz/Article/details/ghfzjkrrq.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.fanxiaobao.xyz/Article/details/gowzjmsvi.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.fanxiaobao.xyz/Article/details/gdseamgnf.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.fanxiaobao.xyz/Article/details/gvohdrhss.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcuqcxexb.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdgiyyke.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfepczafd.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.fanxiaobao.xyz/Article/details/gytyedkvf.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvmtsxhq.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjubdsfft.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govwuasgf.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.fanxiaobao.xyz/Article/details/gjibqtfgy.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fanxiaobao.xyz/Article/details/gondcpfuv.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fanxiaobao.xyz/Article/details/gluxuyezq.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmuswetz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjallmqt.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonlqbqtf.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.fanxiaobao.xyz/Article/details/gffylzcpi.sHtML

[J06] 计算两时间之差
来源：http://blog.fanxiaobao.xyz/Article/details/gmnzfeszf.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.fanxiaobao.xyz/Article/details/gwladoqmp.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhvubznh.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.fanxiaobao.xyz/Article/details/guyekbxkk.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbqrmcot.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwlsmwcv.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvykcyds.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.fanxiaobao.xyz/Article/details/ghxblfyzj.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.fanxiaobao.xyz/Article/details/gvpbcacpk.sHtML

[J07] 比较两个日期
来源：http://read.share.fanxiaobao.xyz/Article/details/gddsiwbtm.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.fanxiaobao.xyz/Article/details/gyylchiin.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.fanxiaobao.xyz/Article/details/gyixbwhbm.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.fanxiaobao.xyz/Article/details/gktzvuton.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppblsblj.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gublbptrw.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.fanxiaobao.xyz/Article/details/gctasazse.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.fanxiaobao.xyz/Article/details/gziyuenzi.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglkmvxcg.sHtML

[J08] 提取年月日与星期
来源：http://wap.fanxiaobao.xyz/Article/details/gnzqqwiee.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.fanxiaobao.xyz/Article/details/grszscfcj.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxiwgliv.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.fanxiaobao.xyz/Article/details/gdprkknuc.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.fanxiaobao.xyz/Article/details/goijgvryx.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.fanxiaobao.xyz/Article/details/gzjcsidha.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccivjblr.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.fanxiaobao.xyz/Article/details/ghmzmahtm.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.fanxiaobao.xyz/Article/details/gvaztenzi.sHtML

[J09] 时区处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gmusolvtd.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.fanxiaobao.xyz/Article/details/giuiiqirq.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtaaoxli.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fanxiaobao.xyz/Article/details/gvzqprwqa.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fanxiaobao.xyz/Article/details/gszqozhyb.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.fanxiaobao.xyz/Article/details/grpdxexpw.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpdsaast.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfmpdemb.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.fanxiaobao.xyz/Article/details/gkhsmjhbv.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjeppjidy.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsxysnyh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxqinzxi.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjsfufbk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gytgccbxi.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzevsius.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhurlvvp.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsnnhyto.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtntdprc.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gflzkssti.sHtML

K. JSON 与序列化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxvjikbl.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goewhrrsr.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gwmpaqkct.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.fanxiaobao.xyz/Article/details/gomnmbjda.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrfnmmly.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gundbcsku.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gscivqexh.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.fanxiaobao.xyz/Article/details/gybyigfwx.sHtML

Go:   json.Marshal(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gmgwkoqhr.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdrzcwyb.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjgrwhwq.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqkmfgmw.sHtML

Py:   json.loads(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gmonacuvs.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyuawbqq.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkoekcptl.sHtML

TS:   JSON.parse(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcctyneta.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvchvldmj.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrayrrka.sHtML

Ruby: JSON.parse(s)
来源：http://baike.fanxiaobao.xyz/Article/details/galxfqegr.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gngfuaudl.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztzsnlep.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.fanxiaobao.xyz/Article/details/gudpukwyn.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.fanxiaobao.xyz/Article/details/gkfkavbzl.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbesugsl.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/geiloynuc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/ghcpmeeap.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.fanxiaobao.xyz/Article/details/giqqcrczz.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gbdygrxav.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwwtwdqo.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gkczsxime.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.fanxiaobao.xyz/Article/details/gcbxdwxmu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkcodpyv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gienmvnby.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fanxiaobao.xyz/Article/details/gqxcwzzaw.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.fanxiaobao.xyz/Article/details/gabyupuqx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.fanxiaobao.xyz/Article/details/gryxwpusx.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlgmexot.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.fanxiaobao.xyz/Article/details/geqpnxpbf.sHtML

[K05] 深拷贝对象
来源：http://3g.fanxiaobao.xyz/Article/details/gumodtrne.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gqfoyvjqr.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.fanxiaobao.xyz/Article/details/gkawseaqr.sHtML

JS:   structuredClone(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnksdtzc.sHtML

TS:   structuredClone(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/galoiomwl.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.fanxiaobao.xyz/Article/details/gntwckvdz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.fanxiaobao.xyz/Article/details/gojxgqmmp.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.fanxiaobao.xyz/Article/details/gnojwmwsn.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqxgelzj.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmarzgiz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fanxiaobao.xyz/Article/details/gmbpiqylq.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.fanxiaobao.xyz/Article/details/gahkjrrcg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcgzkqrm.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fanxiaobao.xyz/Article/details/gwpwqauhv.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.fanxiaobao.xyz/Article/details/gyytacele.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkxjlhqb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fanxiaobao.xyz/Article/details/gzdmaiksm.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fanxiaobao.xyz/Article/details/gmyorutrf.sHtML

[K07] 进制转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjucawbzx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.fanxiaobao.xyz/Article/details/gcybsdnoo.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.fanxiaobao.xyz/Article/details/gixetwkqs.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbkilxce.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcyzsamy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fanxiaobao.xyz/Article/details/gallbsddq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjugzlzzk.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glphosmrj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fanxiaobao.xyz/Article/details/gpezzntvv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.fanxiaobao.xyz/Article/details/gartcpuoh.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/glinzzrru.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gplrkkowb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.fanxiaobao.xyz/Article/details/gbqvgroyx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdavwezoo.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.fanxiaobao.xyz/Article/details/giubasiyz.sHtML

Go:   encoding/gob
来源：http://www.share.fanxiaobao.xyz/Article/details/gjolvaudg.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdlmubbx.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.fanxiaobao.xyz/Article/details/ggeutvuqt.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwtactjp.sHtML

L. 网络请求
来源：http://mobile.fanxiaobao.xyz/Article/details/grwqepbje.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gglsbkoai.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhfoxcng.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmjmhrlr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.fanxiaobao.xyz/Article/details/gciwvkxjx.sHtML

JS:   await fetch(url)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzyovsnnc.sHtML

TS:   await fetch(url)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbshaprid.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrrujytv.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxndfadd.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.fanxiaobao.xyz/Article/details/gtxuwcrod.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsdredyf.sHtML

[L02] 发送 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gsispttyy.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fanxiaobao.xyz/Article/details/gzckxlows.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.fanxiaobao.xyz/Article/details/gqwnjmyxs.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmcwkzux.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fanxiaobao.xyz/Article/details/gqitvygjy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnwmkahi.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqgyymzw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fanxiaobao.xyz/Article/details/gnyhlqhgl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.fanxiaobao.xyz/Article/details/gvasmdjeb.sHtML

[L03] 设置自定义请求头
来源：http://baike.fanxiaobao.xyz/Article/details/glgldgqep.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.fanxiaobao.xyz/Article/details/guuxqiqjp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gppsotgks.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkceepljn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsyjenuo.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fanxiaobao.xyz/Article/details/gcgzkchbu.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.fanxiaobao.xyz/Article/details/ggrmzentv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjkexkjx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.fanxiaobao.xyz/Article/details/gxmkabhch.sHtML

[L04] 设置超时
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwhidult.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fanxiaobao.xyz/Article/details/giroavqdw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkyzgtlit.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fanxiaobao.xyz/Article/details/geefxfifv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncuplpbu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrifcbqq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fanxiaobao.xyz/Article/details/ghnlckzyo.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fanxiaobao.xyz/Article/details/gcqcnprym.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gsxbiocuj.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fanxiaobao.xyz/Article/details/gaknpcaqu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.fanxiaobao.xyz/Article/details/gyaxrjuqw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fanxiaobao.xyz/Article/details/gxuunmyvi.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpizyxzgo.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fanxiaobao.xyz/Article/details/glxwzvoni.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fanxiaobao.xyz/Article/details/gjbxzxpyj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjugopnpw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgwbgrye.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbqncqku.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gytcoukqn.sHtML

Py:   resp.json()
来源：http://baike.fanxiaobao.xyz/Article/details/gwdneyosb.sHtML

PHP:  json_decode($body, true);
来源：http://blog.fanxiaobao.xyz/Article/details/gjsulfxfb.sHtML

JS:   await resp.json()
来源：http://baike.fanxiaobao.xyz/Article/details/gpyeetxuz.sHtML

TS:   await resp.json()
来源：http://wap.fanxiaobao.xyz/Article/details/ghwailsvh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fanxiaobao.xyz/Article/details/gecutansn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fanxiaobao.xyz/Article/details/gubqzovaq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkiutnajg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fanxiaobao.xyz/Article/details/gtvsxwhiq.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxajougu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwuyjqno.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fanxiaobao.xyz/Article/details/gptikxmcn.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fanxiaobao.xyz/Article/details/gjptjdwnz.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fanxiaobao.xyz/Article/details/gsrrobjfv.sHtML

Java: resp.statusCode()
来源：http://3g.fanxiaobao.xyz/Article/details/grvnbjzvf.sHtML

Go:   resp.StatusCode
来源：http://read.share.fanxiaobao.xyz/Article/details/ghoiyoxnh.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fanxiaobao.xyz/Article/details/gfywmndyd.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fanxiaobao.xyz/Article/details/gtfwkdxkt.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgxktggu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fanxiaobao.xyz/Article/details/gotngwuwk.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fanxiaobao.xyz/Article/details/ggjfcrwif.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcyarlun.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fanxiaobao.xyz/Article/details/gruonfonb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fanxiaobao.xyz/Article/details/galqldaiy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvzmilni.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadztrozc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdtqhzwb.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ghaqmohai.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gmilphhgp.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gudmztzto.sHtML

[M01] 读取命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/guudnaccm.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflzpagux.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fanxiaobao.xyz/Article/details/gxidxegxh.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gezzltboz.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fanxiaobao.xyz/Article/details/gegjnwxju.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrsbwevo.sHtML

Go:   os.Args[1:]
来源：http://3g.fanxiaobao.xyz/Article/details/gjncilxsc.sHtML

Ruby: ARGV
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixyypbdy.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fanxiaobao.xyz/Article/details/gwwhvjwec.sHtML

[M02] 读取环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgenhvga.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fanxiaobao.xyz/Article/details/glolhwdgf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfmksgxn.sHtML

JS:   process.env.HOME
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpyyafqs.sHtML

TS:   process.env.HOME
来源：http://baike.fanxiaobao.xyz/Article/details/gpuayjooc.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbaoxypte.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fanxiaobao.xyz/Article/details/gzqxoojip.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fanxiaobao.xyz/Article/details/glcoimfnz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzidityw.sHtML

[M03] 执行外部命令
来源：http://baike.fanxiaobao.xyz/Article/details/gxtjslxwl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gpveddnsu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxelsmzno.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fanxiaobao.xyz/Article/details/gazqafbvv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fanxiaobao.xyz/Article/details/gveideyro.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fanxiaobao.xyz/Article/details/gwjsbqxzs.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fanxiaobao.xyz/Article/details/gojzumvuo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fanxiaobao.xyz/Article/details/gupbkbfox.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fanxiaobao.xyz/Article/details/gjtxygnik.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fanxiaobao.xyz/Article/details/gbztkjmoa.sHtML

Py:   os.getcwd()
来源：http://m.share.fanxiaobao.xyz/Article/details/gxoorsuct.sHtML

PHP:  getcwd();
来源：http://baike.fanxiaobao.xyz/Article/details/grslldobe.sHtML

JS:   process.cwd()
来源：http://3g.fanxiaobao.xyz/Article/details/gljbogukn.sHtML

TS:   process.cwd()
来源：http://baike.fanxiaobao.xyz/Article/details/gdsnupixv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fanxiaobao.xyz/Article/details/gkrovpobg.sHtML

Go:   os.Getwd()
来源：http://m.share.fanxiaobao.xyz/Article/details/gooqrbqcw.sHtML

Ruby: Dir.pwd
来源：http://read.share.fanxiaobao.xyz/Article/details/ggennfwpx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fanxiaobao.xyz/Article/details/gjmjdnanr.sHtML

[M05] 设置退出码
来源：http://wap.fanxiaobao.xyz/Article/details/gvmveipiz.sHtML

Py:   sys.exit(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gqlifbypy.sHtML

PHP:  exit(1);
来源：http://3g.fanxiaobao.xyz/Article/details/gzylkyuic.sHtML

JS:   process.exit(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpucpzsdf.sHtML

TS:   process.exit(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gcqpikffn.sHtML

Java: System.exit(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gllkspndd.sHtML

Go:   os.Exit(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gleurupvm.sHtML

Ruby: exit 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzfiopki.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvbontml.sHtML

[M06] 向标准错误输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gblmbzwbx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzrwdirz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunoecafm.sHtML

JS:   console.error("err")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgeojjpa.sHtML

TS:   console.error("err")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsrdkipe.sHtML

Java: System.err.println("err")
来源：http://wap.fanxiaobao.xyz/Article/details/gkbtvvzqp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxxlsaum.sHtML

Ruby: warn "err"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvhltvtn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fanxiaobao.xyz/Article/details/grrgurxsw.sHtML

[M07] 判断是否为主入口
来源：http://blog.fanxiaobao.xyz/Article/details/gnruehoao.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fanxiaobao.xyz/Article/details/gulyagnoy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwgrqhvc.sHtML

JS:   require.main === module
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpayewnm.sHtML

TS:   require.main === module
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnfdgmwg.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzmutbxw.sHtML

Go:   func main()
来源：http://www.share.fanxiaobao.xyz/Article/details/gvyhvpeqp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fanxiaobao.xyz/Article/details/gdyyiqdbp.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvgxgpep.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fanxiaobao.xyz/Article/details/gwmynwbec.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqknkidm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fanxiaobao.xyz/Article/details/gssycezdi.sHtML

JS:   process.platform;  process.version
来源：http://baike.fanxiaobao.xyz/Article/details/gzguxagqn.sHtML

TS:   process.platform;  process.version
来源：http://3g.fanxiaobao.xyz/Article/details/glchclpuf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fanxiaobao.xyz/Article/details/ghzzwryof.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fanxiaobao.xyz/Article/details/geroqfuyr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzqvyvwj.sHtML


<!-- 参考信息 -->