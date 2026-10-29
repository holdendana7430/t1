代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.hesvh.cn/Article/details/gwxtcawir.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.hesvh.cn/Article/details/gtppyyfmo.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.hesvh.cn/Article/details/gyaketyyc.sHtML

TS:   d.toISOString()
来源：http://baike.hesvh.cn/Article/details/gizcvffgj.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.hesvh.cn/Article/details/gpebljngn.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.fehbvm.com/Article/details/gdyemiomn.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.zdbjq.cn/Article/details/gkrejjpkk.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.fehbvm.com/Article/details/gfrvlyxmz.sHtML

[J03] 字符串解析为日期
来源：http://3g.zdbjq.cn/Article/details/gompiukno.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.fehbvm.com/Article/details/gpnavwjsd.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.zdbjq.cn/Article/details/gmisxxvjd.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gjyheofcy.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gcbqnsagu.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gmxcqjstd.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gkzplsray.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gkxpjdekz.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.fehbvm.com/Article/details/gmnlhzraf.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.fehbvm.com/Article/details/gesczneux.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.fehbvm.com/Article/details/gdkeyzbxu.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.zdbjq.cn/Article/details/gqorcdovy.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.hesvh.cn/Article/details/gotyzphvu.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.fehbvm.com/Article/details/gwllejmnc.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.hesvh.cn/Article/details/gvogsontw.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.hesvh.cn/Article/details/gclblhjpl.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.fehbvm.com/Article/details/gimhudqza.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gockuikpm.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.fehbvm.com/Article/details/gdcuzputm.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.fehbvm.com/Article/details/gzfgqsjva.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.hesvh.cn/Article/details/gaucsznvz.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fehbvm.com/Article/details/gxwmwlvqe.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fehbvm.com/Article/details/gaazrvnri.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.zdbjq.cn/Article/details/ghpfsgkvq.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.fehbvm.com/Article/details/gdzlfchov.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.fehbvm.com/Article/details/gnirfneqh.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.hesvh.cn/Article/details/gznkgcimd.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.hesvh.cn/Article/details/gldolchwa.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.hesvh.cn/Article/details/gtemclwyw.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.hesvh.cn/Article/details/gjrnalocp.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.zdbjq.cn/Article/details/gmddtbosx.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.zdbjq.cn/Article/details/gvohqxvew.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.fehbvm.com/Article/details/gjjrrcnhy.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.hesvh.cn/Article/details/gwwhdajvn.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.zdbjq.cn/Article/details/gewvvcfvc.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.hesvh.cn/Article/details/gwkeqnwzp.sHtML

[J07] 比较两个日期
来源：http://blog.zdbjq.cn/Article/details/gxbjhhjfd.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/gusmrnwuv.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.hesvh.cn/Article/details/gkmzvpyra.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.fehbvm.com/Article/details/gzoqqhkqd.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.hesvh.cn/Article/details/ghkgkxxgl.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.hesvh.cn/Article/details/giaczglpe.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.hesvh.cn/Article/details/glzqlswlw.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.hesvh.cn/Article/details/geuqhwlks.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.fehbvm.com/Article/details/ggnqzjplb.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.hesvh.cn/Article/details/gqeguprkt.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.zdbjq.cn/Article/details/gwuznzhpr.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.zdbjq.cn/Article/details/gjonuzknz.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.hesvh.cn/Article/details/gypzhkfnj.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.zdbjq.cn/Article/details/grxybqjct.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.zdbjq.cn/Article/details/galrctgca.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.zdbjq.cn/Article/details/gtqjozioq.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.fehbvm.com/Article/details/gikzssyib.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.zdbjq.cn/Article/details/gpwplpzpf.sHtML

