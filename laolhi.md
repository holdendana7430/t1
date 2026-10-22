代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2ldtcjkgo.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2oasqrkye.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2axcjygwa.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2igianfbx.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2zbycnoqx.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2mwwwwjnf.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2eywiedlw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2izucadxz.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2ppuhgdkq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2elkxpswf.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2yjdetzav.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2llbypovd.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2exiqjamt.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ncsaoolc.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2wucvsqma.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2aqhyibsf.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2gxouxscg.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2lzgvdgdv.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2srogwcxj.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2cpmnmmtk.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2hcxpisig.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2icaysyon.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2fecrafyt.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tytvkofn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2cbmqmrwe.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2iuwlityx.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2dhrujhnl.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2zvrgvmai.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2ukikpcqe.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2msvjzhet.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2raaubdpe.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2kofsfmdn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2ygwmfevr.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2vcsojxwk.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2fifhbatd.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2zykwifsb.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2kpqjipsu.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2dpbsmhrz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2bldocvst.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2yjcwboys.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2skzxhvcq.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2mkmtxwaw.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2youdacek.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2ijlzsids.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2oeizlcza.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2yfelodss.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2viuvedzk.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2xyoazvjw.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2yuogozsj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2sqnezimi.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2kmvpwvnn.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2hrgkqxhd.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2cqcswbet.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2mupqbffb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2dbyvkygp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2hougwqka.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2emdpzwdy.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2gnnpdizk.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2bptivcut.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2vxytmpmw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2xpoidzpf.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2bmsutgxo.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2vsivtdnr.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2asfpeyxd.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2ujpewxli.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2uenjgxoc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2yrjygtiq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2mqjotkuo.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2ftiatvny.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2swsetlkl.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2sumarpar.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2imiltbmh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2feuqcxhk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2mqgmtrjy.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qrkygdjj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2nxvgfofa.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lttxiaji.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2vunwxvui.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2jngjvbqz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2peaqizlq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hnkqeann.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2kmskfqxz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xzktfmhr.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xjajvktv.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2vwjzycct.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2pjufpswz.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uegnupgn.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2chrknmnw.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2cewxqter.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2sarphudr.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2orobcpee.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bcfiihee.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2xxxyublw.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2vlozfiud.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2kqqaqkre.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ukqjbonp.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ueakcdpb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2awacutou.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2fjdmqfyr.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2cnkemwoa.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2zyezarqi.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2jhvwwymf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2gryqrhgf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2dstlbmsr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2szjsndpo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lbjuvxtc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dfkdmpvp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2vegucfan.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jfmwrinz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2lehnrmru.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2kscbeklt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2kfyseswz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2zwetudgu.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2ajhbfakd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2tlynbekk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2jejbjcky.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2uoesiynr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2tvuhqcvf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2oaakppav.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2qlulbscc.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wggavmuq.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2vdayusdj.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2lzozhhdx.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hdmwunkt.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2ydtslmvm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2bdkhblhl.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2wvnbxazv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2suavjdbq.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2crgohxjc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ldnuwfnn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2ivtaiggf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2dtkpxwgd.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2aitkrgiw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2zlqyhkwb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2niyblogd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2olsajvbl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2jtmdxssf.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2jtvnmuov.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zmxblqwi.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2wozhdrif.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hmozwghh.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2bvkjxuwc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2byztzpql.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2uiejhgbr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2baqbjtlu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2btdpemrc.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2auhnxyoo.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2zlfzhqye.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2lcjazywb.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2erwulcdk.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2mquuekoz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2ffwunjro.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2yvrrxkwf.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2iszleqrp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2vqqiwwwz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dsoxgwbo.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2kwtsunfy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mjvqnvdn.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2qaywwmqz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2bamxlvpu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2lmdpkopw.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2lixluddm.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2sznxfeoh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2gplfkjaq.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2kmrxpgql.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2djbnznxq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2bqkswfjb.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2nuwaqvfr.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2kqvkwnww.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2bwrczewi.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2zhmaqmkm.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2lfvckntj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ywbovppx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2qdonrflo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2uyhuadom.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2vtgubzje.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2zkhbswxd.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2zcqoufrb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lbywixbq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2pgmsgzuz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2klkswglm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2dzagofja.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ywcavctx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2djatadfd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2mjhskrit.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2voafqyvg.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2evukszss.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2ctgkcpuu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2lhyllehl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2fuczcvbh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2vkumjrxb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2totrpocl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2bfwkfchk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2rawdcewe.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2sxrvhaqx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2gpmeohht.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2yupvhaqh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2pxdzhjzk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2gdfuriql.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2baaexpar.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2soiatnbv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2dkexjrqz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jdrijugc.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2cwoaqjzg.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2vhfxesvd.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2irmphzod.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2xhlwahcz.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2cragpjuh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2cptkrlkb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2vjdyedey.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2jdlaumyc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2fptuphcj.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2qgdodrpg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2lqagtzhv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2sszlycvt.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2sqptxmxi.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2pekpyixk.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2zofrdhkc.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2montlioz.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2ormadpkj.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2zxhlvxnn.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2wkjggqhp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2dgljfbju.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2xgzrefif.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2kqcwtzxi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2uyglmjzk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2tdzftjbg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2khasrfpl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2fvnapwuk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2fdjivirj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2plwsgfph.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2kifamyxj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qfhxarkr.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2naawoafg.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2wjmsfbgt.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2hlopigex.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wrakdybs.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2luxqvbgv.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2zbazfmtv.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2qbiduptd.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2jglftqlc.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2voylnyne.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2sytaoxzu.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2sfnkthzj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2oqnqtgne.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2hxamzxdi.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2dyjinqyq.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2obcweydn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lvxtlszm.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2lfvjpioq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qthciaqs.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2yfazaqsn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fiqrjgaf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2retvbcza.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2poyfpztv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2fojsskch.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2ozxujale.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2zuwlllil.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2sguglvzb.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2autqjbcb.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2yhaeppyk.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ncwxjnpm.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2nurgmfxh.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2rpvjqqso.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2nqmdrxtp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2mtxzofhs.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2nxbohpbz.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2cwwfpnkb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2pqwmprby.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2hdhtvihg.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rsrwwlyr.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2yjdkngdt.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wwdyrmow.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wjqqxwwk.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ujvvstkk.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ksbolsrf.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2bqdmvhee.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2gytnnyxh.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2olmxujgz.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2butcxipw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2iiplcrzv.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mbpkryrp.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2axtnypnp.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2axvzfwuw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2boivdqoq.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2fadqejjr.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2shklfgik.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2tovajquq.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2lrnnytnp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2jrlyzuzo.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2urdgcsan.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ylcfhafs.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2zgmmzwyd.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2syugzpak.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2tjhbotyh.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2dltludns.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2hdmumokl.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2idtosjou.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2nqujezhi.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2wlmtmqzk.html


<!-- 参考信息 -->