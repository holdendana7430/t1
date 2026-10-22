代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2nxyqsydl.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2dhkbexhi.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2fctgirxj.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2krxinick.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2knljzrzh.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2jmtwdksl.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2vmogtcmf.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2epopbdpj.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2sfqlfcuz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2jajqjtst.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2nbjnwodd.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2umvqhxhh.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2pioszzzo.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2tnozttfc.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2hnsgyzhw.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2tvhknbof.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2hwsjedns.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2brhxecpb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2kbverbtk.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2xtjyioyj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2dplttbwo.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2hdghiaaw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2ufazmtps.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fmjrorbi.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2yyefdbmb.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2hsrxxkqd.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2iecauaqp.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2ablcikad.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2zalqpplg.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2vynljajh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2vzxaafcy.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2xhicxzzl.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2prpyrcru.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2qcvusbhp.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2tqwouukm.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2xpkkiaxx.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2eedxzvei.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2xqfllbwc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2dhikdabl.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2aklugnba.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2kefxgbwu.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2lsihhiut.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2yevmxhio.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2yfuavykc.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2nwvsmvbl.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2jbrhiqer.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2zjjyazjr.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2zwyatdwk.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2ujzzbvcg.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2qoayflgr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2xvbzojdl.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2cegonuhz.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2nbxeqyhl.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2hpwrqlpz.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2idvuflwh.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2ewifimtg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2hsqifvpy.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2oyavlfjh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2ssfbodij.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2nwfgwbjw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2nbmujmpv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2tfkgyuro.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2zabgtotq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2jemudmfg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2bjtxlnft.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2gxqplpxh.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2qanzlwyk.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2turyznnr.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2pshorhdn.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2oclkljdv.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2jlrxrzgp.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2suemkiun.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2buttzwjz.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2ndardvxw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2stpkzngb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wxmgdfoh.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2peamfjnv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2qwzfusim.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2dzgjyaqm.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2tdiitkfj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2getuyvgu.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2chanevef.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xzhwpwnq.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2opgjevde.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2beoywqae.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ajqcrvip.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2hykuusty.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2rfnqsvlh.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2uqzuhxpm.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2jrbupgob.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2cjeehugu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mskfqtti.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2btdfaqao.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2rqkuougi.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2hntyuvla.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jsjqfvos.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zddufuep.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2esduufge.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2isiytamt.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2jtjmbppd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2ephfvmef.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2qjjagpza.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2xazxqvpd.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2zqmghpqe.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2huregtle.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tdnfpvan.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2trkemppj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2lvpedcaj.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uscouonz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2wwzwkbkp.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2wdbmuijq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ptbqaejs.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2iwagxaml.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2awvqxblq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2izuyxcmk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ujcvabqn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2ifuqshzb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2gdyycqgf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2qxlejozj.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2xqfptbqb.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2pbaidqdg.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2sservaxb.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tvwhcbqv.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2hhdlmwra.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2xledorph.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2tlqgppgl.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2hpwmwgjs.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2aisovapm.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2okbvuxtk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ryjunkjn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2vrrikpud.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2pvruzrrv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2burqgdqe.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2yumpqpda.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2zzkmrqfa.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2qlollyxo.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2inmsrbie.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2sgoccrhz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2kamzrvab.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2mvxojffb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2cdrnubml.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2uvnssvid.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zbjpxnfd.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2yaibtbjh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2yubiwfoc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2tkxnzhfr.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2fkqfivxs.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2dwillpfc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jvmpvemg.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2qwcmldbu.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2okjkyvsi.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2surohjbi.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2qwiurbyv.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2dpnxfrhz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2bxmfihju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qpgchgaq.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2wnyxkqrc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cyghvymu.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2alidelxi.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2heewyxyf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2ipcjwsui.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2zywavgck.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ajmtwqah.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2wsmegluv.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2lyjdmasy.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2xrlocpmn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2necryevi.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2gecthagz.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2reeusjim.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2mouvlmyr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2xjpkajay.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2nbmbttiv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2htynakgu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2pafnpeqo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2hnvdmocf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2afmpagsm.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2anlghzgh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2fyulyzgr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2vkhigvdm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2qvvqtvkq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2eohnpagt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2iqnelotw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2uitypbaw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2ixamyfeo.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2rxdrabfe.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2zppkrwet.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2hufjpahk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2xgrdqiio.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2rlrvxgkk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2gyngiksw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2hgjlcpvw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2yndyucqu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2qjsjdyib.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ccfrkahb.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2ptkzqeur.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2rhcvvxxj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2ulqrqtda.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2daghxugj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2nzifdbqh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2phzqwjfa.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2jzldfpve.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2scifycms.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vobgublx.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2twblpcne.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2gafbduhv.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2qdbwzpve.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ufcwppcg.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2xxaevimj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2mzanrqxc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2ywlftpeh.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2hqmuacxl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2nskgxssc.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2uujdsvhi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2qskmsjou.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ifwlvtgl.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2tdrswkrt.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2zoyvreje.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2niagecow.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2kesxeqzc.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2yenotsam.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2zzvufuuu.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2ijpwntry.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2qhxlipyp.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2fxrrlabe.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2tqpanqcn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2rfekgiyd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2qmvjvukb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2kecnmmvc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ajpakzks.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2fbzvhjdg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2guvxqxes.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2rxofrtfm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qzeizgcu.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2unbyzzql.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zfrxnkog.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2ywvbsapm.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ckdnjyxw.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ydlrqmcq.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2uwyyznpn.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2jgmxpgtc.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2vxfeythi.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2bfoxphao.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2olwpcymy.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2omyagvzw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2jlzemyoa.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2cmbajpwl.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2wtkvzfmz.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2uoieioax.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lojepgwi.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2hhpzfvfc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2akjedhxm.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2iaarjelf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ruamrdma.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2ocwldupx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wtqcrjtf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2cmgoqkqy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2rhmptfma.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2itkjulol.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2wmvtwlyp.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2kwobefic.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2aricbjup.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2ymmztayy.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2dymikszj.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2qqruzepf.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ijybrhak.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2hcxmxaul.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2gjfbfgmo.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2ofucfyrd.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2ygcpeips.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2fcfxxizh.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ijhklxpe.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2sncbyfhj.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xwrgelsz.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ogqxlovd.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2liobgrqj.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uqvbmohk.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2njwiyqmp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2rkpqykag.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2nxuarqds.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2zowvkzub.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2xmwgdmga.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2begaaaud.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vzdaguxh.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2fokkmptn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2gosprgyw.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2txuiclgj.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gzwxlsof.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2vkirphge.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2pvswkdun.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2zpmyylpv.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2eevvqdnx.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2fevyttmy.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ykfondjl.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2udabpvyb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2qvqrfsax.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2gkcvrvyw.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2knvhmtgr.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2yqrqlpej.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ltfjouna.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2xfrgcfsq.html


<!-- 参考信息 -->