[J09] 时区处理
来源：http://wap.zdbjq.cn/Article/details/gkehpdzlz.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.hesvh.cn/Article/details/gchmjatuu.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.fehbvm.com/Article/details/gzjxstbyg.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.hesvh.cn/Article/details/glmqvkxli.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.zdbjq.cn/Article/details/grobzkfma.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.zdbjq.cn/Article/details/gjgnnkyfy.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.fehbvm.com/Article/details/gxqycsjmi.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.hesvh.cn/Article/details/ggwdbowya.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.zdbjq.cn/Article/details/gjsvsvswt.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.zdbjq.cn/Article/details/gjqbpxamv.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.fehbvm.com/Article/details/gtzmasden.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.hesvh.cn/Article/details/gudsmkwsy.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.hesvh.cn/Article/details/gttxntqfy.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.zdbjq.cn/Article/details/gsknwuodp.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.zdbjq.cn/Article/details/gwzlxnmyq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.fehbvm.com/Article/details/gtbellngx.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.zdbjq.cn/Article/details/gqmocrvsk.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.zdbjq.cn/Article/details/goivrchxr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbywxfmyh.sHtML

K. JSON 与序列化
来源：http://www.m.share.zdbjq.cn/Article/details/gyofsdoln.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxcyojvaz.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.zdbjq.cn/Article/details/grgpzxgxb.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.fehbvm.com/Article/details/gfyzphbfc.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.hesvh.cn/Article/details/gwsxvnfhd.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.hesvh.cn/Article/details/gxjyinafc.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.hesvh.cn/Article/details/gxieqogau.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.fehbvm.com/Article/details/gfocqofay.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.fehbvm.com/Article/details/gjtorllhz.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.fehbvm.com/Article/details/gsfwnblaj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.zdbjq.cn/Article/details/gtoktbxto.sHtML

[K02] JSON 字符串转对象
来源：http://blog.hesvh.cn/Article/details/gcmtwzwrw.sHtML

Py:   json.loads(s)
来源：http://baike.fehbvm.com/Article/details/gebboixgb.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.fehbvm.com/Article/details/ggxgbsgoc.sHtML

JS:   JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/gabmrqswd.sHtML

TS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gjwxfpxxr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.fehbvm.com/Article/details/ghgriprbr.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/gckodtqft.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/gugpzrrkf.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.fehbvm.com/Article/details/golujbcrt.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.fehbvm.com/Article/details/gnenvsvtj.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.zdbjq.cn/Article/details/ghpmukjhp.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.hesvh.cn/Article/details/gasrexdow.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.hesvh.cn/Article/details/gatltddph.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.zdbjq.cn/Article/details/gfvweabsk.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.fehbvm.com/Article/details/gowuqvguf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.zdbjq.cn/Article/details/gulfmirnn.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fehbvm.com/Article/details/gftawlafj.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.zdbjq.cn/Article/details/gxazjibre.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.fehbvm.com/Article/details/glryxtjjc.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.zdbjq.cn/Article/details/gszepvvdi.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.fehbvm.com/Article/details/gvafvlqcw.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.hesvh.cn/Article/details/gjaenbaan.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/ghqptpwaa.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.hesvh.cn/Article/details/guzfefwet.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.zdbjq.cn/Article/details/gatxkpcyf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.hesvh.cn/Article/details/gicbtwkec.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.fehbvm.com/Article/details/giprrjcti.sHtML

[K05] 深拷贝对象
来源：http://wap.fehbvm.com/Article/details/gcovfvvew.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.fehbvm.com/Article/details/gkzkbbvro.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.fehbvm.com/Article/details/ghzvjlasp.sHtML

JS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/geotgecqq.sHtML

TS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gwqdnwrsr.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.fehbvm.com/Article/details/gbtorkfgi.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.hesvh.cn/Article/details/glznzndle.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.zdbjq.cn/Article/details/ggaekmcpy.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.zdbjq.cn/Article/details/gqekvytbi.sHtML

[K06] 解析 URL 查询串
来源：http://3g.fehbvm.com/Article/details/gqglvmdsg.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.fehbvm.com/Article/details/gebxqwytr.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.fehbvm.com/Article/details/gqvwhidel.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/geegmuojt.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gipdpmqrr.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.hesvh.cn/Article/details/geuiamqzr.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gtabovilz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gbavozfek.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gcjbjptec.sHtML

[K07] 进制转换
来源：http://blog.hesvh.cn/Article/details/gmhicstgf.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gvqzktjvt.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.hesvh.cn/Article/details/gathgzofq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gnjdhvejy.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gnppsofvz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/ghepgninu.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.hesvh.cn/Article/details/gfrtusgyd.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.fehbvm.com/Article/details/gtbquopbh.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gyvmzogsh.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.hesvh.cn/Article/details/gcmapdsrw.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.hesvh.cn/Article/details/gwdjkrnyu.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.fehbvm.com/Article/details/gvlitdusa.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/gvtjxaxdi.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/gybksziqm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.fehbvm.com/Article/details/gxuvbypqp.sHtML

