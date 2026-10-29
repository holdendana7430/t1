代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.hesvh.cn/Article/details/gvmhwkolo.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.zdbjq.cn/Article/details/gtqsrabsw.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fehbvm.com/Article/details/gbvwslchv.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.zdbjq.cn/Article/details/gchgvxnuf.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.fehbvm.com/Article/details/gzjvayspj.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.zdbjq.cn/Article/details/gjoiaxloc.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.zdbjq.cn/Article/details/gduaagcky.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gqhasblkl.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/giiefcqcr.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gxfvuhars.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.fehbvm.com/Article/details/ggfigydcz.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gozzwnezj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.hesvh.cn/Article/details/giuoxcxyr.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.zdbjq.cn/Article/details/gctykfyoe.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.hesvh.cn/Article/details/glnphfbix.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.zdbjq.cn/Article/details/giczhcwen.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.fehbvm.com/Article/details/gbgqepkbv.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.zdbjq.cn/Article/details/gplfstyqv.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.fehbvm.com/Article/details/gmipmrhlx.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.hesvh.cn/Article/details/guixngasw.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.hesvh.cn/Article/details/gwzaitqay.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.fehbvm.com/Article/details/gofbrcleh.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.fehbvm.com/Article/details/ggzzvyvko.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.hesvh.cn/Article/details/gueqyybab.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.hesvh.cn/Article/details/gztorbosc.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fehbvm.com/Article/details/gynbibgfz.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.zdbjq.cn/Article/details/ghwhzutzl.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.fehbvm.com/Article/details/gmmvynlra.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.zdbjq.cn/Article/details/gztplkhts.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.hesvh.cn/Article/details/gkkodohrn.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.hesvh.cn/Article/details/gkpbckwqm.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.zdbjq.cn/Article/details/gipcmvyjz.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.hesvh.cn/Article/details/gcsssqist.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.zdbjq.cn/Article/details/guyscfogv.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.zdbjq.cn/Article/details/gehbylluo.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.hesvh.cn/Article/details/gtlrvxewb.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.hesvh.cn/Article/details/gjfqtiqzo.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.hesvh.cn/Article/details/gaekhdhav.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.zdbjq.cn/Article/details/gevpzsjjo.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.zdbjq.cn/Article/details/gikvsypxn.sHtML

[J07] 比较两个日期
来源：http://www.blog.fehbvm.com/Article/details/gnuroplew.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/gpygdyugl.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.hesvh.cn/Article/details/gioyeygpm.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.hesvh.cn/Article/details/gkcrptbwz.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.hesvh.cn/Article/details/gurodiikh.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.zdbjq.cn/Article/details/gpbupaarf.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.fehbvm.com/Article/details/gqesfnjwo.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.zdbjq.cn/Article/details/ghfcxwqcb.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.fehbvm.com/Article/details/gwmkaxmxk.sHtML

[J08] 提取年月日与星期
来源：http://wap.hesvh.cn/Article/details/gklebbdjk.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.fehbvm.com/Article/details/gcqgxwdui.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.zdbjq.cn/Article/details/gliykozdx.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.hesvh.cn/Article/details/gscgsrsoq.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.zdbjq.cn/Article/details/gyvyyqizz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.hesvh.cn/Article/details/gbthdvfxn.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.zdbjq.cn/Article/details/ghjswqfjf.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.zdbjq.cn/Article/details/gvjrtfspj.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.fehbvm.com/Article/details/glbvcieag.sHtML

[J09] 时区处理
来源：http://mobile.fehbvm.com/Article/details/gwgnzikrh.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.hesvh.cn/Article/details/gsteotnan.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.hesvh.cn/Article/details/grvetiidw.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.zdbjq.cn/Article/details/gyrgdbvba.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.zdbjq.cn/Article/details/gruijbeoe.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.zdbjq.cn/Article/details/gwpmcqnqp.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.hesvh.cn/Article/details/gasvlfqqq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.fehbvm.com/Article/details/ghfxyhiya.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.hesvh.cn/Article/details/ghzxiqfpr.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.hesvh.cn/Article/details/gkgnwgnfl.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.zdbjq.cn/Article/details/gxucrippn.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.zdbjq.cn/Article/details/gyoddmggb.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.hesvh.cn/Article/details/gnglwyzuv.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gbatirufm.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.hesvh.cn/Article/details/gdhexvoed.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.zdbjq.cn/Article/details/gdciqctgz.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.zdbjq.cn/Article/details/guuufntgf.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.fehbvm.com/Article/details/gxzvcmgwl.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gozptetyp.sHtML

