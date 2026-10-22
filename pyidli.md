代发 wailian999

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2atqugldh.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2thmasmiw.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2kxzdoxxj.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2lgwtawvn.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2vxywcgne.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2ucdntuix.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2xkpfmvyq.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2iyfcrycn.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2elicmsjp.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2urboxczx.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2mcnfkpam.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2tlqbcpsx.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2xxtzbqvx.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2gnggyrnh.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2ixiwbdga.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2mhpemonu.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2szbqnrie.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2sitodokh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2jvioaeeb.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2xizrlfkh.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2bdzjsach.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2uclpcowb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2eaatidmy.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2wlgjdywg.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2avaesgvc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2wtbvsmmn.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2fezvzmpx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ckjrmptq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2wwcohhio.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2hqngqzfk.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2rkbtmhzk.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2wefchogr.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2bcqekccv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2julapzgq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2axsbofhn.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2ydkydnvm.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2fpuscfrt.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2oowlznji.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2wtxumwbs.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2ubstgtnp.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2kkmjjvrm.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2xutupqzy.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2gvchuqgv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2xuxthvvy.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2lqfurfvv.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2abybmuur.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2elrteglf.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2xdkrgogp.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2tacrvgfi.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2rzqvqnjy.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2emdwvukr.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2bacoljvz.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2swzxkevz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2fosehozk.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2ubnyhujn.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2yrkamfht.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2iiceemuu.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2hwugzyot.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2ircoklzy.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2xoapxotr.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2tcpmfcgd.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2vbpubxnh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2simdzajy.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2gvdkkawk.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2psoaswkm.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2zwphtpkv.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2bspnmnng.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2gokwmxut.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2wnnxqbtv.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2homxgjxa.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2joawonhb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2mbbnfplu.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2tqtnumyk.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2eqfdxreu.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2qinxegnj.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2ekeivqjx.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2qqjqjykx.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2ylhursdu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vzorjuef.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2gjwwhnit.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2aslbiihh.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2sldoglcz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2rfcjnbwd.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2btfaddrk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ceqpmvja.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2aenghbba.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hcgzkqrz.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2xmnkwcmt.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2jlrflbmv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2obbqfkxy.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2rxwzydel.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rqtywqhd.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2iqswemju.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mcrcnpih.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2svlvhhkv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2qthadudb.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2ntnndddp.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2ioxnsuul.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2endtjcnj.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2bcuxxqqo.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mcynwfwu.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2aceydfuy.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2cerlhxjt.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2rtolswoh.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2kzuevznl.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2euhbzaoj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2jizfhubb.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2sviptoxz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2psqameiz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2shztjfau.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2vshmkwki.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2sbtodejt.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2wmciqqjo.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2dfaespyo.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2fmaxctbl.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2rdkpvrqp.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2zxydiunb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2qmogsvjo.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2pndpvqnw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2srgnfiql.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2wcbyxkxg.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2cmjbotvb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2hndwjdur.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2iwuryajg.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2btchmqlk.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2tkmkpwrq.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ewhbnmii.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ctuzcike.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2uclosthk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2ctjbxznw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2qtxbmbkl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2paafxkio.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2fiogyhvh.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ojjuuycl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2uaqwqkvc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cyhenyiu.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xqhhuawq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2serlxmka.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2nofoffqh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ffbpkwmt.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2okizsqle.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2hzyirqal.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2kkobxleo.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2mtaicmov.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ygkmuaxp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2wjcfwmye.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hzkjpojv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2vymujaip.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2zqizypxs.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ptshypbh.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2alojtwxr.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2szibkcaj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ojdidbse.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2tbjkgrsc.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2detxyboh.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2qzhyvrkc.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2mntmxjyg.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sgkfktbj.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2prjmorbx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2harodqvz.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2srgtjhgt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qjnetoki.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2zkwvmwpb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2rdycwrgu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2znlgnuhb.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2tzzesjpz.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2onnblwcq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2wmvnrbef.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2rhadqiul.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2qyjkdnbd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2hvpdlqhm.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2fdfokvsw.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2cuhryatf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2lekunohh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2qfsujvxg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2tnrcftwa.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2oywuyeow.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2trfplelz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2lefuoaxr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2psttxaej.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2nesgzsec.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2enmuaycv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2dtmaqrdh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2cnecqktd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ecsbqbcq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2mhfftryh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2swyspzvv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2iocoevop.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2tagnjaai.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2ncvbjfrz.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2axsmclqf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2uvhyyjgh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2bpyxvnbc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2rhdfqrfe.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2zxlxvsro.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2naglfnzl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2fihqxstb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2semvfsaa.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2eoqsqgwa.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2cyzuuuea.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2unqptwke.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2gdswncof.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2yewznfiq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2trqfvoje.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2xzhzxozl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2caugbkwx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xbbkhpno.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2pqkkucue.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2llndbfvx.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2teauksxw.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2jqiyvxlo.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2qgojkkmk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2hxnjvoym.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2poijhcwk.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2popbxhoe.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2uiqrvlos.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2rpyvcluf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2jdmxnizw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2bympynws.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2yiyzonfs.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2uufhgtxp.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2tnshysxs.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2chtwdzgh.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2qbutsjwz.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2qwrdsvmt.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2dxrcysfq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2qgupbegi.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2ojbmhpny.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2houqdvjv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2pdywmzox.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2vidrmczv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2sxtbkmfw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2tniaktac.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2ozvmnght.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xgwygats.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2aapkcola.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2padzssxa.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2pwsaxasg.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2wcmgrvrn.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2emsibxdb.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2pnchttkl.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ejevgbaw.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2euttzzye.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2rceyiycq.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2tuuyejob.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2owopwoyd.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2jmdyzhtz.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2sxrkdjpo.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2iwuzpuqb.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2okrrhgoj.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2fkwcsahf.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2inhmpomg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qhpatota.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2ofwbcsyp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jilxlbgg.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2tulifweb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mzphwzeh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2iwpalwuv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dzttshmi.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jmgqggnl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2zlwwdtcw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2xjappihj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2zikoaivv.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2edatqmvh.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2uktlwbat.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2ytpokemv.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2tmihoeeg.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2yftkdjuo.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2yzpaveat.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2wqkjddhn.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2zmibvzxf.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2ilhvyotj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2bpnzzopv.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2jcozdaan.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dhdejkqj.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2fblupgmr.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bopnttdd.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2alcyytle.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sxiatyns.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2eqgpegul.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2jjfpvone.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2gjkgztof.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2loitowkw.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2lkgdovwl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2vdlcapmq.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wrzqbxpr.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wasaabfh.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2maxjhftf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2wgctisyn.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2jzkeblni.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wuwlsgwh.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2zqxuyiay.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2gjnpipai.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2uceprasw.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2jpmgzcxk.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2hpjfsxwk.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2xayebjmy.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2glcauloj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2vmvaliya.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2dsvleavf.html


<!-- 参考信息 -->