Go:   encoding/gob
来源：http://blog.zdbjq.cn/Article/details/glurvpepm.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.fehbvm.com/Article/details/gsrkssvag.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gpxqecdfz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gytkkizwz.sHtML

L. 网络请求
来源：http://mobile.hesvh.cn/Article/details/gcynkfqig.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmandhlki.sHtML

[L01] 发送 GET 请求
来源：http://mobile.hesvh.cn/Article/details/grzqxlnam.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.zdbjq.cn/Article/details/gjihvjoha.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.zdbjq.cn/Article/details/gwixdhntc.sHtML

JS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/gsxrpwjzi.sHtML

TS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/ggifmpoyq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.zdbjq.cn/Article/details/gkaomexcc.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.zdbjq.cn/Article/details/grmanrbqn.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.zdbjq.cn/Article/details/gzrpjpzln.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.hesvh.cn/Article/details/gewnmwkoi.sHtML

[L02] 发送 POST JSON
来源：http://blog.fehbvm.com/Article/details/gkzusdhbw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gfzrojzwu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.fehbvm.com/Article/details/gvgrpoqke.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gguwrrrwo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gqbfaoqcq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.zdbjq.cn/Article/details/gpktkqizs.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.hesvh.cn/Article/details/glojyleil.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fehbvm.com/Article/details/gpquoazrz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.hesvh.cn/Article/details/gltbilxok.sHtML

[L03] 设置自定义请求头
来源：http://baike.hesvh.cn/Article/details/gktnvoinj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fehbvm.com/Article/details/gucnrvpqc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.hesvh.cn/Article/details/gowpjkshm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/gtphhfghy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gbupfjtll.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fehbvm.com/Article/details/gjsrmytsi.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/gfzhyyzke.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fehbvm.com/Article/details/gybbrjxlc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gnpmmctbr.sHtML

[L04] 设置超时
来源：http://m.share.zdbjq.cn/Article/details/gyplvwsau.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.zdbjq.cn/Article/details/gwroqzxul.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.zdbjq.cn/Article/details/gaslvpucy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gatqyosut.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gfjykbjli.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fehbvm.com/Article/details/ggkdizosd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.hesvh.cn/Article/details/gnptvfyjz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fehbvm.com/Article/details/grvsfiicq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fehbvm.com/Article/details/gmisadyll.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.fehbvm.com/Article/details/guqmckwwi.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.hesvh.cn/Article/details/gzsurzilu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fehbvm.com/Article/details/ghsrdvpcu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/gmfopdzzc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/ghvatsevn.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fehbvm.com/Article/details/gmkloeabk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.zdbjq.cn/Article/details/gzrjxnpuz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fehbvm.com/Article/details/gnxrstoby.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.hesvh.cn/Article/details/gkwzjvtwf.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.hesvh.cn/Article/details/ggvhdslbz.sHtML

Py:   resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gvbqxxreu.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gzanhltas.sHtML

JS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gxiudfzpn.sHtML

TS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gdgipjopx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gigrsfpyi.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.zdbjq.cn/Article/details/gkjqfgcfq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.zdbjq.cn/Article/details/grebnvyom.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fehbvm.com/Article/details/ghrlxfwib.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/ghsfmngys.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fehbvm.com/Article/details/ghgbvpjgi.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.zdbjq.cn/Article/details/ggxcqcvqo.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/grukglslo.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/gicnzqiep.sHtML

Java: resp.statusCode()
来源：http://read.share.zdbjq.cn/Article/details/gcggpglsr.sHtML

Go:   resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gdbrkwnzl.sHtML

Ruby: resp.code.to_i
来源：http://www.share.zdbjq.cn/Article/details/gbvbhkble.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gisqyvfvx.sHtML