K. JSON 与序列化
来源：http://3g.zdbjq.cn/Article/details/gxwiefxmn.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gdyodluso.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.fehbvm.com/Article/details/gkelmavgz.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.hesvh.cn/Article/details/gwsnqtvgl.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.zdbjq.cn/Article/details/gdiamwqqk.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.zdbjq.cn/Article/details/gqfdyaajs.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.zdbjq.cn/Article/details/gbxhjsxzt.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.fehbvm.com/Article/details/gznhpgtly.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.hesvh.cn/Article/details/grgswizss.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.zdbjq.cn/Article/details/grqfwinsd.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.fehbvm.com/Article/details/gchdeozho.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.hesvh.cn/Article/details/gebkobrij.sHtML

Py:   json.loads(s)
来源：http://3g.fehbvm.com/Article/details/gddbatycu.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.fehbvm.com/Article/details/gwsymkeun.sHtML

JS:   JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/gztuihcxv.sHtML

TS:   JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/gufuelzxi.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.hesvh.cn/Article/details/gciblutzf.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/gnjcpnclj.sHtML

Ruby: JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gfuxizpri.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.zdbjq.cn/Article/details/gdqsaxnjp.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.fehbvm.com/Article/details/gamuoayoq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/ghwqlgoea.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.fehbvm.com/Article/details/gkhrnvpew.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.zdbjq.cn/Article/details/ggdaawzvx.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.zdbjq.cn/Article/details/gctayrpjb.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.fehbvm.com/Article/details/gswnjpqtx.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.hesvh.cn/Article/details/gxitkjaeq.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.fehbvm.com/Article/details/gvfudzgnh.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.zdbjq.cn/Article/details/gkzweedwc.sHtML

[K04] 读取 JSON 文件
来源：http://blog.fehbvm.com/Article/details/gjbkgnbki.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gfycktigx.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.fehbvm.com/Article/details/ggcczubwp.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fehbvm.com/Article/details/gxdnhabts.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.hesvh.cn/Article/details/gahszendx.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gkkboffdc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.zdbjq.cn/Article/details/giagtdpgp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.hesvh.cn/Article/details/gswptgnsy.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gubcemaqs.sHtML

[K05] 深拷贝对象
来源：http://read.share.fehbvm.com/Article/details/gzpqphjvm.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.zdbjq.cn/Article/details/gputobptt.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.hesvh.cn/Article/details/gkdcaycsb.sHtML

JS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/givypjzog.sHtML

TS:   structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/glsmwxmjo.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.fehbvm.com/Article/details/gqehzbmmc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.fehbvm.com/Article/details/glhbecomy.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.fehbvm.com/Article/details/ggrxjjwyd.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.fehbvm.com/Article/details/gpcuujtsy.sHtML

[K06] 解析 URL 查询串
来源：http://wap.hesvh.cn/Article/details/gimyjieau.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/gdbxgdcgi.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.fehbvm.com/Article/details/gzajqgsyy.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/gmnhcvdaa.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/gmrfsfdlq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.fehbvm.com/Article/details/gmpadnkom.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gewfoeglj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gayvjwitl.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gireahtlo.sHtML

[K07] 进制转换
来源：http://www.blog.zdbjq.cn/Article/details/gxqqrmotd.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gjciazuls.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.fehbvm.com/Article/details/gjfxmxsly.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gtpmjxmyb.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gqpvqeond.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gacziidna.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.hesvh.cn/Article/details/glmtlmrha.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.fehbvm.com/Article/details/gkkrexcbu.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gmxalzfov.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.zdbjq.cn/Article/details/gjgucawkc.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gaztqnerq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.fehbvm.com/Article/details/glzillyuz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gtebzcqdp.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/gmbozkxog.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.fehbvm.com/Article/details/gkdqomnzf.sHtML

