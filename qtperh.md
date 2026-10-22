代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2mrodortc.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2cbjaafls.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2vyyifluc.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2uyuzntzn.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2hqyjcwnm.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2agenwovo.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2hpcfcjds.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2vkgmlvji.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2najycbvm.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2idcuntoh.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2crzijqbp.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2limepzbr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2osglkksm.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2dbhxlvcp.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2gwvcdytp.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2fxqmxikm.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2yypuhfdh.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2niopnowf.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2jlmuwvod.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2jnemcguq.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2boxqried.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2hqfnwomx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2sjfucrny.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2fuiixbly.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2vjdtgubq.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2wibzoykl.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2ogbgwqll.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2xuqictrx.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2ojxwttrv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2rrowkpdz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2hjwpttrl.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2wcygwjxy.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2dgenpmff.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2xmnnylps.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2lahqicse.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2zsllrirf.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2wqlffhxh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2xiivbeia.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2zpjyvvuz.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2lokfvjcx.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2zugbtavc.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2hiwouzvt.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2hqawzxgd.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2jqgldkji.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2jiwkzpst.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2wuiuzbfc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2mjpfjdgn.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2nnziatnu.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2nnpqtupe.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2eaapxnui.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2ouvjfbse.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2mwqynrqv.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2tgsbuwul.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2rtzcfmuf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2iweolpxx.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2lrplobvs.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2shccsoas.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2fmhkechl.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2piwyoskh.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2jyavbxky.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2rqtdremy.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2uthklqno.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2wwsqdxvu.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2xkjmfdkv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2lelozxcc.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2dsybubyo.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2wliiirxc.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2ojifsgpm.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2ahkzzrun.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2ghzywctw.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2ihypfsvg.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2xziozxfr.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2ynavyytt.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2cyknjltn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2jqcrgvsi.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2elrvpxev.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2okjpuskb.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2hytwkeue.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2cqyrczhn.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2ximckzot.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2xcalubdr.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2gskozpzz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2omdffyet.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2lckjcfgz.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2vdjvkkbr.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2iuoboxmv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2wqcunckv.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ojvugapo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ndrxwknu.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2epylknga.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qygcjcli.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2vvxvzgxa.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2hccarclq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2zebjiudp.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2hcpbrlpp.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2ydkhctll.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2rbsknann.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yhryvays.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2cniejyrs.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fzrwrydt.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2orpxeytl.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rlyvjfcn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2ejatpwoq.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2rjwlhvzt.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iqdtqbia.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2xyddxote.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2mwmzmefm.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2arbnbtfc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gqmnujzt.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2bopenaxy.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2mzbuabmd.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2dufvdhlk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2wssvzfro.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2yypurauc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gnwjdiit.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2jyzbvvyb.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2qypnbpoj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2bbzncemy.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2zqbnimiz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2swgltozg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2jcgtpyfo.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2gqqnpscj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2txausjqs.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2gyanyuxk.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2aafjzidc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2aujsrbxn.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2vxpcxugr.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2gkwauqhm.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wifgceco.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2nnkleyly.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gslpqaow.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qjmfroxp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2pbmpzbwf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2cenkcaot.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2yeiujpyh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2nhpiqykz.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2kyzibukx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2lssvrjxa.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2lkyacjdq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2taepcsfv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2ybcbjweg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2kopgxvye.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2wkxsyqcq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2weohonmb.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2jjfiklxn.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2ddeputcu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2irnsdiyz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2mqnaxfha.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2trcgulit.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ywcdudzl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2edlwxgmo.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ysheebyd.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2qkzydmeo.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2torrugsk.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2tqiawtsv.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ibgppcro.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cckzqzrk.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2vcdirmlx.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2cdlnufnh.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2mwjztids.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2ovjzlnxf.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pqwssnmv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2nepyrmcf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bgkioclu.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2mffegcxi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xtcsetjw.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2cucqtudc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2sudqfeis.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2dxhimbbp.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2svdsitui.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2fokxmmbx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2npnvnezx.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2gzujcxkp.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2anogcdrz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2vnatuzyg.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2oycnikoq.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ugkugine.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2amoigali.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2pfcrgavw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ouiyqkoc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2dwwxzaav.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2ryazknpl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2bakzglrm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2bowfikto.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2heirxdml.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2snhpjtpz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ukgxmpoq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2tdnaican.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2jejtjofp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2hvkjqucj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2qopwnrfm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2aysvyjqo.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2fcklpsuh.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2gprzxsbg.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2wqlgkcpv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2rxqcjltb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2mprsznmm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2jjvvswoz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2pioajowq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2zmgkootn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2myjdilfu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2oegkoajb.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2utnfylom.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2cmolxjlf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2ukohgmtu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2fcbaunaf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2olhznlds.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2cfphwfth.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2ivjtabtd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2diwyidnq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zkikormu.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2ofhckumw.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2qrbdzbvu.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2iumyqfnk.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2mvdfjrbr.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2cwrfkcru.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2knfherqr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2yjpfosjm.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2moadfdct.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2gcevmmav.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2rzxsmkgc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2clkwpuvx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2yanvghsm.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2yvpdsjkg.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2imfbvnex.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2ggvfpvme.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2kfucslzx.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2arpcxcpj.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2yegqumae.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2zblwwhgb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2bcihpnqu.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2wywfehyq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ftcubsfp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2pkwkvllw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2botbpfte.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2akbyuios.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2snbavwlb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2lwmcrcic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tblocvlr.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2uhmzufvq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lxxsmsdd.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2zidsoygs.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2jvzuwceb.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2orzjcngc.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ipghugey.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2bdfvtbwi.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2czlugwfb.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2kirsgftf.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2wayrwivx.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2zoyhwrye.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2pssecmid.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2gobbjkxc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ictjdehq.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2fpylttuf.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ikymyqsj.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2sudjuhpp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ydelxkcm.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2grieheci.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vypruugo.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2dwahurkm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hetiehmr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2aphtqngp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2isaewzbh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2chdlbrya.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2ojerdqlz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2kafjwdrp.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2qklozfdw.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2wybyjdlg.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2zaeafdht.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pxsiqlbi.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2afesrolw.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rlennnbg.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2evfhhagf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2ngawikhd.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2htddqzsc.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2safsdqbx.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2mgdysrai.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2cgdccazg.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zxkcllie.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2nucuvour.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lrmwnifu.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fhwudtad.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lsadofyf.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2osinkdce.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2zxjimycy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2tbzgifwi.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2sjxsnzvq.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2lnhcuafu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2fsgoikjk.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lfvfiema.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2vybhmtjg.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2pymayhdr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2ixmkrrmr.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2wfizmqgq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2uitsdnjp.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2kxsodjnh.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2rzvpplhw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2oaoyiyfx.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2atejbbcf.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2pusnzvkf.html


<!-- 参考信息 -->