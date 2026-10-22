代发 wailian999

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2tchkbopw.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2vieanwxg.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2badjmdfg.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2lfvdpacu.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2rjwinfit.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2ngjfvdvi.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2nzqauzzh.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2gefgtqrq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2cgftnazw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2jhfwiocs.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2pyjicnej.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2kbjtmiry.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2oldwrhsh.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2czzdpqie.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2mwaaraib.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2wrxoixnu.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2hgmkqjnc.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2jxixdusw.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ostcteaf.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2eyxccyzy.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2hrfyhjml.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2fophygln.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2vrbghwue.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2owczdpxe.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2ifikuhxz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2cmmcaynn.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2kqluhvcg.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ymhoahvx.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2xdhjlknn.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2oeyyxztp.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2ojfqqymb.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2vsiielsp.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2ezvyevyy.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2blfwdrec.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2lbdkzxad.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2seejuvrk.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ssqggsly.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2tgrebxkq.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2ilspexhe.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2hbhsowgd.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2mnmjmmwg.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2toahzqfe.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2phjapjtm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2qcqsgxzu.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2ksgfdmif.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2ljryeyap.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2tggrfnqq.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2honctixu.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2ooakgbeq.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2fxybwriz.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2epjxcrwc.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2hlafyptm.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2qjqollrp.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2eyjpqaao.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2jsvmrjkt.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ughgigog.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2hhtcntuf.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2rqeoiylj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2dzzhpbeb.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2acxokygx.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2wxzfqxzp.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2qxpfxrda.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2jtypzufz.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2aqpyzxvn.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2bliivxpl.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2jyuoctvl.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2vcspyxlz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2zqjjrhwe.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2zdnoblde.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2hfupibwz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2oroeffmk.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2ckesvicj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2uubyteqr.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2muibwohg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2akctaeus.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2fablxcpv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2htefpoqq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2ydbmgozm.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2ogglvqix.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gbdkptae.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2caitqifd.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2hchtwofv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2yhobmcwb.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uhssbztq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kaowdxkb.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2secrkpes.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cmqwdrpa.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cckwoqla.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2fvhyzrkn.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2spjybogq.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2ncbezeui.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yunbjzib.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2kckaxpaa.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2tdaebsek.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2zmbhyild.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vvzyxpdf.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2enrkdhwd.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2bqpdyxlm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2myyenjss.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2qsbdkzhf.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rjcodukd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2xtdnqmxd.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2gsxzjwtm.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2kplpjkxa.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yyszsafg.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2raocoyyd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2clrbmthc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2jauvdsdo.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wuilfdnz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uhglftbm.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2hfbmxjkv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2geknlfln.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2srshtsxz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2jqlogcne.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2qtdxkify.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2iawyfgqp.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2srubdygm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2xcnfzsul.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2wjgluavt.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ozlhkktb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2lpvvlske.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2rwolydwg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2fwlndfei.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2efqjbzop.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2ryaosahc.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2negfluej.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fiqcctqr.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2diwrccrj.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2ujbeucxq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2kklsrclo.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2fpwwxhqs.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2poaoitou.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2bmvumzei.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2qncafzhv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2gigujjvl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2qabkugmj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rgerazyt.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2laxbrpek.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2dsnvsbsm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ibbhizkz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2yjldvmmd.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2oghfxchj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ukxdaoan.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2mjhtxqdc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2bhobmaws.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2pslecsso.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ildflbkj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2vencghtk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2advzvkab.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2bxlczxnq.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2hxialbsl.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2ripulbrq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zaedkoqj.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2fbnqmrjr.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2atladrxk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2cgcohgps.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2zvmfdaij.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fwzavprb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2fdkatcgi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2csvougrb.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2fuduqytl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yyrxlugm.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2jfemulzb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2khvkuzsc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2bghttnnl.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2yllkdyuh.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2rmektzhe.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2vcczsdul.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2bizwssjv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2cnnozmju.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2yzlykbsg.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xsfnbkuo.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2prfhdzob.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2wlybgmvg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2woblcjbh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2oufkeyka.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2tztblkgu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2iakcmlxu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2ebmcuuge.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2cycsrfal.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2mbufehfh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2mmpvagal.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2tgyebodu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2pjtqbunu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2gjflfzyd.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2viaxrpyg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2gpwkwxzv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2ngvdrlmm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2swenuqlk.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2ksvckkxo.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2hqvdhxbh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2xcggdepl.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2vekzmdjo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2rsehdpeo.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2vwqrrbco.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2nqsnvtnw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2xgzxwazp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2rkhrpfvu.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2wlkxomxu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2bgvzedxg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2phyjojyo.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2lelcuwyp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2aqtvuzoe.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2ohjrnqdl.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2wiynddof.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2ohfifdbb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vdniwrju.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wnwgzjfw.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2uqefahlu.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2tnfpnfjt.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mwxlixxr.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2gzyporkq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2kffbnsbb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2vsqpkrpb.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2wsbpxpta.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2bxeedhrq.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2wrnkfhxt.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2usyabfam.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2iwjcdlhz.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2fqfccqlj.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2gttvwcpq.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2fryznxyh.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2qfgcbtwh.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2dighmvke.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2qnvfphlv.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2cztisqzb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2rcbqdxjs.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2qexvikuz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2phcjqwje.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2lbciszff.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2tzvmruaj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2lcbtfgfy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2qnksegvu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2poeeejqp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jeyaypcx.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2ynyinkfy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nerbsegp.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2wvlzroiu.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2lkwecdlm.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2vozuxphk.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2unvhllae.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2urvemisd.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2abnxnpmk.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2trhxxkxn.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2ftraplnf.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ncndelil.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xyzbkgws.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gsyqztkh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2jlvmcxlo.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2grrhhtbb.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2gnlskjox.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hepjckwr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vmusgrjp.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2pjldgamf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2gmkqghrk.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2jftmmffy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zbaaxbgr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2zfqlknzl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ogkqlzzb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2unwhkymz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2arfcudnr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2rclhlvmy.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2gbhsfdmf.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2tuubftlg.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2ufbpxjjr.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ojbgdyuv.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2pxdefbiw.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2iugpegru.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nxacezcx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2rdceoece.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gkoxxdta.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2dppgrwpi.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2sheukxni.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2kgoijmey.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2modzyzgw.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2lizkafxs.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ravntvgs.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fqqejeee.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2guajwqik.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zeeppzfj.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2qkmygulq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2hiwxulwq.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2rybvzkwn.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2jnfpjnmi.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2giuikjcu.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mledxtql.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2uekyubkg.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2kjmeteip.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2dnmjopzg.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2pdlpzqku.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2cbrgzslv.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2gudmuheb.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2xwzhydvd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2vzvvmvjx.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2nbhidvvk.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2uostgwiy.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2yesfrurk.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2zvgertwb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2jpfllrwm.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2mxodrdue.html


<!-- 参考信息 -->