Go:   encoding/gob
来源：http://www.share.zdbjq.cn/Article/details/gvgkkqvtq.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.zdbjq.cn/Article/details/gftvixsne.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/gmlqsweqf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/geufgcawl.sHtML

L. 网络请求
来源：http://blog.zdbjq.cn/Article/details/ghbjwolvh.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnljanjbq.sHtML

[L01] 发送 GET 请求
来源：http://baike.hesvh.cn/Article/details/gthpllchu.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.fehbvm.com/Article/details/goumnrsvl.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.zdbjq.cn/Article/details/gadwymbfd.sHtML

JS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/godqyasmw.sHtML

TS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/geyikbypj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fehbvm.com/Article/details/gghvovqbm.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.zdbjq.cn/Article/details/gsemaxrto.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.hesvh.cn/Article/details/gosmzkyum.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fehbvm.com/Article/details/ggsjhhdio.sHtML

[L02] 发送 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gdapkkwqu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gksbcliaj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.zdbjq.cn/Article/details/gejxlhthq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gpkbsesgt.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gystfocmy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.zdbjq.cn/Article/details/gwhfmiymx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.hesvh.cn/Article/details/gyqpobgxd.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.hesvh.cn/Article/details/gvhexzuha.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.hesvh.cn/Article/details/gtkctgxam.sHtML

[L03] 设置自定义请求头
来源：http://blog.zdbjq.cn/Article/details/ghhlzfpfw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fehbvm.com/Article/details/grotbmmgg.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.hesvh.cn/Article/details/gcxqhgacz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gzjqngfkd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gbpcbvknj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.zdbjq.cn/Article/details/gdrckdxkj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gifwawahm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.zdbjq.cn/Article/details/gmvvnwakt.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/gfigiuofg.sHtML

[L04] 设置超时
来源：http://mobile.fehbvm.com/Article/details/gzuuaadob.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.hesvh.cn/Article/details/gmdbafcoj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.hesvh.cn/Article/details/gktvjchrp.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gdffjvqpp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/ggbergjty.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.zdbjq.cn/Article/details/gtbmdpaso.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.zdbjq.cn/Article/details/gavpttodc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.zdbjq.cn/Article/details/gmsncjoov.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gtzpvcokj.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.fehbvm.com/Article/details/glsehvveb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.hesvh.cn/Article/details/ggvcoxhju.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fehbvm.com/Article/details/gwbvxsbcb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gedjstfcn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gkuuqnmru.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.fehbvm.com/Article/details/gomsjdxlr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.hesvh.cn/Article/details/gzubpgimb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.zdbjq.cn/Article/details/gbiegoeiq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.zdbjq.cn/Article/details/gyhqnsqws.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.hesvh.cn/Article/details/gdglfsbiy.sHtML

Py:   resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gbhejejmj.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/gkjctjwhz.sHtML

JS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gaoqeccgb.sHtML

TS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gupznnuab.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.hesvh.cn/Article/details/gyfwuxhxu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.hesvh.cn/Article/details/guihfrdbr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fehbvm.com/Article/details/gfkelwsbq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fehbvm.com/Article/details/ghrgoefdt.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/goxfbjazb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.hesvh.cn/Article/details/gccjtbopg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.hesvh.cn/Article/details/gtigrxiyf.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gdrrwgvqf.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gaoymleek.sHtML

Java: resp.statusCode()
来源：http://read.share.hesvh.cn/Article/details/gqjvkbvzp.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gvwjydkrz.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.zdbjq.cn/Article/details/guspbvlwg.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gujaqesnf.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.zdbjq.cn/Article/details/gnipwpowg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.zdbjq.cn/Article/details/gortgyeks.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.zdbjq.cn/Article/details/gitdufvxn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gqleteipf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/grcwwsgdk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fehbvm.com/Article/details/gmsuujiwd.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fehbvm.com/Article/details/gnsvnpvjp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gqrbwbzlg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.zdbjq.cn/Article/details/gdumqkpbh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gyjjeogvn.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fehbvm.com/Article/details/gvgdvfenp.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gaacokrzl.sHtML