[L08] 并发请求多个地址
来源：http://mobile.fehbvm.com/Article/details/gwyruyzpu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fehbvm.com/Article/details/gwdivijnx.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.hesvh.cn/Article/details/gayqkzhou.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/ghnkrxiam.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gjkdmnoag.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.hesvh.cn/Article/details/galrpfcru.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fehbvm.com/Article/details/gndmjqrrw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.hesvh.cn/Article/details/gcofchida.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.hesvh.cn/Article/details/gyilbixnu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwzgbccdo.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.hesvh.cn/Article/details/gfoafroja.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gscvnjfoj.sHtML

[M01] 读取命令行参数
来源：http://www.share.fehbvm.com/Article/details/gbfcyosdt.sHtML

Py:   sys.argv[1:]
来源：http://wap.zdbjq.cn/Article/details/gcddotcdy.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fehbvm.com/Article/details/gwzhopqsq.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gsxlxmmba.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/ghxvkiaxc.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gcxibajwe.sHtML

Go:   os.Args[1:]
来源：http://blog.fehbvm.com/Article/details/gptqzfjvd.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/ggfrailwm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gbweycpfm.sHtML

[M02] 读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gmzmeakfz.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.zdbjq.cn/Article/details/gfwpidork.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gbshimtuv.sHtML

JS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/glpvmgsxg.sHtML

TS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gzwfmdztk.sHtML

Java: System.getenv("HOME")
来源：http://baike.fehbvm.com/Article/details/gxbrziion.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gmeqizeiv.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/gbexkapeo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gsvhwddql.sHtML

[M03] 执行外部命令
来源：http://3g.hesvh.cn/Article/details/gqvvujmip.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.hesvh.cn/Article/details/gzhoovtbb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.hesvh.cn/Article/details/gkczyeuuv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gaazskrtf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gonhpjbve.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/gxsmftmjq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.hesvh.cn/Article/details/gpuarkxuc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/guxdqpyxr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.zdbjq.cn/Article/details/gnleijaky.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/gtwlcubrn.sHtML

Py:   os.getcwd()
来源：http://wap.hesvh.cn/Article/details/ghcxxzmqx.sHtML

PHP:  getcwd();
来源：http://read.share.zdbjq.cn/Article/details/gzltiffal.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gxexzjjqn.sHtML

TS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gfnhmzgff.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.hesvh.cn/Article/details/geribqqkk.sHtML

Go:   os.Getwd()
来源：http://www.blog.hesvh.cn/Article/details/geivdhpdk.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.hesvh.cn/Article/details/gzdwnxdtj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.zdbjq.cn/Article/details/gikkiujeh.sHtML

[M05] 设置退出码
来源：http://www.blog.zdbjq.cn/Article/details/gclojyuoz.sHtML

Py:   sys.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gcsdoktzg.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/gaskilfhp.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/govhhynvq.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gwrdwmuat.sHtML

Java: System.exit(1)
来源：http://baike.hesvh.cn/Article/details/gsfgwclty.sHtML

Go:   os.Exit(1)
来源：http://baike.fehbvm.com/Article/details/gnprpftiq.sHtML

Ruby: exit 1
来源：http://m.share.hesvh.cn/Article/details/glzskhxjq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/goyddtcql.sHtML

[M06] 向标准错误输出
来源：http://www.share.zdbjq.cn/Article/details/gjydafmdi.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/ggrherjqx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.hesvh.cn/Article/details/gbqchifdf.sHtML

JS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gmpnfuduh.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gdjijflcu.sHtML

Java: System.err.println("err")
来源：http://mobile.fehbvm.com/Article/details/gggbbemft.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/gcxfotqrd.sHtML

Ruby: warn "err"
来源：http://www.m.share.fehbvm.com/Article/details/gvqhbdcqr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fehbvm.com/Article/details/gumorvknf.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.zdbjq.cn/Article/details/gdcuccdwn.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.hesvh.cn/Article/details/gifneounj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/gjhurovxq.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gffjhtpox.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/grtwdqlwx.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/gscrdruui.sHtML

Go:   func main()
来源：http://3g.hesvh.cn/Article/details/gzsqukpbe.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/gbswzrfpv.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/gipbftuer.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/goxgkbtli.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/gojitaqia.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/gfqjqbswp.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/guxgantqr.sHtML


<!-- 参考信息 -->