[M01] 读取命令行参数
来源：http://baike.zdbjq.cn/Article/details/gmhsljsyf.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/gakkvzcia.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fehbvm.com/Article/details/guyxxdguc.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gigtefbor.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/ghgayntut.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gvcfxbhpj.sHtML

Go:   os.Args[1:]
来源：http://wap.hesvh.cn/Article/details/gdwhhhbom.sHtML

Ruby: ARGV
来源：http://baike.hesvh.cn/Article/details/gtspqzmne.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gphrkpfbb.sHtML

[M02] 读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gztljgbhh.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fehbvm.com/Article/details/gctgxltrf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gzzsnmkeo.sHtML

JS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gomnisgxh.sHtML

TS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gjptfxfpc.sHtML

Java: System.getenv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/grzvrqxjp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gjaytoibx.sHtML

Ruby: ENV["HOME"]
来源：http://3g.zdbjq.cn/Article/details/goraogsys.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gybuconiz.sHtML

[M03] 执行外部命令
来源：http://3g.hesvh.cn/Article/details/gqzixlzvv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fehbvm.com/Article/details/gankcfgqj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/gkgxbpllk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/ghluziasz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/geacfjbsv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/gvbonngue.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.hesvh.cn/Article/details/gijrhjgjo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.hesvh.cn/Article/details/gqgkcnmsz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/ggsozdbbc.sHtML

[M04] 获取当前工作目录
来源：http://baike.zdbjq.cn/Article/details/gmmdrhzlb.sHtML

Py:   os.getcwd()
来源：http://www.blog.fehbvm.com/Article/details/gcrhqqjgg.sHtML

PHP:  getcwd();
来源：http://www.m.share.hesvh.cn/Article/details/ghapzyecg.sHtML

JS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gfxmcldbq.sHtML

TS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gemoinnjp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fehbvm.com/Article/details/gdpfprnxj.sHtML

Go:   os.Getwd()
来源：http://read.share.hesvh.cn/Article/details/ggcpbcayu.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/gqflxsrpu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.hesvh.cn/Article/details/gncmfdgnz.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/glrzgoooa.sHtML

Py:   sys.exit(1)
来源：http://3g.fehbvm.com/Article/details/gngoakbpw.sHtML

PHP:  exit(1);
来源：http://www.m.share.zdbjq.cn/Article/details/grnvuxajt.sHtML

JS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gavklsdob.sHtML

TS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gnqolkhru.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/guehxrrfy.sHtML

Go:   os.Exit(1)
来源：http://baike.fehbvm.com/Article/details/gqotszpsh.sHtML

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/gwquxwbrf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.hesvh.cn/Article/details/giiltphlr.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/gxljdbaym.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gxbseascj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.hesvh.cn/Article/details/grxszrbmp.sHtML

JS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gafqlehmt.sHtML

TS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gzfeakxad.sHtML

Java: System.err.println("err")
来源：http://baike.zdbjq.cn/Article/details/gfjbihhkz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/gisgkgzoi.sHtML

Ruby: warn "err"
来源：http://blog.zdbjq.cn/Article/details/ggjlbidck.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gjeavtxqr.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/gjhfgdgoj.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/ghhrtrapu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/gmrtamsfn.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gtxmchdeh.sHtML

TS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gnrsrltcx.sHtML

Java: public static void main(String[] args)
来源：http://www.share.zdbjq.cn/Article/details/gqqpmurxc.sHtML

Go:   func main()
来源：http://wap.zdbjq.cn/Article/details/gadndybpy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/gesqutmjw.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/gmnhqhtin.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.zdbjq.cn/Article/details/gucdwkcmg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.zdbjq.cn/Article/details/gzxnkowzu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fehbvm.com/Article/details/gykteuikr.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gabvufsex.sHtML

TS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gaepoykub.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.hesvh.cn/Article/details/gdxdnvlbt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fehbvm.com/Article/details/gzqffetem.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gwfsfytym.sHtML


<!-- 参考信息 -->